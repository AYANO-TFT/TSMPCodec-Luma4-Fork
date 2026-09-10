# Changelog

## 0.0.3-beta.3

- Provide an SDK-neutral codec prefab for Core's automatic Controller preparation in ordinary Unity and VRChat.
- Detect installed Worlds packages through assembly version defines without requiring VRCSDK through UPM.
- Require Core 0.2.0-beta.1 or newer through VPM; use the exact matching Core version for UPM.
- Preserve Luma4 codec ID, script and material references, shader decoding logic, and wire format.

## 0.0.3-beta.2

- Fix TSMP Core shader includes for local `file:` packages by resolving them through `Packages/com.kibalab.tsmp.core/` (PR #1, contributed by AYANO-TFT).
- Keep shader decoding logic and the encoded data format unchanged.

## 0.0.3-beta.1

- Beta release metadata for VPM distribution.
- Includes the default Luma4 codec runtime, shaders, materials, prefab, and sample.
