# LGPD Compliance Advisor

[English](README.md) | **Português (Brasil)**

Skill de agente para análise de **conformidade com a LGPD** (Lei nº 13.709/2018) em software: bases legais, direitos do titular, retenção, terceiros e transferência internacional, logging de PII e minimização.

Monta o inventário de dados e operadores, mapeia fluxos e separa ações de código de ações jurídicas/contratuais. Não substitui assessoria jurídica.

A skill é **somente leitura**: analisa e reporta, sem editar arquivos.

Segue o formato aberto de [Agent Skills](https://agentskills.io) (`SKILL.md` com frontmatter `name` e `description`) e funciona no Claude Code, Cursor e outros agentes compatíveis.

## Instalação

A pasta de destino deve se chamar `lgpd-compliance-advisor` (o nome da skill), não o nome do repositório.

### Claude Code

```bash
# Para todos os projetos
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git ~/.claude/skills/lgpd-compliance-advisor

# Apenas para um projeto
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git .claude/skills/lgpd-compliance-advisor
```

### Cursor

```bash
git clone https://github.com/jrcarls/skill-lgpd-compliance-advisor.git .cursor/skills/lgpd-compliance-advisor
```

## Uso

O agente carrega a skill automaticamente quando a tarefa combina com a descrição. Para chamar explicitamente no Claude Code:

```text
/lgpd-compliance-advisor
```

## Skills relacionadas

Esta skill faz parte de um conjunto que se complementa:

- `skill-owasp-security-reviewer` — OWASP Top 10
- `skill-llm-security-reviewer` — OWASP LLM Top 10
- `skill-tenant-isolation-reviewer` — IDOR / ownership
- `skill-lgpd-compliance-advisor` — conformidade LGPD
- `skill-qa-verifier` — verificação funcional
- `skill-vue-reviewer` — revisão de frontend Vue

## Licença

[MIT](LICENSE)
