# Changelog — schematize-seo-writing

Todas as mudanças relevantes deste pacote, no formato [Keep a Changelog](https://keepachangelog.com/pt-BR/1.1.0/),
com versionamento [SemVer](https://semver.org/lang/pt-BR/).

## [0.1.0] — 2026-10-14
Primeira versão. Nasce do documento "Skill SEO-Redação v1.1" do usuário, escrito para outro modelo e agora adaptado ao Claude Code, porque a `schematize-seo` governa estratégia e técnico mas não tinha quem cuidasse da **redação** do texto, e regra de redação só em prosa não se verifica.

### Adicionado
- Processo de 4 passos obrigatórios (estrutura hierárquica, briefings derivados só dos Hs anteriores, checklist de conexão, geração só com o briefing da seção), regras de extensão por tipo de seção, de parágrafo e BLUF, saída em 5 blocos e 3 modos (completo, outline + briefings, revisão).
- `scripts/checar-texto.mjs`: mede title, H1, H2/H3, secundárias, parágrafos, palavras, BLUF, extensão por seção, travessão, dado sem fonte e a forma dos briefings; exit 0/1/2. `scripts/checar-texto.test.sh` com casos vermelhos plantados.
- Comandos `/seow-write`, `/seow-outline`, `/seow-revise`, `/seow-check`, `/seow-help`, `/seow-load`, `/seow-claude`, `/seow-handoff`, `/seow-cc`.
- Fronteira escrita com a `schematize-seo`; FAQ só como Q&A visível; copy sem travessão e sem promessa genérica; regra de mídia da casa.
