<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.0.1:START -->
## v3.0.1

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

- v3.0.1은 사용자 승인 AIO 폴더 18개를 전수 감사해 현대 173명을 모두 챔피언 소유 수작업 `main/menu/dmg` 상태기로 승격합니다. 생성 specialist와 공용 QWER 진입은 각각 0명이며 공식 16.15 프로필만 생성물로 유지합니다.
- League Classic(JADE) 60명도 실제 old-kit 전용 상태기로 교체했습니다. FXT 59명과 유일한 CSX Classic Rammus를 이식해 현대 프로필 폴백을 제거했고, 정확하지 않은 폼·재시전·자동 R은 기본 폐쇄합니다.
- 메뉴 선언과 실행 getter를 양방향 검사하고, 1인자 spell callback·TS 점 호출·linear width·Evade 우선·서버 pause를 전 모듈에 강제합니다. 조건식 cast의 이중 발행과 Classic dead alias도 회귀검사로 차단합니다.
- Classic 직접 위빙 11명(Jax/Kassadin/Nasus/Nidalee/Nunu/Olaf/Sivir/Taric/Vayne/Warwick/Wukong)은 `cb.spell`·windup 전이·호출 간격을 이중화하고, 실제 백스윙 0.12초 안에서 spell-lock만 1ms 재시도합니다.
- Classic 자동 판단에 쓰이는 공식 피해식도 전수 재대조해 Ahri, Amumu, Annie, Blitzcrank, Cho'Gath, Corki, Evelynn, Gangplank, Heimerdinger, Jax, Kassadin, Katarina, Kayle, Kog'Maw, Malzahar, Master Yi, Nasus, Nidalee, Nunu, Pantheon, Shaco, Singed, Sivir, Sona, Soraka를 교정하고 이전 식의 복귀를 검사로 차단합니다.
- 공식 raw가 중간 거리곡선을 주지 않는 Nidalee Q, FXT와 공식 자료가 충돌하는 Corki R 피해 유형·Heimer W 속도, 공식 cast time이 없는 Vayne E 지연은 F12 인게임 검증 경계로 명시했습니다.

#### Zeri

- FXT의 협곡 90개 방향 경로와 Q-Aio의 칼바람 14개 경로를 전용 E 벽타기에 연결했습니다. 아레나는 고정 좌표를 추측하지 않고 live navmesh를 스캔하며, 손상된 archive 도착점은 시전 근거로 사용하지 않습니다.

#### Tristana

- 현대 구현은 E 표식 집중·점프 안전·R 밀치기 상태기를 소유합니다. Classic은 현대 3스택 폭탄을 제거하고 공식 Jade 5초 Explosive Shot DoT·50% 치유 감소와 실제 windup 종료 기준 위빙으로 분리했습니다.

#### Rakan

- Q 미사일/회복 표식, W 안전 착지, E 1·2차 및 Xayah 확장 사거리, 위협 실드, E-W 브리지와 Q/W-Flash를 exact 폼 상태기로 구현했습니다. 자동 R은 기본 OFF입니다.

#### Skarner

- 현대 Q 바위/투척, E 벽 끌기, 3인 R 드래그와 타워 Q reset을 구현하고, Classic은 구형 Q/W/E/단일 Impale로 완전히 분리했습니다. Classic 자동 Impale는 새 마스터 스위치가 OFF면 인터럽트까지 모두 닫힙니다.

#### Zac

- 자기 Blob 회수와 W 환급, Q 첫 대상/강화평타 tether, 랭크별 E 충전·지형·포탑 안전, R 4회 bounce와 사이 W를 독립 상태기로 구현했습니다. 자동 R은 기본 OFF입니다.

#### Vayne

- Classic Silver Bolts를 공식 `20~60 + 대상 최대 체력 4~8%` 고정 피해와 몬스터 200 상한으로 교정하고, Condemn은 현재 위치가 아니라 투사체 도착 시점의 미래 위치에서 벽 충돌을 확인합니다. 실제 백스윙 spell-lock은 1ms 간격으로만 재시도합니다.

#### Warwick

- Classic Blood Scent E는 공식 16.15 raw의 Self 토글·4초 재사용과 FXT의 실제 self-cast를 함께 적용했습니다. 내부 Blood Scent 버프가 없을 때만 자동·수동·도주 경로가 정확한 E를 켭니다. Q는 비몬스터에게 고정 피해와 최대 체력 8~16% 중 큰 값을 쓰고, 중립 몬스터는 고정 피해만, 회복은 실제 피해의 80%를 사용합니다.

#### MonkeyKing

- Classic Decoy W를 공식 self 시전·1.5초 은신/분신으로 교정해 현대 300유닛 dash 가정을 제거했습니다. Cyclone 취소는 실제 `jade_wukongr` 버프가 확인될 때만 별도 self 재시전을 보내며, 자동 시작·인터럽트·1초 취소는 기본 OFF인 Auto R master 아래에 있습니다. E 5랭크 피해도 공식 240입니다.

#### TwistedFate

- Classic 카드 잠금은 exact Gold/Blue/Red 폼과 6초 수명을 추적하고, 대상 무효·사거리 이탈·폼 소멸 시 안전하게 해제합니다. 사용되지 않은 카드가 이후 모든 새 카드 선택을 영구 차단하던 상태 고착을 제거했습니다.

#### Tryndamere

- Classic Undying Rage 상태에 FXT와 MasterAio가 함께 관측한 `UndyingRage` live buff를 추가해 R 중 Q 치유 차단, 종료 직후 치유, 중복 R 방지와 상태 표시가 실제 버프를 놓치지 않게 했습니다.

#### Annie

- Classic Molten Shield E를 공식 self-only 시전으로 교정해 위협 반응, 패시브 스택, Tibbers 보호 판단과 도주 경로가 잘못된 대상 지정 전송으로 거부되지 않게 했습니다. Tibbers 오라는 `35 + 0.2 AP`, 기본 공격은 `80/105/130`으로 공식 수치를 적용하고 근거 없는 공격 AP 계수를 제거했습니다.

#### Ahri

- Classic Fox-Fire의 추가 불꽃은 공식 30% 보정으로 합계 1.6배만 계산하고, Spirit Rush는 `70/110/150 + 0.3 AP`로 교정했습니다.

#### Brand

- Classic Ablaze를 현대 3스택 폭발이 아닌 구형 4초 단일 상태로 되돌렸습니다. 총 최대 체력 2% 마법 피해와 중립 몬스터 80 상한만 적용하고, Q 기절·W 1.25배·E 확산·R bounce 결정은 실제 Ablaze 여부를 사용합니다.

#### Heimerdinger

- Classic W 피해가 FXT에서 마나 비용 배열로 잘못 추출된 값을 쓰던 문제를 수정해 공식 `85/135/185/235/285 + 0.55 AP`를 적용했습니다. FXT 속도 1700과 공식 raw 902가 충돌하는 미사일 속도는 추측하지 않고 F12 검증 항목으로 남겼습니다.

#### Nidalee

- Classic에는 Hunted가 없으므로 현대 550 확장 Pounce와 Hunted 증폭·변신 조건을 제거하고 구형 375 Pounce로 복원했습니다. 인간 Q는 공식 `55/95/140/185/230 + 0.65 AP`, 최대 2.5배를 사용하되 공개되지 않은 중간 거리곡선은 자동 처형·막타에서 추측하지 않습니다.

#### MasterYi

- Classic Alpha Strike를 구형 `100/150/200/250/300 + 1.0 AP` 마법 피해와 최대 4대상으로 복원했습니다. 현대 total-AD·고립 7/4 피해와 5~7대상 팜 계산을 제거했습니다.

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

- v3.0.1 audits all 18 user-authorized AIO folders and promotes all 173 modern champions to champion-owned, hand-tuned `main/menu/dmg` state machines. Generated-specialist and generic QWER routes are both zero; only the official 16.15 profiles remain generated.
- All 60 League Classic (JADE) champions now own real old-kit state machines. The 59 FXT kits plus the only CSX Classic Rammus implementation replace every modern-profile fallback, while uncertain forms, recasts, and automatic ultimates stay closed by default.
- Bidirectional menu contracts, one-argument spell callbacks, TS dot calls, linear width, Evade priority, and server pauses are enforced across every module. Regression checks also reject conditional-cast double emission and dead Classic aliases.
- The 11 direct Classic weavers (Jax/Kassadin/Nasus/Nidalee/Nunu/Olaf/Sivir/Taric/Vayne/Warwick/Wukong) now combine `cb.spell`, windup transition, and invoke-gap signals, retrying only a spell lock at 1 ms inside the real 0.12-second backswing.
- Official Classic damage formulas used by automatic decisions were re-audited end to end. Ahri, Amumu, Annie, Blitzcrank, Cho'Gath, Corki, Evelynn, Gangplank, Heimerdinger, Jax, Kassadin, Katarina, Kayle, Kog'Maw, Malzahar, Master Yi, Nasus, Nidalee, Nunu, Pantheon, Shaco, Singed, Sivir, Sona, and Soraka are corrected, with regression checks rejecting the displaced formulas.
- Nidalee Q's undisclosed intermediate distance curve, Corki R's and Heimer W's official/archive conflicts, and Vayne E's source-only cast delay are explicitly retained as F12 in-game validation boundaries.

#### Zeri

- Connected 90 directional Rift routes from FXT and 14 Howling Abyss routes from Q-Aio to the dedicated E wall ride. Arena uses live navmesh scanning instead of guessed coordinates, and damaged archive endpoints are never trusted for casting.

#### Tristana

- The modern module owns E-mark focus, safe jump, and R displacement state. Classic removes the modern three-stack bomb and uses the official five-second Jade Explosive Shot DoT, 50% Grievous Wounds, and real windup-end weaving.

#### Rakan

- Added exact-form state for the Q missile/heal mark, safe W landing, both E casts with Xayah range, threat shielding, the E-W bridge, and Q/W-Flash. Automatic R remains off by default.

#### Skarner

- Added modern rock Q/throw, wall-drag E, three-target R drag, and the exact turret Q reset, while Classic remains a separate old Q/W/E/single-target Impale kit. The new Classic master switch closes every automatic Impale path, including interrupts.

#### Zac

- Added owned Blob pickup and W refund, Q first-target/empowered-attack tethering, rank-scaled E charge with terrain/turret safety, and four R bounces with W between them. Automatic R remains off by default.

#### Vayne

- Corrected Classic Silver Bolts to the official `20–60 + 4–8% target maximum health` true damage with the 200 monster cap. Condemn now checks the target's future impact position rather than its current position, and a locked post-attack cast retries only on the 1 ms weave floor.

#### Warwick

- Classic Blood Scent E now follows both the official 16.15 raw Self toggle with its four-second cooldown and FXT's live self-cast path. Automatic, manual, and flee paths enable the exact E only while its internal buff is absent. Q uses the larger of flat and 8–16% maximum-health damage on non-monsters, flat damage only on neutral monsters, and heals for 80% of dealt damage.

#### MonkeyKing

- Corrected Classic Decoy W to its official self cast and 1.5-second stealth/clone, removing the modern 300-unit dash assumption. Cyclone cancellation sends a separate self recast only while the exact `jade_wukongr` buff is present; automatic start, interrupt, and one-second cancel all sit behind the default-off Auto R master. Rank-five E damage is the official 240.

#### TwistedFate

- Classic card locking tracks the exact Gold/Blue/Red form for six seconds and releases safely when the target becomes invalid, leaves range, or the form disappears. An unused card can no longer permanently block every later selection.

#### Tryndamere

- Added the live `UndyingRage` buff independently observed by FXT and MasterAio so Classic R correctly blocks Q healing, permits post-R healing, prevents duplicate R, and keeps the state display accurate.

#### Annie

- Corrected Classic Molten Shield E to its official self-only cast, so threat reactions, passive stacking, Tibbers protection decisions, and flee no longer fail through an invalid targeted transport. Tibbers' aura now uses the official `35 + 0.2 AP`, his basic attack uses `80/105/130`, and the unsupported attack AP ratio was removed.

#### Ahri

- Classic Fox-Fire secondary flames now use the official 30% modifier for a 1.6x three-flame total, while Spirit Rush uses `70/110/150 + 0.3 AP`.

#### Brand

- Restored Classic Ablaze as the old single four-second state instead of a modern three-stack explosion. It deals 2% maximum-health magic damage in total with an 80 raw cap against neutral monsters; Q stun, W's 1.25x bonus, E spread, and R bounce decisions now consume only the real Ablaze state.

#### Heimerdinger

- Fixed Classic W using an FXT array that was actually its mana cost; damage now follows the official `85/135/185/235/285 + 0.55 AP`. The conflicting missile speeds—1700 in FXT versus 902 in the official raw—remain an explicit F12 validation item instead of being guessed.

#### Nidalee

- Classic has no Hunted mechanic, so the modern 550 extended Pounce and Hunted amplification/transform gates were removed in favor of the old 375 Pounce. Human Q uses the official `55/95/140/185/230 + 0.65 AP` and 2.5x cap, while automatic executes and last hits do not guess the undisclosed intermediate distance curve.

#### MasterYi

- Restored Classic Alpha Strike to the old `100/150/200/250/300 + 1.0 AP` magic damage and four-target cap. Modern total-AD scaling, isolated 7/4 damage, and five-to-seven-target farm counts were removed.

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

- v3.0.1 完整审计 18 个用户授权 AIO 文件夹，并将 173 个现代英雄全部升级为英雄自有的手工 `main/menu/dmg` 状态机。生成 specialist 与通用 QWER 路由均为 0，仅官方 16.15 profile 保持生成。
- League Classic（JADE）60 个英雄也全部拥有真实旧技能组状态机。59 个 FXT 实现加唯一的 CSX Classic Rammus 替代所有现代 profile 回退；不确定形态、再次施放与自动 R 默认关闭。
- 全模块强制双向菜单契约、单参数 spell 回调、TS 点调用、直线 width、Evade 优先与服务器 pause。回归检查也会阻止条件 cast 双重发送和失效的 Classic 别名。
- 11 个直接 Classic 穿插英雄（Jax/Kassadin/Nasus/Nidalee/Nunu/Olaf/Sivir/Taric/Vayne/Warwick/Wukong）会结合 `cb.spell`、windup 转换与调用间隔信号，并只在真实 0.12 秒后摇窗口内以 1ms 重试 spell-lock。
- 重新逐项审计 Classic 自动判断使用的官方伤害公式，并修正 Ahri、Amumu、Annie、Blitzcrank、Cho'Gath、Corki、Evelynn、Gangplank、Heimerdinger、Jax、Kassadin、Katarina、Kayle、Kog'Maw、Malzahar、Master Yi、Nasus、Nidalee、Nunu、Pantheon、Shaco、Singed、Sivir、Sona 与 Soraka；回归检查会阻止旧公式恢复。
- Nidalee Q 未公开的中间距离曲线、Corki R 与 Heimer W 的官方/存档冲突，以及 Vayne E 仅有来源脚本依据的施法延迟，均明确保留为 F12 游戏内验证边界。

#### Zeri

- 将 FXT 的峡谷 90 条方向路线与 Q-Aio 的嚎哭深渊 14 条路线接入专属 E 穿墙。竞技场使用实时 navmesh 扫描而不是猜测坐标，损坏的归档终点绝不作为施法依据。

#### Tristana

- 现代模块独立管理 E 标记集火、安全跳跃与 R 击退。Classic 删除现代三层炸弹，改用官方 Jade 五秒 Explosive Shot 持续伤害、50% 重伤以及真实前摇结束后的连招窗口。

#### Rakan

- 为 Q 飞弹/治疗标记、W 安全落点、两段 E 与 Xayah 扩展距离、威胁护盾、E-W 衔接和 Q/W-闪现加入 exact 形态状态机。自动 R 默认关闭。

#### Skarner

- 实现现代拾石/投掷 Q、撞墙拖拽 E、三目标 R 拖行与精确防御塔 Q 重置；Classic 则完全分离为旧 Q/W/E/单目标 Impale。新的 Classic 总开关关闭时，连打断在内的所有自动 Impale 都不可用。

#### Zac

- 实现自有 Blob 拾取与 W 返还、Q 首目标/强化普攻连接、按等级变化且检查地形与防御塔的 E 蓄力，以及四次 R 弹跳间插入 W。自动 R 默认关闭。

#### Vayne

- 将 Classic Silver Bolts 修正为官方 `20~60 + 目标最大生命值 4~8%` 真实伤害并应用对野怪 200 上限。Condemn 改为在弹道到达时的未来位置检查撞墙，普攻后技能锁仅按 1ms 连招下限重试。

#### Warwick

- Classic Blood Scent E 同时遵循官方 16.15 raw 的 Self 切换技能、4 秒冷却与 FXT 的实际 self-cast 路径；仅在内部 Blood Scent 增益不存在时，自动、手动与逃跑路径才会开启精确 E。Q 对非野怪取固定伤害与最大生命值 8~16% 中较高者，对中立野怪只用固定伤害，并回复实际伤害的 80%。

#### MonkeyKing

- 将 Classic Decoy W 修正为官方 self 施放与 1.5 秒隐身/分身，移除现代 300 距离位移假设。Cyclone 只在确认 exact `jade_wukongr` buff 时发送独立 self 再施放来取消；自动开启、打断与一秒取消全部受默认关闭的 Auto R 总开关控制。E 五级伤害为官方 240。

#### TwistedFate

- Classic 选牌会追踪 exact 金/蓝/红牌形态与六秒寿命，并在目标失效、离开范围或形态消失时安全解除。未打出的牌不再永久阻止后续所有选牌。

#### Tryndamere

- 加入 FXT 与 MasterAio 独立观测一致的 live `UndyingRage` buff，使 Classic R 期间阻止 Q 治疗、R 后治疗、重复 R 防护和状态显示都不会漏掉真实状态。

#### Annie

- 将 Classic Molten Shield E 修正为官方 self-only 施放，使威胁反应、被动叠层、Tibbers 保护判断与逃跑不再因错误的目标施法方式而被拒绝。Tibbers 光环采用官方 `35 + 0.2 AP`，普通攻击采用 `80/105/130`，并移除无依据的攻击 AP 系数。

#### Ahri

- Classic Fox-Fire 的额外火焰采用官方 30% 修正，三发总计仅为 1.6 倍；Spirit Rush 修正为 `70/110/150 + 0.3 AP`。

#### Brand

- 将 Classic Ablaze 从现代三层爆炸恢复为旧版单一 4 秒状态。仅计算总计最大生命值 2% 的魔法伤害，并对中立野怪应用 80 原始伤害上限；Q 眩晕、W 1.25 倍、E 扩散与 R 弹跳判断只使用真实 Ablaze 状态。

#### Heimerdinger

- 修复 Classic W 误用 FXT 中实际为法力消耗的数组，伤害改为官方 `85/135/185/235/285 + 0.55 AP`。FXT 的 1700 与官方 raw 的 902 导弹速度互相冲突，因此不做猜测，保留为 F12 验证项。

#### Nidalee

- Classic 不存在 Hunted，因此移除现代 550 扩展 Pounce、Hunted 增幅与变形条件，恢复旧版 375 Pounce。人形 Q 使用官方 `55/95/140/185/230 + 0.65 AP` 与最高 2.5 倍；自动处决与补刀不会猜测未公开的中间距离曲线。

#### MasterYi

- 将 Classic Alpha Strike 恢复为旧版 `100/150/200/250/300 + 1.0 AP` 魔法伤害与最多 4 个目标，并移除现代 total-AD、孤立 7/4 伤害和 5~7 目标清线计算。
<!-- MESH-AIO:RELEASE:v3.0.1:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
