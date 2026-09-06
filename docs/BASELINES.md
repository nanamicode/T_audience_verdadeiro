# Baselines do TridiAudience

## Regra
Nenhuma versão mais nova é considerada melhor só porque é mais recente.

### v1.14.3 — golden histórica
Arquitetura antiga funcional e relativamente fluida, mas com falsos positivos de impressão.
APK SHA-256: `cf00c3cbefabdd249f4c105985664f09dc830345e69deed02f0ff5aff0f71c12`.

### v1.14.7 — golden EMEET conservadora
EMEET estável, porém rígida.
APK SHA-256: `eac60c77c6cc1db51df97577abc23c137d90090fd38fe3a9f041f3d6d6e5cebe`.

### v1.20.2 — referência vertical
Melhorou impressões, mas ainda aceitava pessoas de lado.
APK SHA-256: `b68f18fbd9c59b365ab6af0263b68508b1fdaceda0b7e63b779665dd23c0e59e`.

### v1.22.0 — GOLDEN BEHAVIOR atual
GazeNet neural + Radar 3D, ARMv7/NCNN, preservando core estável da v1.20.7.
Foi validada fisicamente como contando quem realmente olhava para a tela.
APK SHA-256: `58224ff8b51ad4b29828e2f78f3a72da76f23e889b0947d00f0918c7417f82a5`.

### v1.22.2 — NÃO golden
Foi otimizada para velocidade, mas rejeitada por qualidade.
