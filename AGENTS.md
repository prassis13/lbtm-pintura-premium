# LBTM — Site Pintura Premium

## Identidade do Projeto
Site institucional da **LBTM Serviços** — pintura residencial e comercial de alto padrão em São Paulo. Design vault vindo do Pen Design. Finalização e publicação via OpenCode.

## Arquivos Base
- `lbtm-precision.html` — Mockup conceitual "Precision" (claro, Apple/Airbnb)
- `mq41cbh8-index.html` — Versão "Noir Editorial" (preto + off-white + dourado)
- `mq41cbhb-style.css` — CSS principal com design tokens

## Setup Automático (faça na primeira execução)

1. **Verificar Node.js** — `node --version` e `npm --version`
2. **Instalar UI/UX Pro Max (se ausente):** `npm install -g uipro-cli` + `uipro init --ai opencode`
3. **Instalar Everything OpenCode (se ausente):** `npm install -g everything-opencode` + `everything-opencode install`
4. **Construir graphify:** execute `graphify .` na raiz do projeto
5. **Confirmar skills ativas:** verificar `.opencode/skills/ui-ux-pro-max/SKILL.md`

## Regras de Design (Preservar Obrigatoriamente)

### Design Tokens (do CSS)
- Paleta: `--noir #0A0A0A`, `--cream #F5F2EB`, `--gold #C9A84C`, `--green #1B5E20`
- Serif: Playfair Display / Fraunces (títulos)
- Sans: Inter (corpo)
- Container: 1280px, gutter clamp(20px, 4vw, 48px)
- Easing: cubic-bezier(0.4, 0, 0.2, 1)

### Estilo Visual
- Fundo escuro editorial (noir) com texto em cream
- Dourado fosco como accent (CTA, detalhes)
- Verde LBTM apenas no logo e hairline
- Hierarquia por espaço, não por decoração
- Animações sutis com transparência e transform

## Skills Disponível

| Skill | Como Ativar |
|---|---|
| **graphify** | `/graphify .` constrói, `graphify query "..."` consulta |
| **UI/UX Pro Max** | Ativa automaticamente em tarefas de UI/UX |
| **Get Shit Done (GSD)** | `/gsd-plan-phase`, `/gsd-execute-phase`, `/gsd-discuss-phase` |
| **Everything OpenCode** | `EO-planner`, `EO-designer`, `EO-code-reviewer` (agentes) |
| **agent-browser** | Testar preview local |

## Fluxo de Finalização

1. **Discussão** — Entender qual variação de design usar (Precision vs Noir)
2. **Plano** — Usar `/gsd-plan-phase` para dividir tarefas
3. **UI/UX** — Aplicar UI/UX Pro Max nas decisões de design
4. **Implementação** — Construir seção por seção
5. **Revisão** — Rodar `EO-code-reviewer` e verificar fidelidade visual
6. **Graphify** — Após mudanças, `graphify update .`

## Avisos
- Nunca mudar a paleta de cores definida nos tokens
- Nunca substituir fontes definidas
- Preservar assets da pasta `assets/landing-pintura/`
- Verificar permissões se encontrar erro de instalação
