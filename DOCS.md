# 🍀 오늘의 행운 — 디자인 시안 통합 문서

토스 앱인토스 비게임 미니앱 "오늘의 행운"의 모든 디자인 시안과 결정사항 모음.

> 📅 최종 업데이트: 2026-04-30
> 🔗 라이브: https://hena019999-cmd.github.io/clover-mockup/

---

## 1. 프로젝트 개요

### 컨셉
30초 동안 풀숲(또는 흙)에서 세잎클로버 사이에 숨은 **네잎클로버**를 돋보기로 찾는 힐링 미니게임.

### 분류
- **앱인토스 비게임 트랙** (TDS 필수, 라이트모드, 검수 약 2~3개월)
- 사행성 메타포 0 → 검수 안전성 높음

### 사용자 확정 사항
| 항목 | 값 |
|---|---|
| 한 판 시간 | **30초** |
| 컨셉 | **힐링·명상** |
| 일일 무료 도전권 | **3회** (00시 KST 리셋) |
| 디자인 중요도 | **매우 높음** — 디자인 게이트 통과 필요 |

---

## 2. 게임 룰 & 수익 구조

### 게임 흐름
```
[홈] 도전권 N장 / [시작] / [도감]
  ↓ 시작 (도전권 0이면 광고)
[게임] 풀숲/흙 + 30초 카운트다운
  → 돋보기 가운데 = 하이라이트 기점
  → 가장 가까운 클로버가 1.6배 + 흰색 글로우
  → 네잎클로버 탭 → 성공
[성공] 발견 시간 표시
  → [그냥 받기] / [📺 광고 보고 5배]
[실패 / 시간 초과]
  → [📺 광고 보고 30초 더] / [포기하기]
```

### 보상 테이블

| 발견 시간 | 그냥 받기 | 📺 광고 5배 |
|---|---:|---:|
| 0~10초 ⭐⭐⭐ | 5원 | **25원** |
| 10~20초 ⭐⭐ | 3원 | **15원** |
| 20~30초 ⭐ | 2원 | **10원** |
| 광고로 추가 시간 후 | 1원 | **5원** |
| 시간 초과 / 포기 | 1원 | — |

### 수익화 위치
| # | 시점 | 광고 종류 |
|---|---|---|
| ① | 도전권 0일 때 충전 | 보상형 |
| ② | 시간 초과 후 30초 추가 | 보상형 |
| ③ | 보상 5배 받기 | 보상형 (95%+ 시청률) |
| ④ | 도감/특별 테마 잠금 해제 | 보상형 (Phase 2) |

판당 평균 광고 노출 1.5~3회. 보상 평균 ~12원 → **판당 +3~7원 마진**

---

## 3. 디자인 시안 — 메인 4종 (v1~v4)

각 4가지 **분위기**에 대한 시안. 처음에 만든 무드보드 + 화면 구성.

| # | 이름 | 특징 | URL |
|---|---|---|---|
| **v1** | 미니멀 평면 SVG | 깔끔, 모던, 토스 기본 톤 | [home](https://hena019999-cmd.github.io/clover-mockup/home.html) · [game](https://hena019999-cmd.github.io/clover-mockup/game.html) · [result](https://hena019999-cmd.github.io/clover-mockup/result.html) · [moodboard](https://hena019999-cmd.github.io/clover-mockup/moodboard.html) |
| **v2** | 다크 밤 정원 | 별·반딧불, 신비·명상 | [home](https://hena019999-cmd.github.io/clover-mockup/variants/night/home.html) · [game](https://hena019999-cmd.github.io/clover-mockup/variants/night/game.html) |
| **v3** | 보태니컬 일러스트 | 디테일 잎맥, 깊이감, 손그림 | [home](https://hena019999-cmd.github.io/clover-mockup/variants/realistic/home.html) · [game](https://hena019999-cmd.github.io/clover-mockup/variants/realistic/game.html) |
| **v4** | 사진 합성 | Unsplash 실사 사진, 압도적 몰입감 | [home](https://hena019999-cmd.github.io/clover-mockup/variants/photo/home.html) · [game](https://hena019999-cmd.github.io/clover-mockup/variants/photo/game.html) |

**🔵 채택**: v1 미니멀 평면 SVG (메인 베이스)

---

## 4. 클로버 모양 시안 (V1~V7)

[비교 페이지 →](https://hena019999-cmd.github.io/clover-mockup/clover-shapes.html)

| # | 이름 | 특징 |
|---|---|---|
| **V1** | 둥근 하트 + V무늬 | 실제 클로버에 가장 가까움. 외곽선 + V표식 |
| **V2** | 단순 원형 | 잎이 완벽한 원. 카툰풍, 친근 |
| **V3** | 각진 하트 | 날카로운 직선 윤곽. 그래픽 아이콘 |
| **V4** | 물방울 잎 | 뾰족한 끝, 통통한 몸. 풀잎 같은 |
| **V5** | 가운데 모인 하트 | 잎이 가운데에 거의 붙어있음 |
| **V6** | 미니멀 평면 | 외곽선·표식 없는 단색 |
| **V7** | V1 외곽선 X | V1에서 외곽선만 제거. 부드럽고 자연스러움 |

**🔵 채택 (현재)**:
- `play.html`: **V7** (둥근 하트 + V무늬, 외곽선 X)
- `play-real.html`: **V5** (가운데 모인 하트 + V무늬)

### 클로버 SVG 사양
```js
// V1/V7 path (둥근 하트, 깊은 노치)
const PATH_V1 = "M 0 -2 C -3 -3 -8 -5 -10 -9 C -12 -13 -10 -17 -6 -17
                 C -3 -17 -1 -15 0 -12 C 1 -15 3 -17 6 -17
                 C 10 -17 12 -13 10 -9 C 8 -5 3 -3 0 -2 Z";

// V5 path (가운데 모인)
const PATH_V5 = "M 0 0 C -4 -2 -10 -6 -10 -12 C -10 -16 -6 -18 -2 -16
                 C 0 -14 0 -10 0 -8 C 0 -10 0 -14 2 -16
                 C 6 -18 10 -16 10 -12 C 10 -6 4 -2 0 0 Z";

// V무늬 (옅은 chevron)
const V_MARK = `<path d="M -4.5 -10 Q 0 -8 4.5 -10"
                stroke="${lighter(c)}" stroke-width="0.9"
                fill="none" opacity="0.65" stroke-linecap="round"/>`;

// 3D 라디얼 그라디언트 (cx 0.35, cy 0.35, r 0.9)
// 0% 밝은 / 60% 메인 / 100% 어두운
```

### 잎 구성
- **3-leaf**: 0°, 120°, -120° (중앙에서 균등) + 곡선 stem 아래로
- **4-leaf**: 0°, 90°, 180°, -90° + 곡선 stem 아래로

---

## 5. 풀숲 시안 (F1~F7)

[비교 페이지 →](https://hena019999-cmd.github.io/clover-mockup/fields.html)

### 잔디 + 클로버 조합 (F1~F4)
| # | 이름 | 비율 |
|---|---|---|
| F1 | 잔디밭 — 풀 압도 | 풀 90 / 클로버 75 |
| F2 | 클로버 정원 — 클로버 풍성 | 풀 35 / 클로버 220 |
| F3 | 야생 들판 — 균형 | 풀 70+묶음 22 / 클로버 130 |
| F4 | 단순 정원 — 깔끔 | 풀 20 / 클로버 90 (큼) |

### 진짜 잔디밭 컨셉 (F5~F7) — `field-real.html` (덮어쓰여짐)
| # | 이름 | 비율 |
|---|---|---|
| F5 | 잔디밭 클래식 | 220 뒤풀 + 70 앞풀 + 60 클로버 |
| F6 | 봄 잔디 + 황금톤 | 200 뒤풀 + 60 앞풀 + 70 클로버 |
| F7 | 무성한 야생 | 280 뒤풀 + 110 앞풀 + 50 클로버 |

> ⚠️ field-real.html은 이후 레퍼런스 스타일(빽빽한 클로버 밭)로 덮어쓰여짐

### 레퍼런스 스타일 (Game24 따라함)
- 풀잎 없이 클로버만 화면 가득
- [field-real.html](https://hena019999-cmd.github.io/clover-mockup/field-real.html)

**🔵 채택**: 레퍼런스 스타일 + F6 분위기 + 흙 배경 (혼합)

---

## 6. 색상 시안 14가지 (C1~C14)

[비교 페이지 →](https://hena019999-cmd.github.io/clover-mockup/colors.html)

### 잔디 컨셉 (C1~C10)
| # | 이름 | 키 컬러 |
|---|---|---|
| C1 | 연한 라임 | `#90C870` 라임 그린 |
| C2 | 봄 새싹 | `#85C25A` 신선한 새싹 |
| C3 | 여름 잔디 | `#5E9B38` 활기찬 풀 |
| C4 | 아침 안개 | `#92B074` 회녹색 |
| C5 | 황금 햇살 | `#88B855` + 골드 패치 |
| C6 | 신선한 숲 | `#6BA078` 청록 |
| C7 | 클래식 모스 | `#7AAB58` 무난한 모스 |
| C8 | 연한 올리브 | `#9AA850` 황록색 |
| C9 | 이끼 그린 | `#6EA050` 밝은 이끼 |
| C10 | 파스텔 수채화 | `#A0BD85` 파스텔 |

### 흙 컨셉 (C11~C14) — 갈색 배경 + 그린 클로버
| # | 이름 | 키 컬러 |
|---|---|---|
| **C11** | 햇살 흙 | 갈색 #C29766 + 라임 #88C25A |
| C12 | 진한 흙 | 진흙 #735542 + 그린 #7AB85A |
| C13 | 모래밭 | 베이지 #DAC094 + 그린 #5E9038 |
| C14 | 가을 낙엽 | 갈색·황색 + 그린 #7BAA50 |

**🔵 채택 (현재)**: `play-real.html` = **C11 햇살 흙**

---

## 7. 인터랙션 / 게임 메커니즘 변천사

### 시도된 방식들
1. **블러 + 돋보기 확대** — 풀숲 흐릿, 돋보기 안만 또렷 → 폐기
2. **빽빽함 + 돋보기 확대** — 작은 클로버 빽빽, 돋보기 2.5배 확대 → 폐기
3. **돋보기 영역만 확대 + 배경 hole** — 마스크로 cleanup → 폐기
4. **🔵 채택**: 호버-하이라이트
   - 돋보기 가운데 = 기점
   - 가장 가까운 클로버 1.6배 + 흰색 글로우
   - 탭 = 발견

### 클로버 배치 변천사
1. 무작위 산포 (260~380개) → 겹침 많음
2. 격자 + jitter (9×14, 11×17, 14×22) → 깔끔
3. 🔵 **채택**: 10×15 = 150개 (현재 play-real.html)

---

## 8. 현재 적용 상태

### `play.html` (기존 — 돋보기 확대 방식)
- v1 미니멀 평면 SVG 베이스
- V7 클로버 모양 (둥근 하트 + V무늬, 외곽선 X)
- 클래식 모스 그린 배경
- 9×14 = 126개 클로버
- 돋보기 마스크 확대 인터랙션
- 🔗 https://hena019999-cmd.github.io/clover-mockup/play.html

### `play-real.html` (신규 — 레퍼런스 스타일) ✅ 메인
- v1 미니멀 평면 SVG 베이스
- V5 클로버 모양 (가운데 모인 하트 + V무늬, 외곽선)
- C11 햇살 흙 배경 (갈색 + 라임 클로버)
- 10×15 = **150개 클로버** (격자 + jitter)
- 돋보기 호버-하이라이트 인터랙션
- 🔗 https://hena019999-cmd.github.io/clover-mockup/play-real.html

### 게임 로직 (양쪽 동일)
- 30초 타이머
- 도전권 시스템 (3장 + 광고 충전)
- 결과 모달 (그냥 받기 / 광고 5배)
- 시간 초과 모달 (광고 30초 추가 / 포기)
- 도감 (발견한 4잎 일자별 기록)
- localStorage 저장
- **광고 시뮬은 현재 비활성화** (테스트 편의용 — 즉시 보상)

---

## 9. 미해결 결정 사항

- [ ] 정식 앱 이름 ("오늘의 행운" 가칭 유지 중)
- [ ] 디자인 무드 최종 확정 (잔디 vs 흙 — 현재 C11 흙으로 시도 중)
- [ ] 사운드 포함 여부 (배경 ASMR, 발견 효과음)
- [ ] 토스 포인트 정산 방식 (`getAnonymousKey` + `executePromotion` API)
- [ ] 검수 통과 후 토스페이 결제 추가 여부 (Phase 3)

---

## 10. 다음 단계

1. **디자인 최종 확정** — play-real.html 또는 play.html 중 선택
2. **광고 시뮬 → 실 SDK** (`useInAppAds` 훅, 머니몽에서 복사)
3. **앱인토스 정식 스캐폴드** (`@toss/tds-mobile` + `@toss/tds-mobile-ait`)
4. **콘솔 등록 + 검수 신청** (예상 2~3개월)
5. **Phase 2 콘텐츠** — 계절 테마, 도감 고도화, 친구 공유

---

## 11. 라이브 URL 모음

| 페이지 | 용도 |
|---|---|
| [/](https://hena019999-cmd.github.io/clover-mockup/) | 인덱스 (전체 시안 진입) |
| [play.html](https://hena019999-cmd.github.io/clover-mockup/play.html) | 게임 (돋보기 확대 방식) |
| [play-real.html](https://hena019999-cmd.github.io/clover-mockup/play-real.html) | **게임 (레퍼런스 스타일, 메인)** |
| [moodboard.html](https://hena019999-cmd.github.io/clover-mockup/moodboard.html) | v1 무드보드 |
| [home.html](https://hena019999-cmd.github.io/clover-mockup/home.html) | v1 홈 화면 |
| [game.html](https://hena019999-cmd.github.io/clover-mockup/game.html) | v1 게임 화면 |
| [result.html](https://hena019999-cmd.github.io/clover-mockup/result.html) | v1 결과 시트 |
| [clover-shapes.html](https://hena019999-cmd.github.io/clover-mockup/clover-shapes.html) | 클로버 모양 7개 비교 |
| [fields.html](https://hena019999-cmd.github.io/clover-mockup/fields.html) | 풀숲 시안 4개 비교 |
| [field-real.html](https://hena019999-cmd.github.io/clover-mockup/field-real.html) | 레퍼런스 스타일 풀숲 |
| [colors.html](https://hena019999-cmd.github.io/clover-mockup/colors.html) | 색상 시안 14개 비교 |
| [variants/night/home.html](https://hena019999-cmd.github.io/clover-mockup/variants/night/home.html) | v2 밤 정원 |
| [variants/realistic/home.html](https://hena019999-cmd.github.io/clover-mockup/variants/realistic/home.html) | v3 보태니컬 |
| [variants/photo/home.html](https://hena019999-cmd.github.io/clover-mockup/variants/photo/home.html) | v4 사진 합성 |
