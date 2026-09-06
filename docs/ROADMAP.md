# Roadmap

## Fase 0 — preservação
- [x] Repositório fonte de verdade.
- [x] Hashes das baselines.
- [ ] Importar código exato da v1.22.0.
- [ ] Importar source recuperado v1.22.3 separado.

## Fase 1 — build reproduzível
- [ ] Projeto Android/Gradle completo.
- [ ] Core nativo compilado de source.
- [ ] Aquisição/conversão automática dos modelos públicos.
- [ ] APK ARMv7 via GitHub Actions.
- [ ] Checksums e relatório de build.

## Fase 2 — regressão
- [ ] Olhando tela => impressão.
- [ ] Olhando chão/lado/teto => sem impressão.
- [ ] 50 frames ruins + 1 verdadeiro => exatamente 1 impressão.
- [ ] Mesma track nunca conta duas vezes.
- [ ] Benchmark FPS/latência/CPU/RAM.

## Regra
Toda alteração de impressão, tracking, rotação, gênero ou evidência deve ser comparada contra a v1.22.0.
