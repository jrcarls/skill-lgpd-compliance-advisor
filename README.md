# LGPD Compliance Advisor

**English** | [Português (Brasil)](README.pt-BR.md)

An agent skill that analyzes software compliance with the **LGPD** (Brazil's General Data Protection Law, Law No. 13,709/2018): legal bases, data subject rights, retention, processors and international transfers, PII in logs and data minimization.

It builds the data and processor inventory, maps data flows and separates code actions from legal/contractual actions. It does not replace legal advice.

The skill is **read-only**: it analyzes and reports without editing files.

It follows the open [Agent Skills](https://agentskills.io) format (`SKILL.md` with `name` and `description` frontmatter) and works with Claude Code, Cursor and other compatible agents. The skill instructions are written in Brazilian Portuguese.

## Installation

The target folder must be named `lgpd-compliance-advisor` (the skill name), not the repository name.

### Claude Code

```bash
# All projects
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git ~/.claude/skills/lgpd-compliance-advisor

# A single project
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git .claude/skills/lgpd-compliance-advisor
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git .cursor/skills/lgpd-compliance-advisor
```

## Usage

The agent loads the skill automatically when the task matches its description. To invoke it explicitly in Claude Code:

```text
/lgpd-compliance-advisor
```

## Related skills

This skill is part of a complementary set:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — LGPD compliance
- `skill-qa-verifier` — functional verification
- `skill-vue-reviewer` — Vue frontend review

## License

[MIT](LICENSE)
