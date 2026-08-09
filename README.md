<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.0.3:START -->
## v3.0.3

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

- v3.0.3은 사용자 제공 44개 스크립트 자료와 HanbotDB의 Rift/Classic 채택 데이터를 다시 대조해 현대 173명과 League Classic 60명의 Q/W/E/R, 반응, 팜, 도주, 수동 입력, 상태 전이를 source-first로 전수 의미 감사했습니다. 읽을 수 있는 선정 원본의 메뉴 ID·기본값·동작 순서를 우선하고 Riot 16.15 형태·수치를 최종 권위로 사용합니다.
- DrMundo와 Naafiri가 버프 상수를 `_G[...]`로 찾다가 Hanbot 로드 단계에서 종료되던 오류를 제거했습니다. 모든 962개 Lua 표면과 릴리즈 CI가 런타임에 없는 `_G` 전역 환경 테이블의 재유입을 차단합니다.
- 현대 173명의 primary 분포는 FXT 135, CXJ AIO 17, MasterAio 5, Q-Aio 4, [HGPro]AIO 2, CNo1AIO 2, [HGVip]AIO 2, SA_AIO 2, Pixel-AIO 1, NG-AIO 1, KleeAIO 1, [Viktor]AIO 1입니다. loader·외부 의존 껍데기는 우선 원본으로 세지 않고 다음 readable 구현을 선택했습니다.
- League Classic 60명의 행동 primary는 FXT 50, BrianSharp 7, CXJ AIO 2, CSX AIO 1이며, 구형 스킬 형상은 FXT 59명과 CSX Rammus 1명을 사용합니다. JADE live 이름과 재시전 상태가 확인되지 않은 경로는 현대 폴백 없이 닫힙니다.
- 모든 자동 경로는 Evade 활성 틱을 먼저 반환하고 한 틱에 서버가 수락한 시전 하나만 허용합니다. 팜 스킬은 `(LaneClear | LastHit) && MMB`에서만 열리고 Last Hit은 처치 확정 대상만 사용하며, 자동 R·자동 변신 master는 기본 OFF입니다. 피해 판단은 도착 시점 HP, 버프 잔여시간과 live 모드 보정을 반영합니다.
- 이번 결과는 Lua와 정적 계약을 통과한 의미 감사이지 F12 인게임 검증 완료 선언이 아닙니다. 실제 spell alias, 승인·재시전·채널, 지형·점멸·타워 타이밍은 게임에서 확인해야 하며 정적으로 확정하지 못한 운송은 실패 폐쇄했습니다.

#### Gangplank

- CNo1AIO의 단일·이중·삼중 배럴 상태기와 E 배치·연결 변형을 현재 API로 이식했습니다. 예상 배럴 체력과 폭발 시점으로 Q·평타·패시브·Sheen 우선순위를 중재하고 EEQ/EEA, fake-AA, anti-dash, 귀환 및 업그레이드 R 판단을 연결했으며 자동 R은 기본 OFF입니다.

#### Hwei

- FXT의 10개 Q/W/E 팔레트 결정을 exact live form과 서버 승인 응답을 기다리는 2단계 시전으로 재구성했습니다. R→E2→Q2 후속, CC·갭클로저·인터럽트·스테이시스·팜 반응을 연결하고 stale palette는 안전하게 닫으며 자동 R master는 기본 OFF입니다.

#### Jayce

- FXT를 주계약으로 캐논/해머 exact form, 기존 가속 관문 재사용, EQ 미니언 스플래시, 전투·팜·인터럽트·도주 변신 순서를 복원했습니다. 반대 폼 HUD와 캐논 W 타워 위빙을 유지하되 모든 비수동 변신은 기본 OFF master 아래에서만 열립니다.

#### Pyke

- Q-Aio의 차징·처형 결정을 기준으로 차징 Q→평타→E, W 접근→E→Q, 커서 Delivery E→Q를 독립 상태기로 연결했습니다. Q 차징 중 R 처형 선점과 E-Flash/Q-Flash 승인 순서를 보존하며 자동 R master는 기본 OFF입니다.

#### Sylas

- FXT 14,203줄 원본과 173개 궁 소유자 exact alias를 대조해 훔친 궁의 승인·재시전·차징·채널 상태를 소유자별로 해석합니다. Kai'Sa, Brand, Yasuo, Nidalee/Jayce, Master Yi/Jax, Olaf, Xerath, Kha'Zix, Janna, Azir, Lee Sin, Hwei 전술을 연결했고 모든 자동 훔친 궁은 기본 OFF master를 요구합니다.

#### Viego

- [Viktor]AIO의 원본 비에고 결정을 유지하면서 빙의 중 Q/W/E를 원래 소유자의 Riot 16.15 profile과 모드별 순서로 해석합니다. 두 개 이상의 live alias가 같은 소유자를 가리킬 때만 열고 재시전·차징·채널·변신처럼 소유자 상태가 필요한 형태는 실패 폐쇄하며 자동 영혼 획득과 자동 R은 기본 OFF입니다.

#### Yasuo

- CXJ AIO의 Q1/Q2/Q3, 안전한 E 이동 대상, Q3 보존, 공중 체공 잔여시간 기반 EQR·역순 QR·직접 R 결정을 이식했습니다. EQ3-Flash, 벽넘기 도주, 팜 상태기를 분리했으며 자동 R과 자동 EQ3-Flash는 각각 기본 OFF master 아래에 있습니다.

#### Zeri

- Q-Aio를 기준으로 Q를 전투·파밍의 주공격으로 고정하고 일반 평타는 예측 막타, 완충 패시브 또는 사용자가 누른 Double Q 준비일 때만 엽니다. 실제 평타 백스윙의 Q→E 더블 Q, 협곡 90개·칼바람 14개 벽타기 경로와 Arena live scan, `I` 비효율 R 차단을 연결했으며 자동 R은 기본 OFF입니다.

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

- v3.0.3 re-audits all 44 user-provided script archives and HanbotDB Rift/Classic adoption data, then reviews Q/W/E/R, reactions, farming, flee, manual inputs, and state transitions source-first for 173 modern and 60 League Classic champions. Selected readable menu IDs, defaults, and action order lead; Riot 16.15 forms and values remain authoritative.
- Fixed a Hanbot load-time crash in DrMundo and Naafiri caused by resolving buff constants through `_G[...]`. All 962 Lua surfaces and release CI now reject the unavailable `_G` environment table from runtime sources.
- The 173 modern primaries are FXT 135, CXJ AIO 17, MasterAio 5, Q-Aio 4, [HGPro]AIO 2, CNo1AIO 2, [HGVip]AIO 2, SA_AIO 2, Pixel-AIO 1, NG-AIO 1, KleeAIO 1, and [Viktor]AIO 1. Loader shells and unavailable external dependencies do not outrank the next readable implementation.
- League Classic's 60 behavior primaries are FXT 50, BrianSharp 7, CXJ AIO 2, and CSX AIO 1; old-kit geometry comes from FXT for 59 champions and CSX for Rammus. Unconfirmed JADE live names and recast states close instead of falling back to a modern kit.
- Every automatic path yields to Evade and permits only one server-accepted cast per tick. Farm spells require `(LaneClear | LastHit) && MMB`, Last Hit remains lethal-only, and automatic R or transformation masters default off. Damage decisions use impact-time health, remaining buff time, and live mode balance.
- These results are semantic, Lua, and static-contract validation—not a claim that F12 in-game testing is complete. Live spell aliases, acknowledgements, recasts, channels, terrain, Flash, turret, and timing behavior still require field verification; transports that cannot be proven statically fail closed.

#### Gangplank

- Ported CNo1AIO's single-, double-, and triple-barrel state machines plus E placement and link variants to the current API. Predicted keg health and detonation timing arbitrate Q, attacks, passive, and Sheen; EEQ/EEA, fake-AA, anti-dash, recall, and upgraded-R decisions are connected, with automatic R off by default.

#### Hwei

- Rebuilt FXT's ten Q/W/E palette decisions as two-step casts that require the exact live form and a server acknowledgement. R→E2→Q2 follow-up and CC, gapclose, interrupt, stasis, and farm reactions are connected; stale palettes close safely and the automatic-R master defaults off.

#### Jayce

- Restored FXT as the primary contract for exact Cannon/Hammer forms, existing-gate reuse, EQ minion splash, and combat, farm, interrupt, and flee transformations. The opposite-form HUD and Cannon-W turret weave remain, while every non-manual transformation requires the default-off master.

#### Pyke

- Kept Q-Aio charge and execute decisions while separating charged Q→AA→E, W approach→E→Q, and cursor Delivery E→Q into explicit states. R execution can preempt a Q charge, E-Flash/Q-Flash wait for owned acknowledgements, and the automatic-R master defaults off.

#### Sylas

- Cross-checked the 14,203-line FXT source against exact aliases for all 173 ultimate owners, then tracked acknowledgement, recast, charge, and channel state per owner. Dedicated Kai'Sa, Brand, Yasuo, Nidalee/Jayce, Master Yi/Jax, Olaf, Xerath, Kha'Zix, Janna, Azir, Lee Sin, and Hwei tactics all require the default-off stolen-R master when automatic.

#### Viego

- Retained [Viktor]AIO's native Viego decisions and now resolves possessed Q/W/E through the original owner's Riot 16.15 profile and mode-specific order. Borrowed actions open only when at least two live aliases agree on one owner; recasts, charges, channels, and transforms that need owner state fail closed, and automatic soul taking and R remain off by default.

#### Yasuo

- Ported CXJ AIO's Q1/Q2/Q3 handling, safe E bodies, Q3 conservation, and airborne-time decisions for EQR, reverse QR, and direct R. EQ3-Flash, wall-flee, and farm states are separate, with automatic R and automatic EQ3-Flash protected by independent default-off masters.

#### Zeri

- Made Q-Aio's Q the primary combat and farming attack; an ordinary basic attack opens only for a predicted last hit, a fully charged passive, or a user-held Double Q. Added the real-backswing Q→E sequence, 90 Rift and 14 Howling Abyss wall routes plus Arena live scan, and the `I` ineffective-R block, while automatic R stays off by default.

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

- v3.0.3 重新核对用户提供的 44 份脚本资料与 HanbotDB 的 Rift/Classic 采用数据，并对 173 个现代英雄和 60 个 League Classic 英雄的 Q/W/E/R、反应、清线、逃跑、手动输入与状态转换进行 source-first 语义审计。优先采用可读原版的菜单 ID、默认值和动作顺序，Riot 16.15 的形态与数值仍是最终依据。
- 修复 DrMundo 与 Naafiri 通过 `_G[...]` 查找增益常量而导致的 Hanbot 加载阶段崩溃。全部 962 个 Lua 表面与发布 CI 现在都会拒绝运行时不存在的 `_G` 全局环境表。
- 现代 173 个 primary 的分布为 FXT 135、CXJ AIO 17、MasterAio 5、Q-Aio 4、[HGPro]AIO 2、CNo1AIO 2、[HGVip]AIO 2、SA_AIO 2、Pixel-AIO 1、NG-AIO 1、KleeAIO 1、[Viktor]AIO 1。只有加载器外壳或依赖不可用的来源不会压过下一份可读实现。
- League Classic 60 个行为 primary 为 FXT 50、BrianSharp 7、CXJ AIO 2、CSX AIO 1；旧技能几何由 FXT 提供 59 个，Rammus 使用 CSX。未确认的 JADE live 名称与再次施放状态会直接关闭，不回退到现代技能组。
- 所有自动路径先让 Evade 接管，每 tick 只允许一次服务器接受的施法。清线技能必须满足 `(LaneClear | LastHit) && MMB`，Last Hit 仅对确认可击杀目标使用，自动 R 与自动变形总开关默认关闭；伤害判断使用命中时生命值、剩余增益时间与实时模式平衡。
- 本次结果代表语义、Lua 与静态契约验证通过，并不表示 F12 游戏内测试已经完成。实际技能别名、确认、再次施放、引导、地形、Flash、防御塔与时序仍需实战验证；无法静态确认的施法传输会失败关闭。

#### Gangplank

- 将 CNo1AIO 的单桶、双桶、三连桶状态机以及 E 的放置和连接变化迁移到当前 API。通过预测火药桶血量与爆炸时机协调 Q、普攻、被动和 Sheen，并接入 EEQ/EEA、假普攻、反突进、回城与升级 R 判断；自动 R 默认关闭。

#### Hwei

- 将 FXT 的十种 Q/W/E 调色板决策重建为等待 exact live form 与服务器确认的两步施法。接入 R→E2→Q2 后续，以及控制、突进、打断、凝滞和清线反应；过期调色板会安全关闭，自动 R 总开关默认关闭。

#### Jayce

- 以 FXT 为主契约，恢复炮形态/锤形态 exact form、复用现有加速之门、EQ 小兵溅射，以及战斗、清线、打断和逃跑变形顺序。保留另一形态 HUD 与炮形态 W 防御塔衔接，所有非手动变形都必须经过默认关闭的总开关。

#### Pyke

- 保留 Q-Aio 的蓄力和斩杀决策，并将蓄力 Q→普攻→E、W 接近→E→Q、鼠标 Delivery E→Q 拆分为明确状态。R 斩杀可抢占 Q 蓄力，E-Flash/Q-Flash 等待自身施法确认，自动 R 总开关默认关闭。

#### Sylas

- 将 14,203 行 FXT 原版与 173 个大招拥有者的 exact alias 逐一对照，按拥有者跟踪确认、再次施放、蓄力与引导状态。Kai'Sa、Brand、Yasuo、Nidalee/Jayce、Master Yi/Jax、Olaf、Xerath、Kha'Zix、Janna、Azir、Lee Sin、Hwei 的专属战术在自动使用时都要求默认关闭的偷取大招总开关。

#### Viego

- 保留 [Viktor]AIO 的原生 Viego 决策，并在附身时按原拥有者的 Riot 16.15 profile 与模式顺序解析 Q/W/E。只有至少两个 live alias 指向同一拥有者时才开放；需要拥有者状态的再次施放、蓄力、引导和变形会失败关闭，自动夺魂与自动 R 默认关闭。

#### Yasuo

- 迁移 CXJ AIO 的 Q1/Q2/Q3、安全 E 目标、Q3 保留，以及按击飞剩余时间执行 EQR、反向 QR、直接 R 的判断。EQ3-Flash、穿墙逃跑和清线使用独立状态，自动 R 与自动 EQ3-Flash 分别由默认关闭的总开关保护。

#### Zeri

- 按 Q-Aio 将 Q 固定为战斗与清线主攻击，普通攻击只在预测补刀、满充能被动或玩家按住 Double Q 时开放。加入真实普攻后摇的 Q→E、峡谷 90 条与嚎哭深渊 14 条翻墙路线和 Arena 实时扫描，并用 `I` 阻止无效 R；自动 R 仍默认关闭。
<!-- MESH-AIO:RELEASE:v3.0.3:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
