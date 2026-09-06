# Arquitetura e reconstrução

## Hardware de referência
BTV B11, Android 9/API 28, ARMv7, ~2 GB RAM, EMEET SmartCam S600.

## Pipeline golden v1.22.0
1. Entrada UVC/YUV.
2. Rotação vertical antes da inferência.
3. Core: SCRFD + NanoDet + gênero + tracking.
4. Gaze neural: head pose + landmarks35 + gaze-estimation.
5. Projeção 3D do gaze no plano físico do display.
6. Uma track gera no máximo uma impressão.
7. `NEW_IMPRESSION` só existe no frame vencedor.
8. O JPEG de evidência deve ser o mesmo frame que confirmou a impressão.

## Geometria
Display 320x540 mm; centro relativo à câmera X=-187.3 mm, Y=+70 mm; zona segura X=72 mm, Y=189 mm; profundidade 450–2600 mm; FoV diagonal EMEET 73°.

## Source
`golden/v1.22.0/` preserva código da build validada.
`recovered/v1.22.3/` preservará fontes posteriores úteis à reconstrução, sem tratá-las como golden.
