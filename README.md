# FM Official Studio

Football Manager 27에서 영입·방출이 확정되는 순간, 구단 공식 계정처럼 **오피셜 사진과 포스터**를 만들어 주는 도구예요.

- **인게임 자동 제작:** FM 사이드바에 '오피셜' 메뉴가 생겨요. 우리 팀 이적을 게임 데이터에서 감지해서, 개인 합의 단계에서 사진을 미리 만들어 두고 이적이 확정되면 바로 공개해요. 이적이 무산되면 만들어 둔 사진은 자동으로 버려요.
- **X(트위터) 스타일 구단 게시글:** 구단 로고, 게시글 문구(AI 작성), 게임 속 날짜, 반응 수까지 실제 구단 계정처럼 보여 줘요. 영어 게시글은 한국어 번역 버튼도 있어요.
- **포스터 정보는 게임 데이터 그대로:** 포지션, 나이, 이적료, 주급, 계약 만료 연도
- **앱에서 직접 만들기:** 세이브 파일에서 선수 정보를 불러오거나 직접 입력해서 오피셜 사진과 포스터를 만들 수 있어요.

## 다운로드

[최신 버전 받기 (Releases)](https://github.com/dsgsdfhsdf/FM-Official-Studio/releases/latest)에서 `FM-Official-Studio-Setup-x.y.z.exe`를 받아 실행하세요.

설치하고 나면 새 버전이 나올 때 앱 상단에 **업데이트** 버튼이 떠요. 누르면 내려받고 재시작할 때 자동으로 설치돼요.

## 필요한 것

| 기능 | 필요한 것 |
|---|---|
| 앱 실행, 포스터 만들기 | Windows 10/11 |
| 인게임 자동 제작 | Football Manager 27 (Steam), **BepInEx 6 (IL2CPP용)** |
| AI 오피셜 사진 생성 | **유료 ChatGPT 계정** (Codex로 로그인, 계정의 이미지 생성 한도 사용) |
| 선수 얼굴 | FM 페이스팩 (없으면 사진을 직접 넣을 수 있어요) |
| 세이브에서 선수 불러오기 | 앱의 '기능 설치'에서 원클릭 설치 |

## 설치 방법

1. **BepInEx 설치** (인게임 기능을 쓸 때만)
   [BepInEx 빌드 페이지](https://builds.bepinex.dev/projects/bepinex_be)에서 **BepInEx Unity (IL2CPP) for Windows (x64)** 를 받아 FM27 설치 폴더(`steamapps\common\Football Manager 27`)에 압축을 풀고, FM을 한 번 켰다 꺼 주세요.
2. **FM Official Studio 설치**
   Setup을 실행하면 중간에 **"FM 플러그인 같이 설치"** 체크박스가 나와요. 체크한 채로 설치하면 FM 플러그인까지 같이 들어가요. (FM은 꺼 두세요)
   BepInEx가 없으면 앱만 설치되고, 나중에 앱의 **기능 설치 → 인게임 연동**에서 플러그인을 설치할 수 있어요.
3. **앱 설정**
   앱의 **기능 설치**에서 AI 사진 생성(Codex)을 설치하고 ChatGPT로 로그인한 뒤, **인게임 설정**에서 자동 제작 옵션을 고르세요.
4. FM을 켜면 앱이 함께 켜지고(트레이), 사이드바에 **오피셜** 메뉴가 생겨요.

### "Windows의 PC 보호" 창이 떠요

코드 서명이 없는 개인 제작 프로그램이라 처음 실행할 때 Windows SmartScreen 경고가 나올 수 있어요. **추가 정보 → 실행**을 누르면 설치돼요.

## 알아 두세요

- AI 사진을 만들 때 선수 얼굴 사진, 구단 유니폼, 로고가 OpenAI로 전송되고, 본인 ChatGPT 계정의 이미지 생성 한도를 써요.
- 게임 데이터를 직접 읽는 방식이라 **FM 업데이트(패치) 후 일부 기능이 잠시 동작하지 않을 수 있어요.** 확인되는 대로 업데이트로 고쳐요.
- 한국어 FM에서 테스트했어요. 다른 언어로 FM을 하면 일부 정보가 다르게 보일 수 있어요.
- 만든 오피셜 포스터는 기본으로 `문서\FM Official Studio`에 저장돼요. (인게임 설정에서 바꿀 수 있어요)

## 제거

Windows **설정 → 앱**에서 FM Official Studio를 제거하세요. FM 플러그인은 FM27 폴더의 `BepInEx\plugins\FMOfficial` 폴더를 지우면 돼요.

---

Football Manager는 Sports Interactive와 SEGA의 상표예요. 이 프로젝트는 Sports Interactive, SEGA, OpenAI와 관계없는 개인 팬 제작 도구예요.
