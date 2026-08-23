# Skills de redecoração

Origem: https://github.com/rtadewald/skills-redecoracao (commit abaixo).

Instaladas neste projeto em `.claude/skills/`. Para ativá-las no nível do usuário
(os scripts se referenciam por caminho absoluto `~/.claude/skills/...`):

```bash
cp -r .claude/skills/{redecoracao,nano-banana-pro,busca-produtos} ~/.claude/skills/
```

## Chaves necessárias (`.env` ou variáveis de ambiente)

| Variável | Para quê | Obrigatória? |
|---|---|---|
| `OPENROUTER_API_KEY` | geração de imagem (provider padrão) | uma das duas |
| `GEMINI_API_KEY` | geração de imagem (alternativa) | uma das duas |
| `SERPAPI_API_KEY` | busca de produtos (onde comprar) | só p/ `busca-produtos` |
| `IMGBB_API_KEY` | upload da imagem na busca | opcional |

Pré-requisito: [`uv`](https://docs.astral.sh/uv/) — os scripts rodam com `uv run`.
