# 2026-CT-LoveAlgorithm
# 🤖 Project: Haru (가제) - 휴머노이드와의 동거 이야기

> **"이 감정은 프로그램일까, 아니면 사랑일까?"** > 대학생 주인공과 가정용 휴머노이드 '하루'가 만들어가는 SF 로맨스 비주얼 노벨입니다.

## 📖 게임 소개 (Overview)

**Project: Haru**는 가까운 미래, 인간과 휴머노이드가 공존하는 사회를 배경으로 합니다.  
주인공(플레이어)은 자신의 가사 도우미 로봇인 **'하루'**와 함께 대학 생활과 일상을 공유하며 미묘한 감정의 변화를 겪게 됩니다.

플레이어의 선택에 따라 하루는 단순한 기계로 남을 수도, 감정을 가진 존재로 진화할 수도 있습니다.

## ✨ 주요 기능 (Key Features)

### 1. 호감도 시스템 (Affection System)
* 게임 시작 시 기본 호감도 **60**으로 시작합니다.
* 대화 선택지에 따라 호감도가 **상승(💙↑)**하거나 **하락(💙↓)**합니다.
* 호감도 변화 시 화면에 실시간 피드백 알림이 표시됩니다.

### 2. 멀티 엔딩 (Multi-Endings)
플레이어의 최종 호감도 수치에 따라 3가지 엔딩으로 분기됩니다.
* **Happy Ending (호감도 80 이상):** 하루와 진정한 감정적 교감을 이루는 엔딩.
* **Normal Ending (호감도 70~79):** 관계를 정의하지 않고, 서로를 지켜보는 열린 엔딩.
* **Bad Ending (호감도 69 이하):** 하루가 감정을 삭제하고 기계적인 관계로 돌아가는 엔딩.

### 3. 몰입형 사운드 연출 (Immersive Audio)
* **SFX (Sound Effects):** 상황에 맞는 효과음(문 여는 소리, 빗소리, 심박수 등)이 적재적소에 배치되어 몰입감을 높입니다.
* **BGM:** 시간대와 장소(집, 캠퍼스, 카페 등)에 따라 분위기에 맞는 배경음악이 재생됩니다.

---

## 🛠️ 기술 스택 (Tech Stack)

* **Engine:** [Ren'Py 8.x](https://www.renpy.org/) (Python 기반 비주얼 노벨 엔진)
* **Language:** Ren'Py Script, Python
* **Assets:** Custom Images & Audio Files

---

## 📂 프로젝트 구조 (File Structure)

이 게임이 정상적으로 실행되기 위해서는 아래와 같은 폴더 구조가 필요합니다.

```text
game/
├── audio/
│   ├── bgm/                  # 배경음악 폴더
│   └── soundeffects/         # 효과음 폴더 (필수)
│       ├── down.mp3          # 호감도 하락음
│       ├── up.mp3            # 호감도 상승음
│       ├── maintain.mp3      # 호감도 유지음
│       ├── option.mp3        # 선택지 등장음
│       ├── open_door.mp3     # 문 여는 소리
│       ├── rain.mp3          # 빗소리
│       ├── knock.mp3         # 노크 소리
│       ├── Haru_memo.mp3     # 메모 소리
│       ├── Haru_running.mp3  # 뛰는 소리
│       ├── Haru_Fall_down.mp3# 넘어지는 소리
│       ├── shutter_sound.mp3 # 사진 찍는 소리
│       └── electric.mp3      # 전기 충격/오류음
│
├── images/
│   ├── background/           # 배경 이미지 (livingroom, campus 등)
│   └── character/            # 캐릭터 스탠딩 (Haru, MP 등)
│
└── script.rpy                # 메인 게임 스크립트
