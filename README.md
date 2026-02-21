# Mateus Iuri Rocha

> `levementesalgado` · também conhecido como `vinberkuko`

Estudante de sistemas, com interesse em matemática e desenvolvimento de
software do zero. Uso **Solaris 11 (64-bit)** como sistema principal e
trabalho também em **Slackware 15.0** e **Debian**, onde testo diferentes
shells. Cada ferramenta aqui tem um uso definido.

---

## Setup & ferramentas

### Ambiente

| Camada | O que roda |
|--------|-----------|
| SO principal | Solaris 11 (64-bit) |
| Estação diária | Slackware 15.0 (x86_64, KDE Plasma) |
| Partição irmã | Debian (home compartilhado via bind mount) |
| Terminal | Konsole + Yakuake (dropdown) |
| File managers | Dolphin (GUI) e Midnight Commander (`mc`) no TTY |
| Editores | nano, Vim e Geany |
| Browser | Firefox |

### Shells

Cada shell tem uma função específica:

| Shell | Versão | Uso específico |
|-------|--------|----------------|
| **nushell** (`nu`) | 0.115.0 | Gerenciamento de arquivos: navegação estruturada, pipelines tipados e saída tabular. |
| **ksh93** (`ksh`) | 93u+m/1.0.0-beta.2 (David Korn) | Scripts de longa duração e processamento de volumes grandes; POSIX estável e builtins robustos. |
| **bash** | 5.3.15 | Desenvolvimento de sistemas operacionais (TipOS): `make kernel && make iso`, boot no QEMU e uso geral. |
| **zsh** | 5.9.2 | Uso interativo, com prompt próprio (`%n@%m:%~%#`) e `compinit` completo. |
| **fish** | 4.8.1 | Alternativa interativa com autocomplete já configurado. |
| **tcsh / csh** | — | Compatibilidade e scripts legados. |
| **dash / ash** | — | Scripts enxutos e portáveis. |

No Debian mantenho o mesmo conjunto: `bash`, `ksh`/`ksh93`, `sh`, `dash` —
e o `~/.bashrc` compartilhado centraliza o toolchain de OS dev (Zig 0.16,
Deno, Cargo/Rust) nos dois lados.

### Linguagens

| Linguagem | Versão | Papel |
|-----------|--------|-------|
| **Ruby** | 3.0.3 | Linguagem principal para scripting, automações e protótipos. |
| **Rust** | (via Cargo) | Sistemas, motores, kernels e projetos recentes. |
| **C** | — | Sistemas operacionais (Ovsb.OS) e código de baixo nível. |
| **K** (kdb+) | ngn/k | Cálculo para atratores, fractais e wavelets. |
| **R** | — | Estatística e classificação (mycelium). |
| **Java** | 21 (Temurin) | Atividades acadêmicas e backend. |
| **PHP** | — | Desenvolvimento web. |
| **Assembly** | — | Código de baixo nível quando necessário. |
| **Shell** | a coleção acima | Integração entre ferramentas. |
| **Python** | — | Uso limitado; prefiro Ruby para esse tipo de serviço. |

### Editores / IDE

| Editor | Quando uso |
|--------|-----------|
| **nano** | Edição rápida de qualquer arquivo. |
| **Vim** | Edição em TTY e sessões remotas. |
| **Geany** | Ambiente leve para aulas e compilações simples. |

Testei **VSCodium**, mas o consumo de memória (cerca de **1 GB**) não
compensa para o meu uso. Fico com nano, Vim e Geany.

---

## Projetos em destaque

### Sistemas & linguagens

- **[Ovsb.OS](https://github.com/levementesalgado/Ovsb.OS)** /
  **[OvsbMkM](https://github.com/levementesalgado/OvsbMkM)**
  SO 64-bit do zero em C: kernel próprio, VESA, TinyWM, FAT32 e uma toolkit
  de widgets (OWT) nativa.

- **[MizuOS](https://github.com/levementesalgado/MizuOS)** /
  **[Hako](https://github.com/levementesalgado/Hako)**
  Kernel i686 bare-metal em Rust + assembly, com o Hako — uma DSL que
  descreve boxes/flows e transpila drivers para Rust com menos tokens.

### Matemática & IA

- **[aquario-matematico](https://github.com/levementesalgado/aquario-matematico)**
  Simulações matemáticas numa janela — atratores caóticos, fractais, cardumes
  e filotaxia. Rust + SDL2 na frente, K gerando a matemática pesada.

- **[mycelium](https://github.com/levementesalgado/mycelium)**
  Pipeline Rust + R para ler sinais elétricos de micélio e classificar com
  Reservoir Computing + CNN. Agricultura de precisão via fungos micorrízicos.

- **[amadeus](https://github.com/levementesalgado/amadeus)**
  Motor de inferência 100% Rust, CPU-only, carregando modelos GGUF reais e
  uma gramática tabular experimental (AMADEUS-M).

- **[ondina](https://github.com/levementesalgado/ondina)**
  Previsão de cripto com wavelets em ngn/k, CNN 1D e aprendizado online.
  Projeto de pesquisa em construção (Fase 0).

### Agro & dados

- **[SISPEC](https://github.com/levementesalgado/SISPEC)**
  Sistema Inteligente de Pecuária de Confinamento: Rust + Deno + React,
  ML para predição de peso, anomalias e projeção de abate. Sem Python.

- **[santo-graal](https://github.com/levementesalgado/santo-graal)**
  Análises automáticas dos dados oficiais da CONAB.

- **[interagro-2026](https://github.com/levementesalgado/interagro-2026)**
  Site estático do evento de inovação no agronegócio (FATEC Capão Bonito).

- **[psa-araucaria](https://github.com/levementesalgado/psa-araucaria)** /
  **[survey-cps](https://github.com/levementesalgado/survey-cps)**
  Gestão do PSA Araucária: backend NestJS + PostGIS e app Android em Kotlin,
  mais o cadastro de campo via Survey123/ArcGIS.

- **[hackathon-alternativas](https://github.com/levementesalgado/hackathon-alternativas)**
  Conjunto de MVPs em Ruby/Sinatra para o agronegócio, com interface de
  produto, dados de exemplo e painel geral.

### Aplicações & web

- **[olympus-bx-micro-manager](https://github.com/levementesalgado/olympus-bx-micro-manager)**
  Adaptador de dispositivo para microscópios Olympus no Micro-Manager 2.0.

- **[chibi-chan](https://github.com/levementesalgado/chibi-chan)**
  Pequeno servidor Rust com personagem 3D e chat/TTS.

- **[EJM](https://github.com/levementesalgado/EJM)**
  Sistema desktop para a empresa júnior da FATEC: Rails API + serviço Rust
  + frontend Qt C++.

- **[frente.social](https://github.com/levementesalgado/frente.social)**
  Site estático de comunicação de base: zero JavaScript, zero rastreamento,
  Caddy servindo HTML.

- **[levemente-salgado](https://github.com/levementesalgado/levemente-salgado)**
  Site pessoal em HTML/CSS puro.

Também há utilitários (**hw-list**, **ScriptWebVideosPC**), material de
aulas (**aulas-banco**, **aula-git-github**, **aprender-vb6**,
**aulasdelogica**) e experimentos pelo caminho. Tudo em
[github.com/levementesalgado](https://github.com/levementesalgado).

---

## Conecte

Interessado em trocar ideias sobre sistemas operacionais, matemática visual
e escolhas de ferramentas.

— Mateus Iuri Rocha
