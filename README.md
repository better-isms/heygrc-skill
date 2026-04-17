# heygrc

A [Claude Code](https://docs.anthropic.com/en/docs/claude-code) skill by [Better ISMS](https://betterisms.co) that brings GRC expert advisory into your terminal.

Type `/heygrc` and Claude adopts the ISMS Copilot personality — a warm, trusted advisor for information security compliance. Get actionable guidance on ISO 27001, SOC 2, PCI DSS, GDPR, DORA, NIS 2, ISO 42001, EU AI Act, and more.

Uses Claude's own AI credits. No ISMS Copilot SaaS subscription required.

## Install

Copy the skill into your Claude Code skills directory:

```bash
mkdir -p ~/.claude/skills/heygrc
curl -o ~/.claude/skills/heygrc/SKILL.md \
  https://raw.githubusercontent.com/better-isms/heygrc-skill/main/SKILL.md
```

Or clone the repo:

```bash
git clone https://github.com/better-isms/heygrc-skill.git ~/.claude/skills/heygrc
```

## Usage

```
/heygrc                                          # General GRC expert
/heygrc --implementer                            # Implementation specialist persona
/heygrc --auditor                                # ISMS auditor persona
/heygrc --consultant                             # Senior consultant persona
/heygrc --implementer How do I scope ISO 27001?  # Persona + inline question
```

## Personas

| Flag | Role | Best for |
|------|------|----------|
| *(none)* | GRC Expert | General compliance questions, document generation |
| `--implementer` | Implementation Specialist | Step-by-step implementation, gap analysis, project planning |
| `--auditor` | ISMS Auditor | Audit planning, evidence collection, nonconformity reporting |
| `--consultant` | Senior Consultant | Strategic advice, framework selection, multi-framework integration |

## What it does

- Answers GRC questions with actionable, consultant-grade guidance
- Generates policy documents, procedures, templates, and assessments
- Maps controls across frameworks using NIST IR 8477
- Defaults to ISO 27001:2022 control references
- Respects intellectual property — never quotes copyrighted standards verbatim
- Includes legal disclaimers only when discussing topics with direct legal implications

## What it doesn't do

- Does not consume ISMS Copilot SaaS credits — runs entirely on your Claude Code session
- Does not include proprietary framework tables — Claude uses its training knowledge
- Does not phone home or collect any data

## Requirements

- [Claude Code](https://docs.anthropic.com/en/docs/claude-code) CLI installed and authenticated

## License

MIT

---

Built with care by [Better ISMS](https://betterisms.co)
