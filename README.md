<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.4.0:START -->
## v3.4.0

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

- v3.4.0은 Riot 26.16의 7개 챔피언 밸런스와 변경 아이템 10종을 공식 노트·직접 client-bin fixture로 반영했습니다. Data Dragon 16.16.1과 아직 16.15인 CommunityDragon을 섞지 않도록 전체 갱신은 실패 폐쇄합니다.
- League Classic 전용 모듈은 60명에서 63명으로 늘었습니다. Akali, Kennen, Shen은 Riot F6 game manifest의 exact `Jade_*` 이름·old-kit 형상·피해식만 사용하며 현대 스킬 폴백은 없습니다.
- 현대 173명 wrapper와 직접 시전 426곳을 전수 검사합니다. 서버가 `false`를 반환한 요청은 시전 성공으로 처리하지 않아 Flash 연계·차징 해제·조향·후속 콤보가 거짓으로 진행되지 않습니다.
- 기존 Classic 60명의 스킬·Flash·와드·아이템 경로도 accepted-only로 통일했습니다. 실패한 요청은 예산이나 상태를 소비하지 않고, 성공한 한 요청만 한 틱을 소유합니다.
- 변경 아이템 ID의 Lua 소비를 전수 검사해 오래된 Eclipse, Sterak, Sundered Sky, Sunfire, Black Cleaver 계수를 스크립트가 하드코딩하지 않도록 고정했습니다.
- Lua 981개, 현대 AIO 173명, Classic 63명, 메뉴 237개, Farm 236명, 자동 조준 240개와 공식 계약 629개를 CI에서 함께 검사합니다. 새 JADE buff/particle와 실제 서버 ACK는 F12 후속 경계입니다.

#### Ahri

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Alistar

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Amumu

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### AurelionSol

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Aurora

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Briar

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Caitlyn

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Draven

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Janna

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Jhin

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### KSante

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Locke

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- Riot 26.16 ARAM Mayhem 피해량 105%·받는 피해 95%를 생성 모드 밸런스에 반영했습니다.

#### Lux

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Malphite

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Mel

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Neeko

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Nilah

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Orianna

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Rakan

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Rumble

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Sion

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Skarner

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Teemo

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.
- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Varus

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Velkoz

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Warwick

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Xerath

- 서버가 자동 스킬 요청을 거부하면 로컬 한 틱 시전 예산·pause·후속 상태를 소비하지 않고, 조건이 유지되는 다음 틱에 다시 시도합니다.

#### Blitzcrank

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Corki

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### DrMundo

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Evelynn

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Ezreal

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Fiddlesticks

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Gangplank

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Garen

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Heimerdinger

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### JarvanIV

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Jax

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Kassadin

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Katarina

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Kayle

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### KogMaw

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Leona

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### MissFortune

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Ryze

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Twitch

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Vayne

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.

#### Veigar

- League Classic 전용 상태기도 스킬·점멸·아이템·와드 요청이 실제로 수락된 뒤에만 콤보 단계와 시전 예산을 진행합니다.
- League Classic old-kit의 피해식·폭·사거리·재시전 값은 승인 자료와 Riot F6 원본에 다시 고정해 현대 키트 값을 섞지 않습니다.

#### Akali

- League Classic Akali를 exact Q/W/E/R old-kit 상태기로 추가했습니다. 저체력 W는 독립적으로 작동하고 현대 E/R 재시전을 추측하지 않습니다.

#### Azir

- Riot 26.16 Q 기본 피해를 랭크별 75/95/115/135/155로 갱신했습니다.

#### Belveth

- Riot 26.16의 레벨당 체력과 R 공격 속도 변경을 공식 회귀 fixture에 고정하고 런타임 live 능력치를 권위로 유지합니다.

#### Camille

- Riot 26.16 W 외곽 최대 체력 피해, passive 보호막 레벨 구간과 cooldown, W cooldown을 갱신했습니다.

#### Gwen

- Riot 26.16 passive 회복 비율과 챔피언별 회복 상한을 공식 계약에 고정해 오래된 상한을 다시 넣지 못하게 했습니다.

#### Kennen

- 현대 R 피해/AP 계수와 저항 증가를 26.16에 맞췄고, Classic은 exact Q 투사체·E 몸체·R 오라 상태기로 별도 추가했습니다.

#### Nasus

- Riot 26.16 Q 기본/대형 대상 스택 4/10 계약을 고정하고 실제 스택은 live 상태를 사용합니다.

#### Poppy

- Riot 26.16 기본 능력치와 Q 체력 비율·비챔피언 상한·추가 AD 계수, W 저항 변경을 반영했습니다.

#### Shen

- League Classic Shen을 targeted Q, self W, 575 거리 E 도발 대시, 아군 R 채널의 exact old-kit 상태기로 추가했습니다.

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

- v3.4.0 applies Riot 26.16 balance changes for seven champions and ten changed items from official notes and direct client-bin fixtures. A full refresh fails closed instead of mixing Data Dragon 16.16.1 with CommunityDragon 16.15.
- The dedicated League Classic roster grows from 60 to 63. Akali, Kennen, and Shen use only exact `Jade_*` names, old-kit geometry, and damage from Riot's F6 game manifest, with no modern-spell fallback.
- All 173 modern wrappers and 426 direct casts are audited. A request returning `false` no longer advances Flash chains, charge release, steering, follow-ups, local pause, or the one-tick cast budget.
- Spell, Flash, ward, and item paths across the original 60 Classic modules now follow the same accepted-only contract: a rejected request consumes no state, while one accepted request owns the tick.
- Every Lua consumer of changed item IDs is allowlisted, preventing stale Eclipse, Sterak, Sundered Sky, Sunfire, or Black Cleaver coefficients from being hardcoded back into champion scripts.
- CI jointly validates 981 Lua files, 173 modern AIO modules, 63 Classic modules, 237 menus, 236 Farm layouts, 240 automatic-aim paths, and 629 official contracts. New JADE buffs, particles, and server acknowledgements remain explicit F12 boundaries.

#### Ahri

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Alistar

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Amumu

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### AurelionSol

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Aurora

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Briar

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Caitlyn

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Draven

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Janna

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Jhin

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### KSante

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Locke

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- Applied Riot 26.16 ARAM Mayhem modifiers of 105% damage dealt and 95% damage taken to generated mode balance data.

#### Lux

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Malphite

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Mel

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Neeko

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Nilah

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Orianna

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Rakan

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Rumble

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Sion

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Skarner

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Teemo

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.
- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Varus

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Velkoz

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Warwick

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Xerath

- When the server rejects an automatic cast, the local one-tick budget, pause, and follow-up state remain untouched so the action can retry on the next valid tick.

#### Blitzcrank

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Corki

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### DrMundo

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Evelynn

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Ezreal

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Fiddlesticks

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Gangplank

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Garen

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Heimerdinger

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### JarvanIV

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Jax

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Kassadin

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Katarina

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Kayle

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### KogMaw

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Leona

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### MissFortune

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Ryze

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Twitch

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Vayne

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.

#### Veigar

- League Classic state machines advance spell, Flash, item, and ward sequences only after the request is accepted by the server.
- League Classic old-kit damage, width, range, and recast values are pinned to authorized sources and Riot F6 data without borrowing modern-kit values.

#### Akali

- Added League Classic Akali as an exact Q/W/E/R old-kit state machine. Low-health W remains independent, and modern E/R recasts are never guessed.

#### Azir

- Updated Riot 26.16 Q base damage to 75/95/115/135/155 by rank.

#### Belveth

- Pinned Riot 26.16 health-per-level and R attack-speed changes while keeping live runtime stats authoritative.

#### Camille

- Updated Riot 26.16 outer-W max-health damage, passive shield level bands and cooldown, and W cooldown.

#### Gwen

- Pinned Riot 26.16 passive healing ratio and champion healing cap so stale caps cannot be restored.

#### Kennen

- Updated modern R damage/AP scaling and resistance gains for 26.16, and added a separate Classic exact-Q, moving-E-body, and attached-R-aura state machine.

#### Nasus

- Pinned Riot 26.16 Q stack gains of 4/10 while continuing to read the actual live stack state.

#### Poppy

- Applied Riot 26.16 base stats, Q health ratio, non-champion cap and bonus-AD ratio, plus the W resistance change.

#### Shen

- Added League Classic Shen with targeted Q, self W, a 575-range E taunt dash, and the exact ally-targeted R channel.

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

- v3.4.0 根据官方说明和直接 client-bin fixture 应用 Riot 26.16 的 7 名英雄与 10 件装备改动。完整刷新会安全失败，避免把 Data Dragon 16.16.1 与 CommunityDragon 16.15 混合。
- League Classic 独立模块从 60 名增至 63 名。Akali、Kennen、Shen 只使用 Riot F6 game manifest 的精确 `Jade_*` 名称、旧版几何与伤害，不回退到现代技能。
- 审计全部 173 个现代 wrapper 与 426 个直接施法。返回 `false` 的请求不再错误推进闪现连段、蓄力释放、引导转向、后续状态、本地暂停或单 tick 预算。
- 原 60 个 Classic 模块的技能、闪现、守卫与装备路径统一采用 accepted-only 契约：拒绝的请求不消耗状态，只有一个已接受请求占用该 tick。
- 对改动装备 ID 的全部 Lua 使用点实施白名单，防止在英雄脚本中重新硬编码旧版 Eclipse、Sterak、Sundered Sky、Sunfire 或 Black Cleaver 系数。
- CI 同时验证 981 个 Lua 文件、173 个现代 AIO、63 个 Classic 模块、237 个菜单、236 个 Farm 布局、240 条自动瞄准路径与 629 条官方契约。新 JADE buff、粒子和服务器确认仍为 F12 验证边界。

#### Ahri

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Alistar

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Amumu

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### AurelionSol

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Aurora

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Briar

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Caitlyn

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Draven

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Janna

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Jhin

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### KSante

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Locke

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- 在生成的模式平衡数据中应用 Riot 26.16 ARAM Mayhem 造成伤害 105%、承受伤害 95%。

#### Lux

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Malphite

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Mel

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Neeko

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Nilah

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Orianna

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Rakan

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Rumble

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Sion

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Skarner

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Teemo

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。
- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Varus

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Velkoz

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Warwick

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Xerath

- 服务器拒绝自动施法时，不消耗本地单 tick 预算、暂停或后续状态；条件仍有效时可在下一 tick 重试。

#### Blitzcrank

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Corki

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### DrMundo

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Evelynn

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Ezreal

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Fiddlesticks

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Gangplank

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Garen

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Heimerdinger

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### JarvanIV

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Jax

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Kassadin

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Katarina

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Kayle

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### KogMaw

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Leona

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### MissFortune

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Ryze

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Twitch

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Vayne

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。

#### Veigar

- League Classic 状态机仅在服务器接受请求后才推进技能、闪现、装备与守卫连段。
- League Classic 旧版技能的伤害、宽度、距离与重施数值固定到授权资料和 Riot F6 数据，不混用现代技能组。

#### Akali

- 新增 League Classic Akali 精确 Q/W/E/R 旧版状态机；低血量 W 独立工作，且不会猜测现代 E/R 重施。

#### Azir

- 将 Riot 26.16 Q 基础伤害更新为每级 75/95/115/135/155。

#### Belveth

- 固定 Riot 26.16 每级生命与 R 攻速改动，同时继续以运行时 live 属性为权威。

#### Camille

- 更新 Riot 26.16 W 外圈最大生命伤害、被动护盾等级区间与冷却，以及 W 冷却。

#### Gwen

- 固定 Riot 26.16 被动治疗比例和对英雄治疗上限，阻止旧上限回归。

#### Kennen

- 更新现代 R 伤害/AP 系数和抗性增益，并新增独立 Classic 精确 Q、移动 E 身体与附着 R 光环状态机。

#### Nasus

- 固定 Riot 26.16 Q 叠层 4/10，并继续读取实际 live 层数。

#### Poppy

- 应用 Riot 26.16 基础属性、Q 生命比例、非英雄上限与额外 AD 系数，以及 W 抗性改动。

#### Shen

- 新增 League Classic Shen：目标 Q、自身 W、575 距离 E 嘲讽冲刺，以及精确的友军目标 R 引导。
<!-- MESH-AIO:RELEASE:v3.4.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

- [v3.3.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.3.0)
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
