# [SFC] 브레스 오브 파이어 한글패치

슈퍼패미콤 **브레스 오브 파이어 -용의 전사-** 한글패치입니다. 슈퍼패미콤 실기에서 구동하는 것을 목표로 작업했습니다.

- 블로그 소개글: https://dwyn.tistory.com/7
- 최신 버전 다운로드: [Releases](../../releases/latest)
- 버그 제보: [Issues → 버그 제보](../../issues/new/choose)
- 후원: https://litt.ly/dwyn

## 작업 사항 및 변경 이력

주요 작업 사항, 추가 기능, 변경 이력 등 자세한 내용은 **[블로그](https://dwyn.tistory.com/7)** 글을 참조해 주세요.

## 적용 방법

1. [Releases](../../releases/latest)에서 패치 파일을 받습니다.
2. 직접 가지고 계신 원본 ROM에 패치를 적용합니다.
   - 웹에서 적용: [ROM Patcher JS](https://www.marcrobledo.com/RomPatcher.js/)
   - PC 프로그램: Delta Patcher, Floating IPS 등
3. 패치된 ROM을 에뮬레이터나 플래시카트로 실행합니다.

### 체크섬 확인

패치는 **헤더 없는 일본판 Rev 1 원본 ROM**(1,572,864바이트)에 적용해야 합니다. 패치 후 ROM은 2,097,152바이트로 커집니다.

| 구분 | CRC32 | MD5 | SHA1 |
|---|---|---|---|
| 원본 ROM (일본판 Rev 1) | `E0B0BBEC` | `A8421D749DA1510DF9A37FED5909E129` | `3AB85EE92F5E2C9069E3D2FA595FAB3D452C5D99` |
| 패치 후 (v1.0, 2,097,152바이트) | `4B0C087F` | `E26AE4F84E980D377D9CFFC6E17CE93C` | `CEF10B57C1D51F57E2E143D7EDE6931C3BDD268B` |

- ROM Patcher JS에 ROM 파일을 넣으면 CRC32, MD5, SHA1이 바로 표시됩니다.
- 크기가 1,573,376바이트인 ROM은 512바이트 헤더가 붙은 파일이니, 헤더를 제거한 뒤 적용해 주세요.

> 이 저장소에는 패치 파일만 있습니다. ROM 파일이나 패치를 적용한 ROM은 배포하지 않으며, 요청에도 응하지 않습니다.
