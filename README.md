# TridiAudience — fonte oficial

Este repositório é a nova fonte de verdade do **TridiAudience**.

## Princípio do projeto

O desenvolvimento passa a separar explicitamente três coisas:

1. **Golden baseline** — comportamento já validado fisicamente e que não pode ser alterado sem teste comparativo.
2. **Recovered source** — código recuperado de branches/artefatos históricos, preservado com proveniência.
3. **Development** — mudanças novas, sempre versionadas e comparáveis contra a baseline.

## Golden behavior inicial

A baseline funcional escolhida para a linha vertical é a **v1.22.0 GazeNet + Radar 3D**, porque existe artefato auditado e feedback físico positivo de que ela contava quem realmente olhava para a tela.

Golden baselines históricas adicionais:
- v1.14.3 — arquitetura antiga completa/fluida, mas com falso positivo de impressão.
- v1.14.7 — EMEET estável e conservadora, porém rígida.
- v1.20.2 — vertical promissora, ainda com falsos positivos laterais.
- v1.22.0 — baseline neural validada para impressão verdadeira.

A v1.22.2 **não** é tratada como baseline de qualidade apesar das otimizações de velocidade.

## Hardware-alvo inicial

- BTV B11
- Android 9 / API 28
- ARMv7 / armeabi-v7a
- ~2 GB RAM
- câmera EMEET SmartCam S600
- execução local com NCNN/CPU/NEON

## Objetivo

Chegar a um APK reproduzível a partir do repositório, preservar o comportamento validado da v1.22.0 e, só então, evoluir precisão, fluidez, gênero, evidências de impressão, servidor e telemetria sem regressões silenciosas.

Veja `docs/ARCHITECTURE.md`, `docs/BASELINES.md` e `docs/ROADMAP.md` quando a fundação estiver importada.
