---
documento: orientação para agentes
audiência: IA (Claude, GPT, outros LLMs ou agentes)
---

# AGENTS.md

Este documento existe para que um agente de IA, ao ser entregue a este repositório sem contexto prévio, consiga compreender a estrutura, a tese, e o estado do trabalho em uma única leitura.

## Tese em uma frase

A natureza já resolveu, sob pressão evolutiva, vários problemas de coordenação multi-agente que a IA contemporânea está tentando resolver. Catalogar essas soluções biológicas é matéria-prima de engenharia, não metáfora.

## Estrutura semântica

```
biomimetica/
├── README.md                ← índice e estado geral
├── AGENTS.md                ← este arquivo
├── 00-tese.md               ← capítulo zero, define o estudo
├── 01-colonia-abelhas.md    ← capítulos por sistema natural
├── 02-formigueiro.md
├── ... (até 09)
├── primitivas/              ← dicionário de tradução
│   ├── coordenacao-sem-coordenador.md
│   ├── stigmergy.md
│   ├── consenso-descentralizado.md
│   └── ...
└── projetos/                ← aplicação em projetos próprios
```

## Cabeçalho YAML obrigatório

Todo arquivo `.md` no repositório começa com bloco YAML. Campos esperados:

- `título` — string
- `capítulo` ou `tipo` — string (capítulo: 01, tipo: primitiva, tipo: projeto, etc)
- `autor` — string

Capítulos de sistema natural adicionam:
- `arquétipo` — nome curto do sistema (ex: "colônia-abelhas")
- `primitivas-envolvidas` — lista de primitivas referenciadas
- `status-mapeamento-ia` — `verde` | `amarelo` | `cinza` | `misto`

## Como interpretar status

- **Verde 🟢** — IA aplicada hoje resolve isso bem. Frameworks maduros, papers consolidados, casos de uso em produção.
- **Amarelo 🟡** — área ativa de pesquisa, soluções parciais, sem consenso. Vale acompanhar.
- **Cinza ⚪** — gap real. A natureza resolveu, IA não tem boa resposta. Território de pesquisa primária.

Capítulos com `status-mapeamento-ia: misto` indicam que o sistema natural cobre primitivas em estágios diferentes — algumas verdes, outras cinzas. O detalhamento fica no corpo do capítulo.

## Convenções de escrita

- Português brasileiro.
- Registro acadêmico-aplicado: rigoroso o suficiente para ser citável, acessível o suficiente para ser lido fora do círculo acadêmico.
- Referências primárias (biologia) e secundárias (IA) separadas em seções distintas.
- Citações no corpo do texto em formato livre; bibliografia consolidada ao final de cada capítulo.
- Quando um capítulo aciona uma primitiva, faz link explícito para o arquivo da primitiva.

## Quando assistir o autor

Se o autor pedir para escrever um capítulo, expandir uma seção, buscar referências, ou revisar um trecho, o agente deve:

1. Ler o capítulo zero (`00-tese.md`) se ainda não tiver lido nesta sessão.
2. Ler o capítulo ou primitiva diretamente envolvido.
3. Manter a voz e o registro estabelecidos.
4. Sinalizar inconsistências ou gaps em vez de inventar conteúdo.

## O que o agente não deve fazer

- Reescrever a tese sem solicitação explícita.
- Adicionar capítulos não previstos no índice sem combinar.
- Inflar a bibliografia com papers não lidos.
- Substituir prosa densa por bullets quando a prosa estiver funcionando.
- Tratar o estudo como produto comercial. Não é.
