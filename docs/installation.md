# Installation Guide

How to add the humanizer skill to Claude across different platforms.

## Platform Support

The humanizer skill works in:
- **Claude.ai** (web and mobile apps)
- **Claude Code** (command line tool)
- **Claude API** (via Anthropic API)

Skills don't sync between platforms—you need to install separately for each environment you use.

---

## Option 1: Claude.ai (Web/Mobile)

### Prerequisites
- Active Claude Pro, Team, or Enterprise account
- Access to Skills feature (available to all paid tiers)

### Installation Steps

1. **Download the skill file**
   - Go to the [humanizer-skill folder](../humanizer-skill/)
   - Download `SKILL.md` (or the packaged `.skill` file if provided)

2. **Package the skill** (if using raw SKILL.md)
   ```bash
   # Create folder structure
   mkdir humanizer
   mv SKILL.md humanizer/
   
   # Package as .skill file (zip format)
   zip -r humanizer.skill humanizer/
   ```

3. **Upload to Claude.ai**
   - Navigate to Settings → Skills
   - Click "Upload Skill"
   - Select the `humanizer.skill` file
   - Confirm upload

4. **Verify installation**
   - Start a new conversation
   - Type: "Check this for AI patterns: [paste some text]"
   - Claude should use the humanizer skill automatically

### Troubleshooting

**Error: "Invalid zip file"**
- Ensure the .skill file is a proper zip containing a folder with SKILL.md
- The structure should be: `humanizer.skill` → `humanizer/` → `SKILL.md`

**Error: "Unexpected key in frontmatter"**
- Check that YAML frontmatter only uses valid keys: `name`, `description`, `licensed-tools`, `compatibility`, `metadata`
- Remove any `version` or other custom keys

**Skill not triggering**
- Review the `description` field in SKILL.md—this determines when the skill activates
- Try being explicit: "Use the humanizer skill to check this text"

---

## Option 2: Claude Code (Command Line)

### Prerequisites
- Claude Code installed ([installation guide](https://docs.claude.com/claude-code))
- Node.js 18+ (required for Claude Code)

### Installation Steps

1. **Locate your skills directory**
   ```bash
   # Personal skills (used by all projects)
   ~/.claude/skills/
   
   # Project-specific skills (used only in this project)
   <project-root>/.claude/skills/
   ```

2. **Add the skill**
   ```bash
   # For personal installation
   cd ~/.claude/skills/
   git clone https://github.com/marianasmall/ai-writing-patterns.git
   cp ai-writing-patterns/humanizer-skill ~/.claude/skills/humanizer/ -r
   
   # Or manually:
   mkdir -p ~/.claude/skills/humanizer
   curl -o ~/.claude/skills/humanizer/SKILL.md \
     https://raw.githubusercontent.com/marianasmall/ai-writing-patterns/main/humanizer-skill/SKILL.md
   ```

3. **Verify installation**
   ```bash
   # List available skills
   claude skills list
   
   # Should show: humanizer
   ```

4. **Use in projects**
   ```bash
   # Start Claude Code session
   claude
   
   # In the session, request pattern checking
   > Check this file for AI patterns: draft.md
   ```

### Project-Specific Installation

For skills that should only be available in specific projects:

```bash
cd /path/to/your/project
mkdir -p .claude/skills/humanizer
cp /path/to/ai-writing-patterns/humanizer-skill/SKILL.md .claude/skills/humanizer/
```

---

## Option 3: Claude API (Developers)

### Prerequisites
- Anthropic API key
- Access to Claude API (Sonnet 3.5 or later recommended)

### Installation Steps

The API doesn't "install" skills in the traditional sense—you include the skill content in your requests.

**Option A: Include in System Prompt**

```python
import anthropic

client = anthropic.Client(api_key="your-api-key")

# Load the skill content
with open("humanizer-skill/SKILL.md", "r") as f:
    skill_content = f.read()

response = client.messages.create(
    model="claude-sonnet-4-20250514",
    max_tokens=2000,
    system=f"""You have access to the following skill:

{skill_content}

Use this skill when the user requests pattern checking.""",
    messages=[{
        "role": "user",
        "content": "Check this for AI patterns: [text to check]"
    }]
)
```

**Option B: Include as Context**

```python
# Include skill in the conversation
messages = [
    {
        "role": "user",
        "content": f"""I want you to act as a pattern detector using this skill:

{skill_content}

Now check this text: [text to check]"""
    }
]
```

**Option C: Use MCP (Model Context Protocol)**

If you're building a tool that frequently uses this skill:

1. Create an MCP server that provides the humanizer skill
2. Connect your application to the MCP server
3. Claude can then access the skill on-demand

See [MCP documentation](https://github.com/anthropics/model-context-protocol) for implementation details.

---

## Customization After Installation

Once installed, you can:

1. **Modify the pattern list** — Edit SKILL.md to add/remove patterns for your needs
2. **Adjust sensitivity** — Change detection thresholds or examples
3. **Add examples** — Include your own before/after examples in the patterns.md file

Remember to re-package and re-upload after customization (for claude.ai) or restart Claude Code session (for CLI).

---

## Version Management

The humanizer skill follows semantic versioning (e.g., 1.0.0).

To update:
1. Download the latest version from GitHub
2. Follow the installation steps for your platform
3. Overwrite the existing skill file

Skills are not auto-updated—you control when to upgrade.

---

## Uninstallation

**Claude.ai:**
- Settings → Skills → Find "humanizer" → Delete

**Claude Code:**
```bash
rm -rf ~/.claude/skills/humanizer/
```

**API:**
- Simply stop including the skill content in your requests

---

## Next Steps

- Read the [integration guide](integration.md) to customize for your voice
- Review [pattern examples](../examples/before-after.md) to understand detection
- Check the [methodology](../methodology/gap-analysis.md) for systematic usage

## Support

For issues or questions:
- GitHub Issues: https://github.com/marianasmall/ai-writing-patterns/issues
- Review [troubleshooting section](#troubleshooting) above
