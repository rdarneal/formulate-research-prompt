# Create Research Prompt

A Claude Skill that generates structured, domain-specific research prompts ready to paste into Perplexity Deep Research (or any AI research tool). It classifies your request, selects the right template, and outputs a comprehensive prompt — it never answers the research question itself.

Three domains are supported:

- **Technical** — engineering, architecture, integrations, DevOps, tooling
- **Strategic** — market analysis, competitive positioning, org design, GTM
- **Learning** — training design, instructional programs, capability building

## Files

```
SKILL.md                  # Skill definition (orchestrator)
resources/
  technical.md            # Technical architecture template
  strategic.md            # Strategic business intelligence template
  learning.md             # Learning & instructional design template
```

## Installation

### Option A: Download the zip

Download `create-research-prompt.zip` from this repo's root.

**Verify the download:**

| Platform | Command |
|----------|---------|
| Mac/Linux | `shasum -a 256 create-research-prompt.zip` |
| Windows (PowerShell) | `Get-FileHash create-research-prompt.zip -Algorithm SHA256` |

Expected SHA-256:

```
d1bc378ef14a001b569ee008349abb0cfa7c01f67d92d8b90b50e9a4fc5f9c63
```

For Claude Desktop, drop the zip directly into the skill importer. For Claude Code, unzip the archive and follow the steps below.

### Option B: Clone the repo

```bash
git clone https://github.com/rdarneal/formulate-research-prompt.git
cd formulate-research-prompt
```

---

### Claude Desktop / claude.ai

Installation is the same on Mac, Windows, and Linux — everything is done through the app settings.

1. Open Claude Desktop and go to **Settings**
2. Navigate to **Capabilities** > **Skills**
3. Click the **+** button to add a new skill
4. Drop in the `create-research-prompt.zip` file
5. The skill and its resource files will be imported automatically

### Claude Code (CLI)

Claude Code reads skills from a `.claude/skills/` directory. You can install at the project level or globally.

#### Mac / Linux

**Project-level** (available only in one project):

```bash
mkdir -p /path/to/your/project/.claude/skills/create-research-prompt/resources
cp SKILL.md /path/to/your/project/.claude/skills/create-research-prompt/
cp resources/*.md /path/to/your/project/.claude/skills/create-research-prompt/resources/
```

**Global** (available in all projects):

```bash
mkdir -p ~/.claude/skills/create-research-prompt/resources
cp SKILL.md ~/.claude/skills/create-research-prompt/
cp resources/*.md ~/.claude/skills/create-research-prompt/resources/
```

#### Windows (PowerShell)

**Project-level:**

```powershell
New-Item -ItemType Directory -Force -Path "C:\path\to\your\project\.claude\skills\create-research-prompt\resources"
Copy-Item "SKILL.md" -Destination "C:\path\to\your\project\.claude\skills\create-research-prompt\"
Copy-Item "resources\*.md" -Destination "C:\path\to\your\project\.claude\skills\create-research-prompt\resources\"
```

**Global:**

```powershell
New-Item -ItemType Directory -Force -Path "$env:USERPROFILE\.claude\skills\create-research-prompt\resources"
Copy-Item "SKILL.md" -Destination "$env:USERPROFILE\.claude\skills\create-research-prompt\"
Copy-Item "resources\*.md" -Destination "$env:USERPROFILE\.claude\skills\create-research-prompt\resources\"
```

## Usage

Ask Claude to create a research prompt on any topic:

> "Create a research prompt about migrating our monolith to microservices on AWS"

> "I need a research prompt analyzing the competitive landscape for AI coding assistants"

> "Build me a research prompt for designing a data literacy training program for product managers"

Claude will classify the domain, select the matching template, populate it with your context, and output a ready-to-use prompt in a code block.

## Related Skills

This skill is part of a three-skill workflow:

1. **create-research-prompt** (this repo) — generates the prompt
2. **run-perplexity-deep-research** — executes the prompt via Perplexity
3. **generate-presentation** — turns research output into slide decks

## License

MIT
