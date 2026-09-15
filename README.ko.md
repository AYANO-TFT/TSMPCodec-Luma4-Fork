**한국어** | [English](README.en.md) | [日本語](README.md)

# TSMP Codec Luma4

Luma4는 TSMP의 기본 코덱입니다. 색상 정보 대신 밝기 단계 중심으로 TSMP 데이터를 기록해, 설정이 단순하고 디코딩 경로가 안정적인 기준 코덱으로 사용됩니다.

처음 TSMP를 설치하거나 문제를 진단할 때는 Luma4를 먼저 사용하는 것을 권장합니다.

## 특징

- TSMP 기본 코덱
- 낮은 색상 의존도와 단순한 디코딩 경로
- VRChat 화면 캡처, OBS/Spout 같은 일반적인 영상 경로에서 테스트하기 쉬운 기준 패턴
- Core 패키지의 `TSMPSetup` Codec 탭에서 자동 검색

## 요구 사항

- TSMP Core: https://github.com/kibalab/TSMP-Core
- Unity 2022.3
- `com.kibalab.tsmp.core` 0.2.0 이상 (UPM 의존성: 0.2.0)
- VRChat 월드에서 사용하는 경우에만 VRChat Worlds SDK 3.9.0 이상 필요

## 설치

VRChat Creator Companion에서 VPM 저장소를 추가합니다.

```text
https://vpm.kiba.red/
```

그 다음 `TSMP Core`와 `TSMP Codec Luma4`를 설치합니다.

일반 Unity에서는 UPM의 **Add package from disk**로 Core 0.2.0과 이 패키지를 설치합니다. VRCSDK/UdonSharp는 필요하지 않습니다. 두 환경 모두 동일한 Controller 프리팹과 자동 설정을 사용합니다.

## 사용 방법

1. Core 패키지의 `Packages/com.kibalab.tsmp.core/Samples/TSMPController.prefab`을 씬에 배치합니다.
2. `TSMPSetup`의 Codec 탭에서 `Refresh Codecs`를 누릅니다.
3. `Luma4`를 선택합니다.
4. 입출력 설정을 확인합니다. 컴포넌트와 바인딩은 자동으로 준비되며, `Apply Setup`으로 수동 갱신할 수도 있습니다.

## 배포 상태

Luma4 0.0.3은 TSMP Core 0.2.0용 정식 릴리즈입니다. 1.0 이전에는 공개 API가 변경될 수 있습니다.

## 라이선스

MIT License. Copyright (c) 2026 KIBA_Labs.
