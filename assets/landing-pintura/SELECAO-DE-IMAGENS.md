# SELEÇÃO DE IMAGENS — LANDING PINTURA LBTM

> **Regras de seleção:**
> 1. Principal = menor numeração encontrada no nome do arquivo.
> 2. Empate em "01": desempate por decisão explícita do Paulo (ou alfabético, na falta de decisão).
> 3. Alternativas = 02, 03, 04... na ordem crescente.
> 4. Sem renomeação. Sem data. Sem escolha por gosto.
> 5. Se a pasta estiver vazia ou a imagem for cross-folder substituta, **avisar** — não inventar.

---

## Hero
Pasta: `assets/landing-pintura/hero/`
Qtd. encontrada: **6**

| Posição | Caminho |
|---|---|
| **Principal (desktop)** | `assets/landing-pintura/hero/hero-principal (1).jpeg` |
| Mobile (decisão Paulo) | `assets/landing-pintura/hero/hero-principal (2).jpeg` |
| Alternativa 1 | `assets/landing-pintura/hero/hero-principal (3).jpeg` |
| Alternativa 2 | `assets/landing-pintura/hero/hero-principal (4).jpeg` |
| Alternativa 3 | `assets/landing-pintura/hero/hero-principal (5).jpeg` |
| Alternativa 4 | `assets/landing-pintura/hero/hero-principal (6).jpeg` |

> Regra 1ª = desktop, 2ª = mobile (decisão do Paulo). Todas as 6 estão numeradas. Nenhuma sem numeração.

---

## Acabamento
Pasta: `assets/landing-pintura/acabamento/`
Qtd. encontrada: **4** (alterada — antes eram 3)

| Posição | Caminho |
|---|---|
| **Principal** | `assets/landing-pintura/acabamento/Luxury_living_room_interior_design_202606052221_2.jpeg` |
| Alternativa 1 | `assets/landing-pintura/acabamento/Luxury_living_room_interior_design_202606052221_3.jpeg` |
| Alternativa 2 | `assets/landing-pintura/acabamento/Luxury_residential_interior_São_…_202606052221_3.jpeg` |
| Alternativa 3 | `assets/landing-pintura/acabamento/Luxury_residential_interior_São_…_202606052221.jpeg` (sem sufixo numérico) |

> ⚠️ **Inconsistências detectadas nesta pasta:**
> 1. **Numeração quebrada:** nenhum arquivo com sufixo `_1`. A menor numeração encontrada é `_2`. Provavelmente faltou gerar a imagem "01".
> 2. **Dois prefixos diferentes:** `Luxury_living_room…` e `Luxury_residential_interior_São_…` — não são da mesma série.
> 3. **Data no nome do arquivo:** todos contêm timestamp `202606052221` (2026-06-05 22:21). A regra "não usar data" foi respeitada na seleção; a data está apenas no nome do arquivo gerado, sem ter influenciado a escolha.
> 4. **Nome truncado com `…`:** os arquivos `Luxury_residential_interior_São_…` têm reticências no meio do nome (truncamento do gerador ou do sistema).
> 5. **Arquivo sem sufixo numérico:** `Luxury_residential_interior_São_…_202606052221.jpeg` é o único sem `_N` no final — tratado como "alternativa 3" por eliminação.
>
> Os 3 arquivos `antes-depois-XX.webp` que estavam aqui **foram removidos** pelo Paulo (agora estão em `antes-depois/`).
>
> ✅ **APROVAÇÃO PROVISÓRIA DO PAULO (2026-06-05):** as 4 imagens ficam como estão. V2 pode usá-las. A pasta `acabamento/` deve ser **padronizada depois** (regenerar com série única 01–04, mesmo prefixo, sem data no nome, sem truncamento) — mas isso **não bloqueia** a V2.

---

## Equipe
Pasta: `assets/landing-pintura/equipe/`
Qtd. encontrada: **6**
Empate em `01`: `equipe-externa-01.webp` e `equipe-interna-01.webp`. Desempate por decisão anterior do Paulo: a `externa-01` foi realocada para a seção **galpão (comercial/)** até gerar imagem própria. Logo, a principal da equipe é a `interna-01`.

| Posição | Caminho |
|---|---|
| **Principal** | `assets/landing-pintura/equipe/equipe-interna-01.webp` |
| Alternativa 1 | `assets/landing-pintura/equipe/equipe-externa-02.webp` (próxima menor após o 01) |
| Alternativa 2 | `assets/landing-pintura/equipe/equipe-interna-03.webp` |
| Alternativa 3 | `assets/landing-pintura/equipe/equipe-interna-04.webp` |
| Alternativa 4 | `assets/landing-pintura/equipe/equipe-interna-05.webp` |
| (realocada) | `assets/landing-pintura/equipe/equipe-externa-01.webp` — usada como **galpão substituto** em `comercial/`. Não entra como principal da equipe. |

> `equipe-interna-02` não existe (pulada de propósito pelo Paulo — renomeação errada). Não listada.

---

## Fachadas
Pasta: `assets/landing-pintura/fachadas/`
Qtd. encontrada: **2**

| Posição | Caminho |
|---|---|
| **Principal** | `assets/landing-pintura/fachadas/fachada-residencial-01.webp` |
| Alternativa 1 | `assets/landing-pintura/fachadas/fachada-residencial-02.webp` |

---

## Comercial
Pasta: `assets/landing-pintura/comercial/`
Qtd. encontrada: **2**
Empate em `01`: `clinica-01.webp` e `escritorio-01.webp`. Desempate por decisão explícita do Paulo: principal = `clinica-01`.

| Posição | Caminho |
|---|---|
| **Principal (clínica)** | `assets/landing-pintura/comercial/clinica-01.webp` |
| Alternativa 1 (escritório) | `assets/landing-pintura/comercial/escritorio-01.webp` |
| **Galpão (substituta cross-folder)** | `assets/landing-pintura/equipe/equipe-externa-01.webp` |

> Imagem própria de galpão (`galpao-01.webp`) ainda não foi gerada. A V2 deve referenciar `equipe/equipe-externa-01.webp` no slot galpão. Quando a imagem real existir, substituir.

---

## Antes e Depois
Pasta: `assets/landing-pintura/antes-depois/`
Qtd. encontrada: **3** (alterada — antes era 0)

| Posição | Caminho |
|---|---|
| **Principal** | `assets/landing-pintura/antes-depois/antes-depois-01.webp` |
| Alternativa 1 | `assets/landing-pintura/antes-depois/antes-depois-02.webp` |
| Alternativa 2 | `assets/landing-pintura/antes-depois/antes-depois-03.webp` |

> Mudança do Paulo: os 3 arquivos `antes-depois-XX.webp` saíram de `acabamento/` e voltaram para esta pasta. A V2 já pode usar o bloco "antes-e-depois" com imagens reais, sem placeholder.

---

## Leandro
Pasta: `assets/landing-pintura/leandro/`
Qtd. encontrada: **3**

| Posição | Caminho | Conteúdo confirmado |
|---|---|---|
| **Principal** | `assets/landing-pintura/leandro/Leandro 01.jpeg` | homem em pé, terno escuro, braços cruzados, fundo cinza — "em pé em pose" |
| Alternativa 1 | `assets/landing-pintura/leandro/Leandro 02.jpeg` | homem sentado à mesa do escritório, logo LBTM verde ao fundo, plantas arquitetônicas — "sentado na mesa" |
| Alternativa 2 (reserva) | `assets/landing-pintura/leandro/Leandro 03.jpeg` | conteúdo não verificado — guardada como reserva |

> ✅ **Inconsistência de case resolvida pelo Paulo:** o arquivo `Leandro 01.jpeg` agora está com L maiúsculo, igual aos outros. Não há mais mistura de case.

---

# RESUMO DO MAPA

| Pasta | Qtd | Principal | Alternativas | Pendência |
|---|---|---|---|---|
| `hero/` | 6 | `(1)` desktop | `(2)` mobile, `(3)`–`(6)` extras | nenhuma |
| `acabamento/` | 4 | `Luxury_living_room…_2` | 3 imagens `_3` e 1 sem sufixo | ⚠️ aprovação **provisória** — padronizar depois; não bloqueia V2 |
| `equipe/` | 6 | `equipe-interna-01` | `externa-02`, `interna-03`, `interna-04`, `interna-05` | `externa-01` realocada para galpão; `interna-02` inexistente |
| `fachadas/` | 2 | `fachada-residencial-01` | `02` | nenhuma |
| `comercial/` | 2 | `clinica-01` | `escritorio-01` | falta `galpao-01` (substituta = `equipe/equipe-externa-01`) |
| `antes-depois/` | 3 | `antes-depois-01` | `02`, `03` | nenhuma — imagens voltaram para cá |
| `leandro/` | 3 | `Leandro 01.jpeg` | `Leandro 02.jpeg`, `Leandro 03.jpeg` | nenhuma — case corrigido |

**Arquivos sem numeração (sufixo numérico ausente):** 1 — `acabamento/Luxury_residential_interior_São_…_202606052221.jpeg` (sem `_N` no final).
**Pastas vazias:** nenhuma das 3 revisadas (`acabamento/`, `antes-depois/`, `leandro/`).
**Imagens cross-folder (substitutas):** 1 — `comercial/galpão` → `equipe/equipe-externa-01.webp` (não tocada nesta revisão).
**Inconsistências de nome em `acabamento/`:** numeração quebrada (sem `_1`), 2 prefixos diferentes (`Luxury_living_room` e `Luxury_residential`), data no nome, 1 nome truncado com `…`, 1 arquivo sem sufixo numérico. Não renomear.
**Inconsistência de nome em `leandro/`:** RESOLVIDA — todos com L maiúsculo agora.

---

# O QUE NÃO FOI TOCADO

- HTML — não alterado.
- CSS — não alterado.
- V2 — não gerada.
- Nenhuma imagem renomeada ou movida.
- Nenhuma data ou escolha por gosto aplicada.
