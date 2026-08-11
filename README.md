<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.3.0:START -->
## v3.3.0

### 한국어

#### 지원 챔피언

- 애니
- 올라프
- 갈리오
- 트위스티드 페이트
- 신 짜오
- 우르곳
- 르블랑
- 블라디미르
- 피들스틱
- 케일
- 마스터 이
- 알리스타
- 라이즈
- 사이온
- 시비르
- 소라카
- 티모
- 트리스타나
- 워윅
- 누누와 윌럼프
- 미스 포츈
- 애쉬
- 트린다미어
- 잭스
- 모르가나
- 질리언
- 신지드
- 이블린
- 트위치
- 카서스
- 초가스
- 아무무
- 람머스
- 애니비아
- 샤코
- 문도 박사
- 소나
- 카사딘
- 이렐리아
- 잔나
- 갱플랭크
- 코르키
- 카르마
- 타릭
- 베이가
- 트런들
- 스웨인
- 케이틀린
- 블리츠크랭크
- 말파이트
- 카타리나
- 녹턴
- 마오카이
- 레넥톤
- 자르반 4세
- 엘리스
- 오리아나
- 오공
- 브랜드
- 리 신
- 베인
- 럼블
- 카시오페아
- 스카너
- 하이머딩거
- 나서스
- 니달리
- 우디르
- 뽀삐
- 그라가스
- 판테온
- 이즈리얼
- 모데카이저
- 요릭
- 아칼리
- 케넨
- 가렌
- 레오나
- 말자하
- 탈론
- 리븐
- 코그모
- 쉔
- 럭스
- 제라스
- 쉬바나
- 아리
- 그레이브즈
- 피즈
- 볼리베어
- 렝가
- 바루스
- 노틸러스
- 빅토르
- 세주아니
- 피오라
- 직스
- 룰루
- 드레이븐
- 헤카림
- 카직스
- 다리우스
- 제이스
- 리산드라
- 다이애나
- 퀸
- 신드라
- 아우렐리온 솔
- 케인
- 조이
- 자이라
- 카이사
- 세라핀
- 나르
- 자크
- 야스오
- 벨코즈
- 탈리야
- 카밀
- 아크샨
- 벨베스
- 브라움
- 진
- 킨드레드
- 제리
- 징크스
- 탐 켄치
- 브라이어
- 비에고
- 세나
- 루시안
- 제드
- 클레드
- 에코
- 키아나
- 바이
- 아트록스
- 나미
- 아지르
- 유미
- 사미라
- 쓰레쉬
- 일라오이
- 렉사이
- 아이번
- 칼리스타
- 바드
- 라칸
- 자야
- 오른
- 사일러스
- 니코
- 아펠리오스
- 렐
- 파이크
- 벡스
- 요네
- 암베사
- 멜
- 유나라
- 로크
- 세트
- 릴리아
- 그웬
- 레나타 글라스크
- 오로라
- 닐라
- 크산테
- 스몰더
- 밀리오
- 자헨
- 흐웨이
- 나피리

#### 핵심 및 메뉴

- v3.3.0은 실제 사용자 로그에서 확인된 5개 MESH 치명 오류를 원인별로 닫았습니다. 메뉴 color/keybind의 금지된 setter, 원형 예측 speed 누락, 선언되지 않은 상수, Hanbot vec2/vec3 프록시의 벡터 곱을 각각 전수 검사로 고정했습니다.
- 현대 173명·Classic 60명·공용 코어의 237개 `main.lua`에서 자동 논타겟 조준을 전수 감사했습니다. 62개 Lua 경로가 예측 실패 뒤 현재 위치·커서·오래된 경로로 시전하지 않도록 교정됐고, 새 검사는 같은 폴백이 다시 추가되면 릴리즈를 막습니다.
- 아군 Blitzcrank/Thresh/Nautilus/Pyke 같은 끌기·밀치기 중에는 장지연 스킬을 대상의 현재 위치가 아니라 공식 강제이동 도착점에 맞춥니다. 도착점을 증명할 수 없으면 자동 시전하지 않습니다.
- AIO, MGoD Orb, `[MESH]Evade`는 계속 각각 단독으로 동작합니다. AIO는 오직 `meshevade` 공개 facade만 0.5초 제한 재탐색하며 native Evade3나 다른 스크립트를 생성·필수 로드하지 않습니다.
- Zoe는 Kiri의 Q/Q2·벽 E·안전 R·W 파편·수면 평타 억제 교리를 현재 API로 재구성했고, Yone은 HGPro의 Q3 몸 대시/피격선 분리·Q-W-E-R·E 복귀·R 착지 안전·Q3-Flash를 수작업 상태기로 이식했습니다. 보호 loader나 외부 의존성은 포함하지 않았습니다.
- Classic 8개 모듈(Corki, Fiddlesticks, Heimerdinger, Janna, Malphite, Nidalee, Olaf, Pantheon)의 장지연·예측 실패 자동 시전도 같은 실패 폐쇄 계약으로 교정했습니다.
- Lua 5.1, 173 AIO, 60 Classic, 234 메뉴, 233 Farm, 공식 16.15 데이터, 선형 폭, 벡터 연산, 상수, 강제이동, 자동 조준, 위빙 계약을 CI에서 함께 검사합니다. 실제 live 이름·서버 승인·차징 해제 시각은 F12 후속 검증 항목입니다.

#### Aatrox

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.
- 로그의 `number` 대 `struct109` 비교 원인이던 벡터 프록시 곱을 명시적 성분 내적으로 바꾸고 Q 자동 조준을 실패 폐쇄했습니다.

#### Ahri

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Anivia

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Annie

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Aphelios

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Bard

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Belveth

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Cassiopeia

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Corki

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Ekko

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Ezreal

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Gragas

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Hwei

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Illaoi

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Irelia

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Jhin

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.
- W/E가 아군 그랩 대상의 이동 전 위치에 쏘지 않으며, 공식 강제이동 도착점을 얻은 경우에만 그 위치를 우선합니다.

#### Kled

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### KogMaw

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Leona

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Lillia

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Lissandra

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Locke

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Lux

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Malphite

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Malzahar

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Maokai

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Mel

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Milio

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Mordekaiser

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Ornn

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Pantheon

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Poppy

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Pyke

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Rumble

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Senna

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Seraphine

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Shaco

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Shyvana

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Soraka

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Taliyah

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Taric

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Tristana

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Trundle

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Urgot

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Varus

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Veigar

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Velkoz

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Viego

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Viktor

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.
- 벡터 프록시 오류를 제거하고 W/R의 강제이동 도착점 조준 및 실패 시전 억제를 적용해 과도한 연속 요청을 줄였습니다.

#### Xerath

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.
- R 채널 시작과 R2 탄환 상태를 분리해 Combo 키를 누르는 동안 준비된 탄환을 매 틱 안전하게 재시도하며, 예측 실패 시 현재 위치로 쏘지 않습니다.

#### XinZhao

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Zac

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Zed

- 자동 논타겟 스킬이 유효한 예측점·강제이동 도착점·대시 도착점을 얻지 못하면 현재 위치나 커서로 추측해 허공에 시전하지 않고 실패 폐쇄합니다.

#### Chogath

- 원형 Q 예측 입력에 누락되지 않는 즉시형 speed를 보장해 nil 산술 치명 오류를 막았습니다.

#### Sylas

- 선언되지 않은 `Q_DETONATION` 산술을 실제 Q 폭발 지연 상수로 교체하고 상수 전수 검사에 등록했습니다.

#### Yasuo

- Q1/Q2/Q3와 EQ가 유효한 예측·대시 도착점을 얻지 못하면 허공에 시전하지 않도록 상태기와 신뢰도 게이트를 교정했습니다.

#### Yone

- HGPro 교리를 현재 공식 16.15 형태와 결합했습니다: Q3 대시 450/피격선 1050 분리, Q-W-E-R, 안전 E 복귀·처형, R 착지 검증, 2틱 Q3-Flash, 실제 Semi R 우선순위.

#### Zeri

- Farm이 켜진 Lane Clear에서 유효한 미니언 Q와 오브워커가 실제 공격 중인 적 포탑 Q를 모두 지원합니다. 주변 구조물을 임의 탐색하거나 Combo에서 포탑을 고르지 않으며, Q 경로 뒤에만 네이티브 평타 막타를 폴백합니다.

#### Zoe

- Kiri 교리를 보호 코드 없이 이식해 Q1-Q2 소유권, 최대 2875 벽 E, 안전한 R 복귀, W 파편, CC/채널/갭 반응, 수면 평타 차단, Semi E 우선순위를 정리했습니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- Twisted Fate
- Xin Zhao
- Urgot
- LeBlanc
- Vladimir
- Fiddlesticks
- Kayle
- Master Yi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu & Willump
- Miss Fortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Cho'Gath
- Amumu
- Rammus
- Anivia
- Shaco
- Dr. Mundo
- Sona
- Kassadin
- Irelia
- Janna
- Gangplank
- Corki
- Karma
- Taric
- Veigar
- Trundle
- Swain
- Caitlyn
- Blitzcrank
- Malphite
- Katarina
- Nocturne
- Maokai
- Renekton
- Jarvan IV
- Elise
- Orianna
- Wukong
- Brand
- Lee Sin
- Vayne
- Rumble
- Cassiopeia
- Skarner
- Heimerdinger
- Nasus
- Nidalee
- Udyr
- Poppy
- Gragas
- Pantheon
- Ezreal
- Mordekaiser
- Yorick
- Akali
- Kennen
- Garen
- Leona
- Malzahar
- Talon
- Riven
- Kog'Maw
- Shen
- Lux
- Xerath
- Shyvana
- Ahri
- Graves
- Fizz
- Volibear
- Rengar
- Varus
- Nautilus
- Viktor
- Sejuani
- Fiora
- Ziggs
- Lulu
- Draven
- Hecarim
- Kha'Zix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- Aurelion Sol
- Kayn
- Zoe
- Zyra
- Kai'Sa
- Seraphine
- Gnar
- Zac
- Yasuo
- Vel'Koz
- Taliyah
- Camille
- Akshan
- Bel'Veth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- Tahm Kench
- Briar
- Viego
- Senna
- Lucian
- Zed
- Kled
- Ekko
- Qiyana
- Vi
- Aatrox
- Nami
- Azir
- Yuumi
- Samira
- Thresh
- Illaoi
- Rek'Sai
- Ivern
- Kalista
- Bard
- Rakan
- Xayah
- Ornn
- Sylas
- Neeko
- Aphelios
- Rell
- Pyke
- Vex
- Yone
- Ambessa
- Mel
- Yunara
- Locke
- Sett
- Lillia
- Gwen
- Renata Glasc
- Aurora
- Nilah
- K'Sante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- v3.3.0 closes five distinct MESH fatal errors observed in user logs. Release gates now cover forbidden color/keybind setters, missing circular-prediction speed, undeclared constants, and vector multiplication on Hanbot vec2/vec3 proxy objects.
- Automatic non-targeted aiming was audited across all 237 `main.lua` files: 173 modern champions, 60 Classic champions, and the shared core. Sixty-two Lua paths no longer cast at current, cursor, or stale positions after prediction failure, and a new mutation checker blocks regressions.
- Long-delay spells now aim at the verified landing point of allied pulls and knockbacks such as Blitzcrank, Thresh, Nautilus, and Pyke. If that endpoint cannot be established, automation fails closed.
- AIO, MGoD Orb, and `[MESH]Evade` remain independently usable. AIO only resolves the public `meshevade` facade, throttled to 0.5 seconds, and neither creates native Evade3 nor hard-loads a companion script.
- Zoe rebuilds Kiri's Q/Q2, wall-E, safe-R, W-shard, and sleep-AA doctrine on the current API. Yone ports HGPro's split Q3 dash/hit ranges, Q-W-E-R flow, E return, R landing safety, and Q3-Flash into a hand-owned state machine without protected loaders or external dependencies.
- Eight Classic modules (Corki, Fiddlesticks, Heimerdinger, Janna, Malphite, Nidalee, Olaf, Pantheon) now apply the same fail-closed contract to long-delay and failed-prediction automation.
- CI jointly validates Lua 5.1, 173 AIO, 60 Classic, 234 menus, 233 Farm layouts, official 16.15 data, linear width, vectors, constants, forced movement, automatic aim, and weaving. Live names, server acceptance, and charge-release timing remain explicit F12 boundaries.

#### Aatrox

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.
- Replaced the proxy-vector multiplication behind the logged `number` versus `struct109` error with an explicit component dot product and made automatic Q fail closed.

#### Ahri

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Anivia

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Annie

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Aphelios

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Bard

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Belveth

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Cassiopeia

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Corki

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Ekko

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Ezreal

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Gragas

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Hwei

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Illaoi

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Irelia

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Jhin

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.
- W/E no longer aim at the pre-pull position of an allied hook target and prefer an officially derived forced-movement endpoint only when it is valid.

#### Kled

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### KogMaw

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Leona

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Lillia

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Lissandra

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Locke

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Lux

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Malphite

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Malzahar

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Maokai

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Mel

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Milio

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Mordekaiser

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Ornn

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Pantheon

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Poppy

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Pyke

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Rumble

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Senna

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Seraphine

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Shaco

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Shyvana

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Soraka

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Taliyah

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Taric

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Tristana

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Trundle

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Urgot

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Varus

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Veigar

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Velkoz

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Viego

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Viktor

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.
- Removed proxy-vector arithmetic, uses forced-movement landing points for W/R, and suppresses failed repeated casts that could flood the server.

#### Xerath

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.
- Separates R channel start from R2 shots, retries a ready shot every tick while Combo is held, and never falls back to current position after prediction failure.

#### XinZhao

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Zac

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Zed

- Automatic skillshots now fail closed instead of guessing the current position or cursor when no valid prediction, forced-movement endpoint, or dash endpoint exists.

#### Chogath

- Circular Q prediction now always supplies a non-missing instant-speed value, preventing the logged nil arithmetic failure.

#### Sylas

- Replaced arithmetic on the undeclared `Q_DETONATION` field with the owned Q detonation-delay constant and registered it with the constant checker.

#### Yasuo

- Q1/Q2/Q3 and EQ now require a valid prediction or dash endpoint, preventing empty-space casts.

#### Yone

- Rebuilt on HGPro doctrine with official 16.15 forms: Q3 dash 450 versus hit line 1050, Q-W-E-R, safe E return/execute, R landing checks, two-tick Q3-Flash, and reachable Semi R priority.

#### Zeri

- With Farm enabled, Lane Clear Q supports both valid minions and the enemy turret the orbwalker is actually attacking. It neither scans arbitrary structures nor selects turrets in Combo, and native-AA last hitting remains a fallback after the Q paths.

#### Zoe

- Ports Kiri doctrine without protected code: Q1-Q2 ownership, bounded 2875 wall E, safe R return, W shards, CC/channel/gap reactions, sleep-AA hold, and Semi E priority.

### 简体中文

#### 支持英雄

- 黑暗之女
- 狂战士
- 正义巨像
- 卡牌大师
- 德邦总管
- 无畏战车
- 诡术妖姬
- 猩红收割者
- 远古恐惧
- 正义天使
- 无极剑圣
- 牛头酋长
- 符文法师
- 亡灵战神
- 战争女神
- 众星之子
- 迅捷斥候
- 麦林炮手
- 祖安怒兽
- 雪原双子
- 赏金猎人
- 寒冰射手
- 蛮族之王
- 武器大师
- 堕落天使
- 时光守护者
- 炼金术士
- 痛苦之拥
- 瘟疫之源
- 死亡颂唱者
- 虚空恐惧
- 殇之木乃伊
- 披甲龙龟
- 冰晶凤凰
- 恶魔小丑
- 祖安狂人
- 琴瑟仙女
- 虚空行者
- 刀锋舞者
- 风暴之怒
- 海洋之灾
- 英勇投弹手
- 天启者
- 瓦洛兰之盾
- 邪恶小法师
- 巨魔之王
- 诺克萨斯统领
- 皮城女警
- 蒸汽机器人
- 熔岩巨兽
- 不祥之刃
- 永恒梦魇
- 扭曲树精
- 荒漠屠夫
- 德玛西亚皇子
- 蜘蛛女皇
- 发条魔灵
- 齐天大圣
- 复仇焰魂
- 盲僧
- 暗夜猎手
- 机械公敌
- 魔蛇之拥
- 上古领主
- 大发明家
- 沙漠死神
- 狂野女猎手
- 兽灵行者
- 圣锤之毅
- 酒桶
- 不屈之枪
- 探险家
- 铁铠冥魂
- 牧魂人
- 离群之刺
- 狂暴之心
- 德玛西亚之力
- 曙光女神
- 虚空先知
- 刀锋之影
- 放逐之刃
- 深渊巨口
- 暮光之眼
- 光辉女郎
- 远古巫灵
- 龙血武姬
- 九尾妖狐
- 法外狂徒
- 潮汐海灵
- 不灭狂雷
- 傲之追猎者
- 惩戒之箭
- 深海泰坦
- 奥术先驱
- 北地之怒
- 无双剑姬
- 爆破鬼才
- 仙灵女巫
- 荣耀行刑官
- 战争之影
- 虚空掠夺者
- 诺克萨斯之手
- 未来守护者
- 冰霜女巫
- 皎月女神
- 德玛西亚之翼
- 暗黑元首
- 铸星龙王
- 影流之镰
- 暮光星灵
- 荆棘之兴
- 虚空之女
- 星籁歌姬
- 迷失之牙
- 生化魔人
- 疾风剑豪
- 虚空之眼
- 岩雀
- 青钢影
- 影哨
- 虚空女皇
- 弗雷尔卓德之心
- 戏命师
- 永猎双子
- 祖安花火
- 暴走萝莉
- 河流之王
- 狂厄蔷薇
- 破败之王
- 涤魂圣枪
- 圣枪游侠
- 影流之主
- 暴怒骑士
- 时间刺客
- 元素女皇
- 皮城执法官
- 暗裔剑魔
- 唤潮鲛姬
- 沙漠皇帝
- 魔法猫咪
- 沙漠玫瑰
- 魂锁典狱长
- 海兽祭司
- 虚空遁地兽
- 翠神
- 复仇之矛
- 星界游神
- 幻翎
- 逆羽
- 山隐之焰
- 解脱者
- 万花通灵
- 残月之肃
- 镕铁少女
- 血港鬼影
- 愁云使者
- 封魔剑魂
- 铁血狼母
- 流光镜影
- 不破之誓
- 灰烬驱魔人
- 腕豪
- 含羞蓓蕾
- 灵罗娃娃
- 炼金男爵
- 双界灵兔
- 不羁之悦
- 纳祖芒荣耀
- 炽炎雏龙
- 明烛
- 不落魔锋
- 异画师
- 百裂冥犬

#### 核心与菜单

- v3.3.0 按根因修复了用户日志中的 5 类 MESH 致命错误。发布门禁现已覆盖非法 color/keybind setter、圆形预测缺少 speed、未声明常量，以及 Hanbot vec2/vec3 代理对象的向量乘法。
- 已审计全部 237 个 `main.lua` 的自动非指向瞄准：173 个现代英雄、60 个 Classic 英雄和共用核心。62 条 Lua 路径在预测失败后不再向当前位置、鼠标或过期路径施法，并由新的变异测试阻止回归。
- 长延迟技能会瞄准 Blitzcrank、Thresh、Nautilus、Pyke 等友方拉拽/击退的已验证落点；无法证明落点时自动逻辑会安全失败。
- AIO、MGoD Orb 与 `[MESH]Evade` 仍可分别独立使用。AIO 只解析公开 `meshevade` facade，并将重查限制为 0.5 秒；不会创建原生 Evade3，也不会硬加载其他脚本。
- Zoe 以当前 API 重建 Kiri 的 Q/Q2、穿墙 E、安全 R、W 碎片与睡眠普攻抑制；Yone 将 HGPro 的 Q3 冲刺/命中距离分离、Q-W-E-R、E 返回、R 落点安全和 Q3-Flash 移植为自有状态机，不包含保护 loader 或外部依赖。
- 8 个 Classic 模块（Corki、Fiddlesticks、Heimerdinger、Janna、Malphite、Nidalee、Olaf、Pantheon）的长延迟与预测失败自动施法也统一采用安全失败契约。
- CI 同时验证 Lua 5.1、173 AIO、60 Classic、234 菜单、233 Farm、官方 16.15 数据、线性宽度、向量、常量、强制位移、自动瞄准与 weave。实际名称、服务器接受与蓄力释放时序仍列为 F12 验证边界。

#### Aatrox

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。
- 将日志中 `number` 与 `struct109` 比较错误的代理向量乘法改为显式分量点积，并使自动 Q 安全失败。

#### Ahri

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Anivia

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Annie

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Aphelios

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Bard

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Belveth

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Cassiopeia

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Corki

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Ekko

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Ezreal

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Gragas

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Hwei

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Illaoi

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Irelia

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Jhin

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。
- W/E 不再瞄准友方钩子目标位移前的位置，仅在有效时优先使用官方推导的强制位移落点。

#### Kled

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### KogMaw

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Leona

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Lillia

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Lissandra

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Locke

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Lux

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Malphite

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Malzahar

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Maokai

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Mel

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Milio

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Mordekaiser

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Ornn

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Pantheon

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Poppy

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Pyke

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Rumble

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Senna

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Seraphine

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Shaco

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Shyvana

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Soraka

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Taliyah

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Taric

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Tristana

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Trundle

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Urgot

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Varus

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Veigar

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Velkoz

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Viego

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Viktor

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。
- 移除代理向量算术，W/R 使用强制位移落点，并抑制可能造成服务器请求洪泛的失败重复施法。

#### Xerath

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。
- 分离 R 开启与 R2 弹体状态，按住 Combo 时每 tick 重试已就绪弹体，预测失败后不再向当前位置施放。

#### XinZhao

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Zac

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Zed

- 自动非指向技能在无法取得有效预测点、强制位移落点或冲刺终点时会安全失败，不再猜测当前位置或鼠标位置。

#### Chogath

- 圆形 Q 预测始终提供非空的瞬时 speed，避免日志中的 nil 算术致命错误。

#### Sylas

- 用自有 Q 爆炸延迟常量替代未声明 `Q_DETONATION` 的算术，并加入常量检查。

#### Yasuo

- Q1/Q2/Q3 与 EQ 现在必须取得有效预测或冲刺终点，避免向空处施法。

#### Yone

- 按 HGPro 与官方 16.15 形态重建：Q3 冲刺 450/命中线 1050、Q-W-E-R、安全 E 返回与处决、R 落点检查、两 tick Q3-Flash，以及可达的 Semi R 优先级。

#### Zeri

- Farm 开启的 Lane Clear 中，Q 同时支持有效小兵和走砍器正在实际攻击的敌方防御塔；不会任意扫描建筑，也不会在 Combo 选择防御塔，原生普攻补刀仅作为 Q 路径之后的后备。

#### Zoe

- 不含保护代码地移植 Kiri：Q1-Q2 所有权、最多 2875 穿墙 E、安全 R 返回、W 碎片、CC/引导/突进反应、睡眠普攻抑制与 Semi E 优先级。
<!-- MESH-AIO:RELEASE:v3.3.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

- [v3.2.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.2.1)
- [v3.2.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.2.0)
- [v3.1.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.3)
- [v3.1.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.2)
- [v3.1.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.1)
- [v3.0.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.0.3)
- [v3.0.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.0.1)
- [v2.26.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.26.0)
- [v2.25.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.25.1)
- [v2.25.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.25.0)
- [v2.24.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.24.0)
- [v2.23.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.23.0)
- [v2.22.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.22.0)
- [v2.21.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.21.3)
- [v2.21.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.21.2)
- [v2.21.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.21.1)
- [v2.20.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.20.0)
- [v2.19.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.19.0)
- [v2.18.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.18.0)
- [v2.17.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.17.1)
- [v2.17.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.17.0)
- [v2.16.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.16.0)
- [v2.15.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.15.0)
- [v2.14.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.14.0)
- [v2.13.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.13.0)
- [v2.12.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.12.0)
- [v2.11.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.11.0)
- [v2.10.6](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.6)
- [v2.10.5](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.5)
- [v2.10.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.3)
- [v2.10.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.2)
- [v2.10.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.1)
- [v2.10.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.10.0)
- [v2.9.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.9.0)
- [v2.8.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.8.2)
- [v2.8.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.8.1)
- [v2.8.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.8.0)
- [v2.7.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.7.0)
- [v2.6.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.6.0)
- [v2.5.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.5.0)
- [v2.4.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.4.2)
- [v2.4.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.4.1)
- [v2.4.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.4.0)
- [v2.3.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.3.0)
- [v2.2.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.2.0)
- [v2.1.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.1.0)
- [v2.0.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.0.1)
- [v2.0.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.0.0)
- [v1.1.15](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.15)
- [v1.1.14](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.14)
- [v1.1.13](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.13)
- [v1.1.11](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.11)
- [v1.1.10](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.10)
- [v1.1.9](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.9)
- [v1.1.8](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.8)
- [v1.1.7](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.7)
- [v1.1.6](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.6)
- [v1.1.5](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.5)
- [v1.1.4](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.4)
- [v1.1.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.3)
- [v1.1.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.2)
- [v1.1.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.1)
- [v1.1.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.1.0)
- [v1.0.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.0.2)
- [v1.0.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.0.1)
- [v1.0.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v1.0.0)
<!-- MESH-AIO:UPDATES:END -->
