# test_01
MS 강의 중 스네이크 게임 코드 by html

# 🐍 Snake Game (HTML / CSS / JavaScript — Single File)

이 프로젝트는 **HTML 한 파일 안에 CSS와 JavaScript가 모두 포함된 스네이크 게임**입니다.  
브라우저만 있으면 어디서나 실행할 수 있으며, 설치가 필요 없습니다.

***

## 🎮 게임 특징

*   **HTML 파일 한 개로 완성** (CSS + JS 포함)
*   **키보드 화살표 키**로 플레이
    *   ↑ ↓ ← → : 이동
    *   Space : 일시정지 / 재개
    *   R : 게임 재시작
*   **부드러운 애니메이션**, 고급스러운 UI
*   **로컬 스토리지 기반 최고 점수 저장**
*   점수를 먹을수록 **속도 증가**
*   반응형 HUD 디자인

***

## 🛠 실행 방법

1.  저장소를 다운로드하거나 클론합니다.
2.  프로젝트 폴더 안의 `snake.html` 파일을 실행합니다.
3.  웹 브라우저에서 자동으로 게임이 작동합니다.

예:

```bash
git clone https://github.com/your-repo/snake-game.git
cd snake-game
```

***

## 📂 파일 구조

    📁 project
    │
    └── snake.html   # 게임이 담긴 단일 파일

***

## ⌨ 조작법

| 키     | 기능        |
| ----- | --------- |
| ↑     | 위로 이동     |
| ↓     | 아래로 이동    |
| ←     | 왼쪽 이동     |
| →     | 오른쪽 이동    |
| Space | 일시정지 / 재개 |
| R     | 재시작       |

***

## 🖼 스크린샷 (원하면 추가 가능)

> *원하시면 실제 게임 화면 스크린샷을 추가해 드릴게요!*

***

## 🔧 커스터마이즈 방법

### 🔹 격자 크기 변경

```js
const tileCount = 21;   // → 25 또는 30 등 원하는 숫자로 변경
```

### 🔹 게임 속도 조절

```js
const SPEED_MIN = 6;     // 시작 속도
const SPEED_MAX = 18;    // 최대 속도
const SPEED_STEP = 0.6;  // 먹을 때마다 속도 증가량
```

### 🔹 벽 통과 모드(래핑) 활성화

`update()` 함수에서 벽 충돌 코드를 제거하고 아래로 대체:

```js
newHead.x = (newHead.x + tileCount) % tileCount;
newHead.y = (newHead.y + tileCount) % tileCount;
```

***

## 📜 라이선스

이 프로젝트는 자유롭게 수정하고 사용할 수 있습니다.  
필요하시면 MIT 라이선스 등 별도 라이선스를 추가해 드립니다.

***

