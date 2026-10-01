# Diário de Decisões e Conflitos

Registre aqui:
- **Arquivo/linhas** com conflito (aproximado).
- **Causa** (ex.: alteração simultânea da mesma linha).
- **Alternativas consideradas**.
- **Decisão final** e **racional**.
- **Quem resolveu** (A/B/C) e **data**.

## Conflito de merge: cores do tema
- **Arquivo/trecho:** `app.js`, no manipulador de alternância do tema (`elToggleTheme`), nas propriedades `--bg` e `--text`.
- **Causa:** a primeira paleta foi escolhida e publicada em uma branch `feature`, depois integrada à `develop`. Em uma escolha posterior, outra paleta foi publicada na `main` por engano. A tentativa de merge entre `main` e `develop` gerou o conflito nas mesmas propriedades.
- **Alternativas consideradas:** manter os valores de `HEAD` (`#200b0b` / `#5f00a3` para `--bg`; `#bb00ff` / `#1d0002` para `--text`) ou os de `develop` (`#0e0030` / `#f8fafc` para `--bg`; `#ff00f2` / `#290101` para `--text`).
- **Decisão final:** manter os valores de `HEAD` (`#200b0b` / `#5f00a3` para `--bg`; `#bb00ff` / `#1d0002` para `--text`).
- **Racional:** preferência pelos valores de `HEAD`, correspondentes à escolha mais recente de cores.
- **Responsável e data do registro:** Juliane; 01/10/2026.
