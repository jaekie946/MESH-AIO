<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.10.2:START -->
## v2.10.2

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.10.2. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.
- Q 막타가 정글 몬스터에도 동작합니다(중립 목록을 스캔하지 않아 라인에서만 되던 문제 수정). 막타 우선순위는 처치 가능한 대포·슈퍼 미니언 최우선, 그 외에는 체력이 가장 낮은 미니언 순입니다. 자기 화약통은 막타 대상에서 제외됩니다.
- 트리플 배럴 옵션(기본 켜짐): 콤보에서 화약통을 최대 3개까지 연계해 사거리를 늘립니다.
- 자동 콤보의 사슬이 E-Q-E 방식으로 바뀌었습니다(사용자 교리): 미리 둘째 통을 까는 기존 E-E-Q는 적이 통을 부수거나 피하기 쉬워, 이제 준비된 통이 연결 거리 1~2개 안에 대상을 두면 즉시 Q로 격발하고 후속 통들은 Q·퓨즈가 날아가는 동안 실시간 대상 위치로 이어집니다(대상이 움직이면 자연스럽게 사선 연결).
- 시작 통 위치를 N 키로 실시간 전환할 수 있습니다(내 쪽 / 상대 쪽, 상태줄에 EnemySide로 표시). 메뉴 드롭다운은 기본값이고 토글이 뒤집습니다.
- 세미 통(X1MB)이 이제 안정적으로 격발합니다: 수동 키는 명시적 의도이므로 준비된 통이면 주변 적 여부와 무관하게 즉시 터뜨립니다.
- E-Q-E(G)의 간헐 동작 두 가지를 고쳤습니다: Q가 쿨다운이어도 첫 통을 미리 깔고(대기 중 Q가 돌아옴), Q 격발과 같은 틱에 나가는 두 번째 통이 내부 틱 가드에 먹혀 무작위로 빠지던 문제를 직접 시전으로 해결했습니다.
- E-Q-E(G)는 거리 적응형이 되었습니다: 대상이 E-Q-E 사거리면 두 통으로, 그보다 멀고 충전이 3개 있으면 자동으로 E-Q-E-E 세 통 체인으로 실행합니다. 첫 통은 항상 연결 거리의 정수 배만큼 대상 뒤에 깔려 마지막 통이 대상 정중앙에 떨어지고, 세 번째 통은 공식 0.5초 설치 간격에 맞춰 키를 떼도 자동으로 이어집니다.
- 콤보 타겟 탐색이 Q/E 사거리(1000)로 잘려 있어, 발밑의 준비된 통으로 체인이 닿는 먼 적(최대 약 2400)에게 아무 것도 하지 않던 문제를 고쳤습니다. 이제 통 플레이의 실제 도달 거리까지 타겟을 잡습니다.
- 평타 격발 연계를 추가했습니다: 준비된 통이 평타 사거리 안이면 Q를 아끼고 평타로 격발하며, 격발 순간 후속 통이 퓨즈를 타고 이어집니다(평-E). 통이 평타 밖이면 기존처럼 Q 트리거(Q-E)를 씁니다.
- 콤보에서 챔피언 직접 Q는 이제 처형 전용입니다: Q 한 발로 죽는 적이거나 통 플레이가 아예 불가능할 때(통·충전 전무)만 나갑니다. 하레스 견제 Q는 그대로입니다.
- 화약통 설치 간격이 연결 거리 슬라이더의 경계값 그대로여서 실제로는 이어지지 않던 문제를 고쳤습니다: 모든 자동/세미 배치는 이제 슬라이더보다 60유닛 안쪽으로 깔려 경계 오차로 사슬이 끊기지 않습니다(기존 통 감지·표시는 슬라이더 값 그대로).
- Q 리드 격발이 너무 일찍 나가 통을 터뜨리지 못하고 체력만 깎던 버그를 고쳤습니다: 감소 틱 경계 정각에 도착하도록 쏘던 것을, 내장 150ms 안전 여유(+ 슬라이더 추가분)만큼 틱이 지난 뒤 도착하도록 바꿨습니다. 평타 격발은 관측 체력이 1일 때만 나갑니다.
- 자동 한타 R를 추가했습니다(기본 켜짐): 궁은 글로벌이므로 모든 적을 후보 중심으로 보고, 설정한 인원(기본 3명, 조절 가능)이 525 충격파 안에 확실히 들어오는 최적 지점에 자동 시전합니다. 명중 신뢰도 옵션을 켜면 0.5초 시전 동안 걸어 나갈 수 없는 적만 셉니다.
- 세미 통(X1MB)은 마우스 위치가 아니라 마우스 방향 최대 거리에 설치합니다: 기존 통이 있으면 그 통에서 연결 거리 최대로 연장하고, 없으면 Q가 직접 닿는 최대 거리에 깝니다(짧은 거리 낭비 수정).

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.10.2. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.
- The Q last hit now also works on jungle monsters (the neutral list was not scanned, so only lane worked). Priority: a killable cannon/super minion always first, then the lowest-health minion; our own kegs are excluded as targets.
- Triple barrel option (default on): Combo chains up to three kegs for range.
- The automatic combo chain now plays E-Q-E (user doctrine): the old pre-placed second keg (E-E-Q) was visible and got broken or dodged, so a ready keg within one or two links of the target is Q-detonated immediately and the follow-up kegs land while the Q and fuse are already in the air, aimed at the target's live position (naturally diagonal when they move).
- The opening barrel side flips in real time on N (my side / enemy side, shown as EnemySide in the status list). The menu dropdown is the default and the toggle inverts it.
- The semi barrel (X1MB) now detonates reliably: a held manual key is explicit intent, so any ready keg is blown regardless of nearby enemies.
- Two intermittent E-Q-E (G) issues are fixed: the first keg now drops even while Q is cooling (Q returns during the decay wait), and the second keg no longer randomly disappears when it left on the same tick as the Q - it is cast directly past the per-tick guard.
- E-Q-E (G) is now distance-adaptive: inside E-Q-E reach it plays two kegs, and beyond that - with three charges banked - it automatically runs the three-keg E-Q-E-E chain. The first keg always sits a whole number of links short of the target so the LAST keg lands exactly on them, and the third keg follows on the official 0.5-second between-barrels clock even if the key is released.
- Fixed the combo target scan being capped at Q/E range (1000): a READY keg at your feet chains to enemies up to roughly 2400 away, but such enemies produced no action at all. The scan now covers the real keg-play reach.
- Added the basic-attack trigger chain: a ready keg inside attack range is detonated with an auto (saving the Q) and the follow-up kegs ride the fuse the moment the attack fires; kegs out of attack reach keep the Q trigger.
- Combo direct Q on champions is now execute-only: it fires when one Q kills, or when no keg play is possible at all (no kegs, no charges). The harass poke Q is unchanged.
- Fixed kegs being seated at exactly the link-distance boundary, where they failed to actually connect: every automatic and semi placement now undershoots the slider by 60 units so a boundary error can never break the chain (detection and drawing of existing kegs keep the raw value).
- Fixed the Q lead firing too early: aiming the arrival exactly at the decay-tick boundary made the shot land a few dozen milliseconds before the real tick, shaving the keg to 1 instead of detonating it. The arrival now trails the tick by a built-in 150 ms safety margin (plus the slider), and the basic-attack detonation only goes when the observed health already reads 1.
- Added the automatic teamfight R (default on): the barrage is global, so every enemy is a candidate zone center and it fires at the best spot reliably holding the configured head-count (default 3, adjustable). With the accuracy option on, only enemies that cannot walk out during the 0.5-second cast are counted.
- The semi barrel (X1MB) now places at maximum reach toward the mouse instead of at the mouse: a full link from the keg nearest the mouse when one exists, else the farthest point a direct Q can still trigger (short placements were wasted).

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.10.2。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
- Q 尾刀现在对野怪也生效（此前未扫描中立列表，只有兵线可用）。优先级：可击杀的炮车/超级兵永远优先，其余按血量最低的小兵；自己的火药桶不会被当作尾刀目标。
- 三桶选项（默认开启）：连招中最多连接三个火药桶来延伸距离。
- 自动连招的桶链改为 E-Q-E 方式（用户教义）：旧的预放第二桶（E-E-Q）容易被敌人打掉或躲开，现在只要就绪的桶在距目标一到两个连接距离内就立即用 Q 引爆，后续桶在 Q 与引信飞行期间按目标实时位置接上（目标移动时自然形成斜线连接）。
- 起手桶位置可用 N 键实时切换（己方侧 / 敌方侧，状态栏显示 EnemySide）。菜单下拉为默认值，切换键将其反转。
- 半自动放桶（X1MB）现在稳定引爆：按住手动键即明确意图，只要有就绪的桶就立刻引爆，无论附近有无敌人。
- 修复了 E-Q-E（G）的两个间歇性问题：Q 冷却中也会先放第一个桶（等待期间 Q 会转好）；与 Q 同一帧发出的第二个桶不再被内部帧保护随机吞掉，改为直接施放。
- E-Q-E（G）现在按距离自适应：目标在 E-Q-E 射程内时使用两个桶；更远且备有三层充能时，自动执行三桶的 E-Q-E-E 连锁。第一个桶始终放在距目标整数个连接距离之后，使最后一个桶正好落在目标身上；第三个桶按官方 0.5 秒放桶间隔自动接上，即使松开按键也会完成。
- 修复了连招目标扫描被限制在 Q/E 射程（1000）的问题：脚下就绪的桶实际可连锁到约 2400 外的敌人，但此前对这些敌人毫无动作。现在扫描覆盖真实的桶链可达距离。
- 新增普攻引爆连锁：就绪的桶在普攻距离内时用普攻引爆（节省 Q），攻击出手的瞬间后续桶沿引信接上；桶在普攻距离外时仍用 Q 触发。
- 连招中对英雄的直接 Q 现在仅用于处决：只有一发 Q 能击杀、或完全无法进行桶连招（无桶无充能）时才施放。骚扰消耗 Q 不变。
- 修复了火药桶恰好放在连接距离滑条边界值上而实际无法连接的问题：所有自动/半自动放置现在比滑条值收进 60 单位，使边界误差不再断链（对已存在桶的检测与绘制仍使用原值）。
- 修复了 Q 提前引爆过早的问题：此前瞄准衰减刻度边界的精确时刻，导致弹丸比真实刻度早几十毫秒到达，只把桶削到 1 而没有引爆。现在到达时刻会滞后刻度一个内置 150 毫秒安全余量（加滑条附加值），普攻引爆只在观测血量已为 1 时进行。
- 新增自动团战 R（默认开启）：大招为全图施放，因此以每个敌人为候选中心，在可靠容纳设定人数（默认 3 人，可调）的最佳位置自动施放。开启命中可靠性选项时，只统计在 0.5 秒施法期间走不出范围的敌人。
- 半自动放桶（X1MB）改为朝鼠标方向的最大距离放置而非鼠标位置：已有桶时从离鼠标最近的桶延伸一个完整连接距离，否则放在 Q 能直接触发的最远处（修复近距离浪费）。
<!-- MESH-AIO:RELEASE:v2.10.2:END -->

<!-- MESH-AIO:RELEASE:v2.10.1:START -->
## v2.10.1

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.10.1. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.
- Q 막타가 정글 몬스터에도 동작합니다(중립 목록을 스캔하지 않아 라인에서만 되던 문제 수정). 막타 우선순위는 처치 가능한 대포·슈퍼 미니언 최우선, 그 외에는 체력이 가장 낮은 미니언 순입니다. 자기 화약통은 막타 대상에서 제외됩니다.
- 트리플 배럴 옵션(기본 켜짐): 콤보에서 화약통을 최대 3개까지 연계해 사거리를 늘립니다.
- 자동 콤보의 사슬이 E-Q-E 방식으로 바뀌었습니다(사용자 교리): 미리 둘째 통을 까는 기존 E-E-Q는 적이 통을 부수거나 피하기 쉬워, 이제 준비된 통이 연결 거리 1~2개 안에 대상을 두면 즉시 Q로 격발하고 후속 통들은 Q·퓨즈가 날아가는 동안 실시간 대상 위치로 이어집니다(대상이 움직이면 자연스럽게 사선 연결).
- 시작 통 위치를 N 키로 실시간 전환할 수 있습니다(내 쪽 / 상대 쪽, 상태줄에 EnemySide로 표시). 메뉴 드롭다운은 기본값이고 토글이 뒤집습니다.
- 세미 통(X1MB)이 이제 안정적으로 격발합니다: 수동 키는 명시적 의도이므로 준비된 통이면 주변 적 여부와 무관하게 즉시 터뜨립니다.
- E-Q-E(G)의 간헐 동작 두 가지를 고쳤습니다: Q가 쿨다운이어도 첫 통을 미리 깔고(대기 중 Q가 돌아옴), Q 격발과 같은 틱에 나가는 두 번째 통이 내부 틱 가드에 먹혀 무작위로 빠지던 문제를 직접 시전으로 해결했습니다.
- E-Q-E(G)는 거리 적응형이 되었습니다: 대상이 E-Q-E 사거리면 두 통으로, 그보다 멀고 충전이 3개 있으면 자동으로 E-Q-E-E 세 통 체인으로 실행합니다. 첫 통은 항상 연결 거리의 정수 배만큼 대상 뒤에 깔려 마지막 통이 대상 정중앙에 떨어지고, 세 번째 통은 공식 0.5초 설치 간격에 맞춰 키를 떼도 자동으로 이어집니다.
- 화약통 설치 간격이 연결 거리 슬라이더의 경계값 그대로여서 실제로는 이어지지 않던 문제를 고쳤습니다: 모든 자동/세미 배치는 이제 슬라이더보다 60유닛 안쪽으로 깔려 경계 오차로 사슬이 끊기지 않습니다(기존 통 감지·표시는 슬라이더 값 그대로).
- Q 리드 격발이 너무 일찍 나가 통을 터뜨리지 못하고 체력만 깎던 버그를 고쳤습니다: 감소 틱 경계 정각에 도착하도록 쏘던 것을, 내장 150ms 안전 여유(+ 슬라이더 추가분)만큼 틱이 지난 뒤 도착하도록 바꿨습니다. 평타 격발은 관측 체력이 1일 때만 나갑니다.
- 자동 한타 R를 추가했습니다(기본 켜짐): 궁은 글로벌이므로 모든 적을 후보 중심으로 보고, 설정한 인원(기본 3명, 조절 가능)이 525 충격파 안에 확실히 들어오는 최적 지점에 자동 시전합니다. 명중 신뢰도 옵션을 켜면 0.5초 시전 동안 걸어 나갈 수 없는 적만 셉니다.
- 세미 통(X1MB)은 마우스 위치가 아니라 마우스 방향 최대 거리에 설치합니다: 기존 통이 있으면 그 통에서 연결 거리 최대로 연장하고, 없으면 Q가 직접 닿는 최대 거리에 깝니다(짧은 거리 낭비 수정).

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.10.1. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.
- The Q last hit now also works on jungle monsters (the neutral list was not scanned, so only lane worked). Priority: a killable cannon/super minion always first, then the lowest-health minion; our own kegs are excluded as targets.
- Triple barrel option (default on): Combo chains up to three kegs for range.
- The automatic combo chain now plays E-Q-E (user doctrine): the old pre-placed second keg (E-E-Q) was visible and got broken or dodged, so a ready keg within one or two links of the target is Q-detonated immediately and the follow-up kegs land while the Q and fuse are already in the air, aimed at the target's live position (naturally diagonal when they move).
- The opening barrel side flips in real time on N (my side / enemy side, shown as EnemySide in the status list). The menu dropdown is the default and the toggle inverts it.
- The semi barrel (X1MB) now detonates reliably: a held manual key is explicit intent, so any ready keg is blown regardless of nearby enemies.
- Two intermittent E-Q-E (G) issues are fixed: the first keg now drops even while Q is cooling (Q returns during the decay wait), and the second keg no longer randomly disappears when it left on the same tick as the Q - it is cast directly past the per-tick guard.
- E-Q-E (G) is now distance-adaptive: inside E-Q-E reach it plays two kegs, and beyond that - with three charges banked - it automatically runs the three-keg E-Q-E-E chain. The first keg always sits a whole number of links short of the target so the LAST keg lands exactly on them, and the third keg follows on the official 0.5-second between-barrels clock even if the key is released.
- Fixed kegs being seated at exactly the link-distance boundary, where they failed to actually connect: every automatic and semi placement now undershoots the slider by 60 units so a boundary error can never break the chain (detection and drawing of existing kegs keep the raw value).
- Fixed the Q lead firing too early: aiming the arrival exactly at the decay-tick boundary made the shot land a few dozen milliseconds before the real tick, shaving the keg to 1 instead of detonating it. The arrival now trails the tick by a built-in 150 ms safety margin (plus the slider), and the basic-attack detonation only goes when the observed health already reads 1.
- Added the automatic teamfight R (default on): the barrage is global, so every enemy is a candidate zone center and it fires at the best spot reliably holding the configured head-count (default 3, adjustable). With the accuracy option on, only enemies that cannot walk out during the 0.5-second cast are counted.
- The semi barrel (X1MB) now places at maximum reach toward the mouse instead of at the mouse: a full link from the keg nearest the mouse when one exists, else the farthest point a direct Q can still trigger (short placements were wasted).

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.10.1。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
- Q 尾刀现在对野怪也生效（此前未扫描中立列表，只有兵线可用）。优先级：可击杀的炮车/超级兵永远优先，其余按血量最低的小兵；自己的火药桶不会被当作尾刀目标。
- 三桶选项（默认开启）：连招中最多连接三个火药桶来延伸距离。
- 自动连招的桶链改为 E-Q-E 方式（用户教义）：旧的预放第二桶（E-E-Q）容易被敌人打掉或躲开，现在只要就绪的桶在距目标一到两个连接距离内就立即用 Q 引爆，后续桶在 Q 与引信飞行期间按目标实时位置接上（目标移动时自然形成斜线连接）。
- 起手桶位置可用 N 键实时切换（己方侧 / 敌方侧，状态栏显示 EnemySide）。菜单下拉为默认值，切换键将其反转。
- 半自动放桶（X1MB）现在稳定引爆：按住手动键即明确意图，只要有就绪的桶就立刻引爆，无论附近有无敌人。
- 修复了 E-Q-E（G）的两个间歇性问题：Q 冷却中也会先放第一个桶（等待期间 Q 会转好）；与 Q 同一帧发出的第二个桶不再被内部帧保护随机吞掉，改为直接施放。
- E-Q-E（G）现在按距离自适应：目标在 E-Q-E 射程内时使用两个桶；更远且备有三层充能时，自动执行三桶的 E-Q-E-E 连锁。第一个桶始终放在距目标整数个连接距离之后，使最后一个桶正好落在目标身上；第三个桶按官方 0.5 秒放桶间隔自动接上，即使松开按键也会完成。
- 修复了火药桶恰好放在连接距离滑条边界值上而实际无法连接的问题：所有自动/半自动放置现在比滑条值收进 60 单位，使边界误差不再断链（对已存在桶的检测与绘制仍使用原值）。
- 修复了 Q 提前引爆过早的问题：此前瞄准衰减刻度边界的精确时刻，导致弹丸比真实刻度早几十毫秒到达，只把桶削到 1 而没有引爆。现在到达时刻会滞后刻度一个内置 150 毫秒安全余量（加滑条附加值），普攻引爆只在观测血量已为 1 时进行。
- 新增自动团战 R（默认开启）：大招为全图施放，因此以每个敌人为候选中心，在可靠容纳设定人数（默认 3 人，可调）的最佳位置自动施放。开启命中可靠性选项时，只统计在 0.5 秒施法期间走不出范围的敌人。
- 半自动放桶（X1MB）改为朝鼠标方向的最大距离放置而非鼠标位置：已有桶时从离鼠标最近的桶延伸一个完整连接距离，否则放在 Q 能直接触发的最远处（修复近距离浪费）。
<!-- MESH-AIO:RELEASE:v2.10.1:END -->

<!-- MESH-AIO:RELEASE:v2.10.0:START -->
## v2.10.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.10.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.
- Q 막타가 정글 몬스터에도 동작합니다(중립 목록을 스캔하지 않아 라인에서만 되던 문제 수정). 막타 우선순위는 처치 가능한 대포·슈퍼 미니언 최우선, 그 외에는 체력이 가장 낮은 미니언 순입니다. 자기 화약통은 막타 대상에서 제외됩니다.
- 트리플 배럴 옵션(기본 켜짐): 콤보에서 화약통을 최대 3개까지 연계해 사거리를 늘립니다.
- 자동 콤보의 사슬이 E-Q-E 방식으로 바뀌었습니다(사용자 교리): 미리 둘째 통을 까는 기존 E-E-Q는 적이 통을 부수거나 피하기 쉬워, 이제 준비된 통이 연결 거리 1~2개 안에 대상을 두면 즉시 Q로 격발하고 후속 통들은 Q·퓨즈가 날아가는 동안 실시간 대상 위치로 이어집니다(대상이 움직이면 자연스럽게 사선 연결).
- 시작 통 위치를 N 키로 실시간 전환할 수 있습니다(내 쪽 / 상대 쪽, 상태줄에 EnemySide로 표시). 메뉴 드롭다운은 기본값이고 토글이 뒤집습니다.
- 세미 통(X1MB)이 이제 안정적으로 격발합니다: 수동 키는 명시적 의도이므로 준비된 통이면 주변 적 여부와 무관하게 즉시 터뜨립니다.
- E-Q-E(G)의 간헐 동작 두 가지를 고쳤습니다: Q가 쿨다운이어도 첫 통을 미리 깔고(대기 중 Q가 돌아옴), Q 격발과 같은 틱에 나가는 두 번째 통이 내부 틱 가드에 먹혀 무작위로 빠지던 문제를 직접 시전으로 해결했습니다.
- E-Q-E(G)는 거리 적응형이 되었습니다: 대상이 E-Q-E 사거리면 두 통으로, 그보다 멀고 충전이 3개 있으면 자동으로 E-Q-E-E 세 통 체인으로 실행합니다. 첫 통은 항상 연결 거리의 정수 배만큼 대상 뒤에 깔려 마지막 통이 대상 정중앙에 떨어지고, 세 번째 통은 공식 0.5초 설치 간격에 맞춰 키를 떼도 자동으로 이어집니다.
- 자동 한타 R를 추가했습니다(기본 켜짐): 궁은 글로벌이므로 모든 적을 후보 중심으로 보고, 설정한 인원(기본 3명, 조절 가능)이 525 충격파 안에 확실히 들어오는 최적 지점에 자동 시전합니다. 명중 신뢰도 옵션을 켜면 0.5초 시전 동안 걸어 나갈 수 없는 적만 셉니다.
- 세미 통(X1MB)은 마우스 위치가 아니라 마우스 방향 최대 거리에 설치합니다: 기존 통이 있으면 그 통에서 연결 거리 최대로 연장하고, 없으면 Q가 직접 닿는 최대 거리에 깝니다(짧은 거리 낭비 수정).

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.10.0. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.
- The Q last hit now also works on jungle monsters (the neutral list was not scanned, so only lane worked). Priority: a killable cannon/super minion always first, then the lowest-health minion; our own kegs are excluded as targets.
- Triple barrel option (default on): Combo chains up to three kegs for range.
- The automatic combo chain now plays E-Q-E (user doctrine): the old pre-placed second keg (E-E-Q) was visible and got broken or dodged, so a ready keg within one or two links of the target is Q-detonated immediately and the follow-up kegs land while the Q and fuse are already in the air, aimed at the target's live position (naturally diagonal when they move).
- The opening barrel side flips in real time on N (my side / enemy side, shown as EnemySide in the status list). The menu dropdown is the default and the toggle inverts it.
- The semi barrel (X1MB) now detonates reliably: a held manual key is explicit intent, so any ready keg is blown regardless of nearby enemies.
- Two intermittent E-Q-E (G) issues are fixed: the first keg now drops even while Q is cooling (Q returns during the decay wait), and the second keg no longer randomly disappears when it left on the same tick as the Q - it is cast directly past the per-tick guard.
- E-Q-E (G) is now distance-adaptive: inside E-Q-E reach it plays two kegs, and beyond that - with three charges banked - it automatically runs the three-keg E-Q-E-E chain. The first keg always sits a whole number of links short of the target so the LAST keg lands exactly on them, and the third keg follows on the official 0.5-second between-barrels clock even if the key is released.
- Added the automatic teamfight R (default on): the barrage is global, so every enemy is a candidate zone center and it fires at the best spot reliably holding the configured head-count (default 3, adjustable). With the accuracy option on, only enemies that cannot walk out during the 0.5-second cast are counted.
- The semi barrel (X1MB) now places at maximum reach toward the mouse instead of at the mouse: a full link from the keg nearest the mouse when one exists, else the farthest point a direct Q can still trigger (short placements were wasted).

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.10.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
- Q 尾刀现在对野怪也生效（此前未扫描中立列表，只有兵线可用）。优先级：可击杀的炮车/超级兵永远优先，其余按血量最低的小兵；自己的火药桶不会被当作尾刀目标。
- 三桶选项（默认开启）：连招中最多连接三个火药桶来延伸距离。
- 自动连招的桶链改为 E-Q-E 方式（用户教义）：旧的预放第二桶（E-E-Q）容易被敌人打掉或躲开，现在只要就绪的桶在距目标一到两个连接距离内就立即用 Q 引爆，后续桶在 Q 与引信飞行期间按目标实时位置接上（目标移动时自然形成斜线连接）。
- 起手桶位置可用 N 键实时切换（己方侧 / 敌方侧，状态栏显示 EnemySide）。菜单下拉为默认值，切换键将其反转。
- 半自动放桶（X1MB）现在稳定引爆：按住手动键即明确意图，只要有就绪的桶就立刻引爆，无论附近有无敌人。
- 修复了 E-Q-E（G）的两个间歇性问题：Q 冷却中也会先放第一个桶（等待期间 Q 会转好）；与 Q 同一帧发出的第二个桶不再被内部帧保护随机吞掉，改为直接施放。
- E-Q-E（G）现在按距离自适应：目标在 E-Q-E 射程内时使用两个桶；更远且备有三层充能时，自动执行三桶的 E-Q-E-E 连锁。第一个桶始终放在距目标整数个连接距离之后，使最后一个桶正好落在目标身上；第三个桶按官方 0.5 秒放桶间隔自动接上，即使松开按键也会完成。
- 新增自动团战 R（默认开启）：大招为全图施放，因此以每个敌人为候选中心，在可靠容纳设定人数（默认 3 人，可调）的最佳位置自动施放。开启命中可靠性选项时，只统计在 0.5 秒施法期间走不出范围的敌人。
- 半自动放桶（X1MB）改为朝鼠标方向的最大距离放置而非鼠标位置：已有桶时从离鼠标最近的桶延伸一个完整连接距离，否则放在 Q 能直接触发的最远处（修复近距离浪费）。
<!-- MESH-AIO:RELEASE:v2.10.0:END -->

<!-- MESH-AIO:RELEASE:v2.9.0:START -->
## v2.9.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.9.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.
- Q 막타가 정글 몬스터에도 동작합니다(중립 목록을 스캔하지 않아 라인에서만 되던 문제 수정). 막타 우선순위는 처치 가능한 대포·슈퍼 미니언 최우선, 그 외에는 체력이 가장 낮은 미니언 순입니다. 자기 화약통은 막타 대상에서 제외됩니다.
- 트리플 배럴 옵션(기본 켜짐): 콤보에서 화약통을 최대 3개까지 연계해 사거리를 늘립니다.
- 자동 콤보의 사슬이 E-Q-E 방식으로 바뀌었습니다(사용자 교리): 미리 둘째 통을 까는 기존 E-E-Q는 적이 통을 부수거나 피하기 쉬워, 이제 준비된 통이 연결 거리 1~2개 안에 대상을 두면 즉시 Q로 격발하고 후속 통들은 Q·퓨즈가 날아가는 동안 실시간 대상 위치로 이어집니다(대상이 움직이면 자연스럽게 사선 연결).
- 시작 통 위치를 N 키로 실시간 전환할 수 있습니다(내 쪽 / 상대 쪽, 상태줄에 EnemySide로 표시). 메뉴 드롭다운은 기본값이고 토글이 뒤집습니다.
- 세미 통(X1MB)이 이제 안정적으로 격발합니다: 수동 키는 명시적 의도이므로 준비된 통이면 주변 적 여부와 무관하게 즉시 터뜨립니다.
- E-Q-E(G)의 간헐 동작 두 가지를 고쳤습니다: Q가 쿨다운이어도 첫 통을 미리 깔고(대기 중 Q가 돌아옴), Q 격발과 같은 틱에 나가는 두 번째 통이 내부 틱 가드에 먹혀 무작위로 빠지던 문제를 직접 시전으로 해결했습니다.
- E-Q-E(G)는 거리 적응형이 되었습니다: 대상이 E-Q-E 사거리면 두 통으로, 그보다 멀고 충전이 3개 있으면 자동으로 E-Q-E-E 세 통 체인으로 실행합니다. 첫 통은 항상 연결 거리의 정수 배만큼 대상 뒤에 깔려 마지막 통이 대상 정중앙에 떨어지고, 세 번째 통은 공식 0.5초 설치 간격에 맞춰 키를 떼도 자동으로 이어집니다.
- 세미 통(X1MB)은 마우스 위치가 아니라 마우스 방향 최대 거리에 설치합니다: 기존 통이 있으면 그 통에서 연결 거리 최대로 연장하고, 없으면 Q가 직접 닿는 최대 거리에 깝니다(짧은 거리 낭비 수정).

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.9.0. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.
- The Q last hit now also works on jungle monsters (the neutral list was not scanned, so only lane worked). Priority: a killable cannon/super minion always first, then the lowest-health minion; our own kegs are excluded as targets.
- Triple barrel option (default on): Combo chains up to three kegs for range.
- The automatic combo chain now plays E-Q-E (user doctrine): the old pre-placed second keg (E-E-Q) was visible and got broken or dodged, so a ready keg within one or two links of the target is Q-detonated immediately and the follow-up kegs land while the Q and fuse are already in the air, aimed at the target's live position (naturally diagonal when they move).
- The opening barrel side flips in real time on N (my side / enemy side, shown as EnemySide in the status list). The menu dropdown is the default and the toggle inverts it.
- The semi barrel (X1MB) now detonates reliably: a held manual key is explicit intent, so any ready keg is blown regardless of nearby enemies.
- Two intermittent E-Q-E (G) issues are fixed: the first keg now drops even while Q is cooling (Q returns during the decay wait), and the second keg no longer randomly disappears when it left on the same tick as the Q - it is cast directly past the per-tick guard.
- E-Q-E (G) is now distance-adaptive: inside E-Q-E reach it plays two kegs, and beyond that - with three charges banked - it automatically runs the three-keg E-Q-E-E chain. The first keg always sits a whole number of links short of the target so the LAST keg lands exactly on them, and the third keg follows on the official 0.5-second between-barrels clock even if the key is released.
- The semi barrel (X1MB) now places at maximum reach toward the mouse instead of at the mouse: a full link from the keg nearest the mouse when one exists, else the farthest point a direct Q can still trigger (short placements were wasted).

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.9.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
- Q 尾刀现在对野怪也生效（此前未扫描中立列表，只有兵线可用）。优先级：可击杀的炮车/超级兵永远优先，其余按血量最低的小兵；自己的火药桶不会被当作尾刀目标。
- 三桶选项（默认开启）：连招中最多连接三个火药桶来延伸距离。
- 自动连招的桶链改为 E-Q-E 方式（用户教义）：旧的预放第二桶（E-E-Q）容易被敌人打掉或躲开，现在只要就绪的桶在距目标一到两个连接距离内就立即用 Q 引爆，后续桶在 Q 与引信飞行期间按目标实时位置接上（目标移动时自然形成斜线连接）。
- 起手桶位置可用 N 键实时切换（己方侧 / 敌方侧，状态栏显示 EnemySide）。菜单下拉为默认值，切换键将其反转。
- 半自动放桶（X1MB）现在稳定引爆：按住手动键即明确意图，只要有就绪的桶就立刻引爆，无论附近有无敌人。
- 修复了 E-Q-E（G）的两个间歇性问题：Q 冷却中也会先放第一个桶（等待期间 Q 会转好）；与 Q 同一帧发出的第二个桶不再被内部帧保护随机吞掉，改为直接施放。
- E-Q-E（G）现在按距离自适应：目标在 E-Q-E 射程内时使用两个桶；更远且备有三层充能时，自动执行三桶的 E-Q-E-E 连锁。第一个桶始终放在距目标整数个连接距离之后，使最后一个桶正好落在目标身上；第三个桶按官方 0.5 秒放桶间隔自动接上，即使松开按键也会完成。
- 半自动放桶（X1MB）改为朝鼠标方向的最大距离放置而非鼠标位置：已有桶时从离鼠标最近的桶延伸一个完整连接距离，否则放在 Q 能直接触发的最远处（修复近距离浪费）。
<!-- MESH-AIO:RELEASE:v2.9.0:END -->

<!-- MESH-AIO:RELEASE:v2.8.2:START -->
## v2.8.2

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.8.2. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.8.2. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.8.2。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
<!-- MESH-AIO:RELEASE:v2.8.2:END -->

<!-- MESH-AIO:RELEASE:v2.8.1:START -->
## v2.8.1

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.8.1. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.8.1. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.8.1。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
<!-- MESH-AIO:RELEASE:v2.8.1:END -->

<!-- MESH-AIO:RELEASE:v2.8.0:START -->
## v2.8.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.8.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 21개에서 22개로 늘었고(갱플랭크 추가) 나머지 151챔피언은 공용 엔진을 사용합니다.
- 공식 수치 회귀 계약을 16개 추가해 총 504개가 되었습니다. 갱플랭크의 스킬 수치·반경·화약통 감소 주기가 공식 원본과 어긋나면 빌드 전에 검사에서 걸립니다.

#### Gangplank

- 전용 모듈로 승격했습니다. 핵심은 화약통 추적기입니다: 아군 오브젝트에서 통을 찾아 체력 변화 시각을 기록하고, 공식 감소 주기 표(2초 → 7레벨 1초 → 13레벨 0.5초)로 미래 시점의 체력을 예측합니다. 격발은 Q가 실제로 도착하는 순간(시전 프레임 + 공식 2600 투사체 속도) 통이 체력 1일 때만 시도하며 보정 슬라이더를 제공합니다.
- 통 사슬은 연결 거리 슬라이더(기본 660, 공식 캐시에 없는 값이라 인게임 확정 대상)로 그래프 탐색해 계산하고, 폭발 적중은 공식 325 반경의 안쪽 여유 또는 경직 관통만 인정합니다. 콤보 순서는 준비된 사슬 격발 → 적이 통을 깨기 직전의 선제 격발 → 대상 쪽으로 사슬 연장 또는 명중 신뢰도를 통과한 새 통 설치 → 일반 Q이며, 통 우선 토글을 끄면 일반 Q가 먼저 나갑니다.
- 사용자 콤보 가이드의 13레벨 장거리 E-Q-E를 G 키에 담았습니다: 마우스 대상 쪽 끝 사거리에 첫 통을 깔고, 준비되는 순간 Q를 쏘며, Q가 떠나는 즉시 두 번째 통이 사슬로 이어집니다. X1MB는 마우스 방향 반자동 통 설치+격발입니다.
- W는 경직 클렌즈(둔화는 옵션)와 저체력 힐, R는 Space 세미(마우스 근처 최다 적 지점)와 기본 꺼짐인 처치 자동 R(계산 웨이브 수 슬라이더)를 제공합니다. 킬스틸은 처치 가능한 사슬 격발을 최우선으로 시도합니다.
- 팜은 약탈 골드를 위한 Q 막타(처치 확정일 때만), N마리 이상을 덮는 사슬 격발, 선택형 라인 통 설치를 제공합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.8.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 21 to 22 with Gangplank; the remaining 151 champions use the shared engine.
- Added 16 official-number regression contracts, bringing the total to 504, so any drift between Gangplank's numbers, radii, or the barrel decay table and the official source fails the check before a build.

#### Gangplank

- Promoted to a hand-tuned module. The heart is the powder-keg tracker: barrels are found among ally objects, every health change is timestamped, and future health is predicted from the official decay table (2 s, 1 s at level 7, 0.5 s at level 13). A detonation is attempted only when the keg will read 1 health at the moment the Q actually arrives (cast frame plus the official 2600 missile speed), with a timing-correction slider.
- Chains are computed as a graph walk over the link-distance slider (default 660; not an official cache field, so it awaits in-game confirmation), and chain hits count only enemies inside the official 325 radius with an inner margin or locked by CC through the blast. Combo order: detonate a ready covering chain, pre-empt an enemy about to break a keg, extend a chain toward the target or place a fresh reliability-gated keg, then plain Q - and the barrel-first toggle can put plain Q ahead.
- The user guide's level-13 long E-Q-E lives on G: a far keg toward the mouse target, Q the instant it reads ready, and the second keg chains on as the Q leaves. X1MB is the semi barrel toward the mouse with auto detonation.
- W cleanses hard CC (slows optional) and heals at low HP; R is Semi Space at the densest cluster near the mouse plus a default-off lethal auto-R with a configurable wave count. Killsteal detonates a killing chain first.
- Farming offers plunder-gold Q last hits (only when the kill is certain), chain detonations covering N minions, and optional lane kegs.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.8.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 21 个增加到 22 个（新增普朗克），其余 151 位英雄使用共用引擎。
- 新增 16 条官方数值回归约定，总数达到 504 条；普朗克的技能数值、半径或火药桶衰减表与官方原始数据不一致，都会在构建前被检查拦下。

#### Gangplank

- 升级为专属模块。核心是火药桶追踪器：在友方对象中找到火药桶，记录每次生命变化的时间，并按官方衰减表（2 秒 → 7 级 1 秒 → 13 级 0.5 秒）预测未来时刻的生命值。只有当 Q 实际到达的瞬间（施法帧加官方 2600 弹速）桶读数为 1 时才尝试引爆，并提供校正滑条。
- 桶链以连接距离滑条（默认 660；官方缓存中无此字段，待游戏内确认）做图遍历计算，链式命中只统计处于官方 325 半径内侧余量或被控住的敌人。连招顺序：引爆已就绪且覆盖目标的桶链 → 抢在敌人打破桶之前引爆 → 向目标延伸桶链或放置通过命中可靠性判定的新桶 → 普通 Q；关闭“桶优先”开关则普通 Q 提前。
- 用户攻略中的 13 级远程 E-Q-E 绑定在 G 键：朝鼠标目标在极限距离放第一个桶，桶就绪的瞬间 Q，Q 出手的同时第二个桶接上链。X1MB 为朝鼠标方向的半自动放桶加引爆。
- W 解除硬控（减速可选）并在低血量时治疗；R 为 Space 半手动（鼠标附近敌人最密处），另有默认关闭的致命自动 R（可配置计算波数）。击杀补足优先引爆能击杀的桶链。
- 补刀提供掠夺金币的 Q 尾刀（仅在确定击杀时）、覆盖 N 个小兵的桶链引爆，以及可选的清线放桶。
<!-- MESH-AIO:RELEASE:v2.8.0:END -->

<!-- MESH-AIO:RELEASE:v2.7.0:START -->
## v2.7.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.7.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 모듈 21개, 공용 엔진 152개) 지원을 그대로 유지합니다.
- 최근 전용 챔피언들에 도입한 명중 신뢰도·스테이시스 저격 표준을 기존 전용 모듈로 역이식하는 릴리즈입니다. 이번에는 신드라가 대상입니다.

#### Syndra

- 자동 Q와 자동 W 던지기에 공용 명중 신뢰도 판정을 추가했습니다. 이전에는 다중 적중 점수화가 신뢰 가능한 후보를 찾지 못하면 원시 예측 지점에 그대로 시전할 수 있었는데, 이제 대상이 도착 전에 판정을 벗어날 수 없거나, 멈춰 있거나, 경로가 확정된 경우에만 자동으로 발사합니다. 각 스킬에 켜고 끌 수 있는 옵션(기본 켜짐)이며 세미 키·도주·고정 착지(팜)는 이전과 동일하게 즉시 발사합니다.
- 스테이시스 저격을 추가했습니다. 존야·초시계·바드 R·리산드라 자체 R로 얼어 있는 적에게 해제되는 순간 정확히 도착하도록 Q 또는 W 던지기를 미리 시전합니다(각 스킬 옵션, 기본 켜짐). 얼어 있는 동안에는 절대 낭비 시전하지 않습니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.7.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data (21 hand-tuned modules, 152 on the shared engine).
- This release back-ports the hit-reliability and stasis-snipe standards introduced with the recent dedicated champions into an existing dedicated module: Syndra.

#### Syndra

- Automatic Q and automatic W throws now pass the shared hit-reliability gate. Previously, when the multi-hit scorer found no reliable candidate it could fall back to casting at the raw predicted point; now automatic casts fire only when the target cannot leave the shape before impact, is standing still, or is on a confirmed path. Each spell has its own toggle (default on), and semi keys, flee, and fixed farm landings still fire immediately as before.
- Added the stasis snipe: against an enemy frozen by Zhonya's, Stopwatch, Bard R, or Lissandra's self R, a Q or W throw is pre-cast to land exactly as the stasis breaks (per-spell toggles, default on). Nothing is ever wasted into an enemy still frozen.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.7.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（21 个专属模块，152 个使用共用引擎）。
- 本次将近期专属英雄引入的命中可靠性与凝滞狙击标准回移植到既有专属模块：辛德拉。

#### Syndra

- 自动 Q 与自动 W 投掷现在通过共用的命中可靠性判定。此前当多重命中评分找不到可靠候选时，可能退回到直接朝原始预测点施放；现在只有当目标在落点生效前无法离开判定范围、处于静止、或路径已确认时才自动施放。每个技能有独立开关（默认开启），半手动键、逃跑与固定落点（补刀）仍像以前一样立即施放。
- 新增凝滞狙击：对被中娅、秒表、巴德 R 或丽桑卓自身 R 冻结的敌人，预先施放 Q 或 W 投掷，使其在凝滞解除的瞬间精准落地（每技能开关，默认开启）。绝不会浪费在仍处于冻结状态的敌人身上。
<!-- MESH-AIO:RELEASE:v2.7.0:END -->

<!-- MESH-AIO:RELEASE:v2.6.0:START -->
## v2.6.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.6.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 20개에서 21개로 늘었고(오리아나 추가) 나머지 152챔피언은 공용 엔진을 사용합니다.
- 공식 수치 회귀 계약을 24개 추가해 총 488개가 되었습니다. 오리아나의 모든 스킬 수치·사거리·반경이 공식 원본과 어긋나면 빌드 전에 검사에서 걸립니다.

#### Orianna

- 전용 모듈로 승격했습니다. 핵심은 공 위치 추적입니다: 시전 기록으로 상태 기계를 유지하고(직접 시전한 스킬도 포함), Q는 도착 지점에 고정, E는 대상 아군에 부착, 공을 든 아군이 죽으면 그 자리에 남으며, 공식 1500 사거리를 벗어나면 자동으로 회수된 것으로 처리합니다. 공이 아직 날아가는 중에는 W·R처럼 공 주변에 터지는 스킬을 절대 쏘지 않습니다.
- Q는 공이 현재 있는 위치에서의 실제 비행 시간(공식 1400 속도)을 예측에 반영해 조준하고, 명중 신뢰도 판정을 통과할 때만 자동 시전합니다. W는 대상이 공 주변 공식 225 반경 안쪽 여유까지 들어왔을 때만, R는 설정한 수의 적이 0.5초 시전 동안 공식 415 충격파 밖으로 걸어 나갈 수 없을 때만 사용합니다.
- R는 기본적으로 자동 시작하지 않습니다. 콤보에서는 최소 적 수(기본 2) 조건, 별도의 자동 모드(기본 꺼짐)는 더 높은 기준(기본 3)을 요구합니다. 공 근처의 채널링 스킬 인터럽트, 돌진 착지 R(기본 꺼짐), 킬스틸을 제공합니다. G 키는 공을 몸에 붙인 상태에서 가장 많은 적을 덮는 지점으로 점멸한 뒤 즉시 충격파를 터뜨립니다.
- E는 이미 걸린 경직이나 나에게 착지가 확정된 돌진에 반응해 보호막을 씌우고, 체력이 낮은 아군에게도 사용합니다. 세미 E는 마우스에 가까운 아군 또는 자신에게 공을 보냅니다. 도주에서는 E로 공을 회수해 보호막을 받고 W 가속 장판(공식 15~45%)으로 빠져나갑니다.
- 팜은 Q 원을 미니언 무리에 점수화하고, 공이 이미 앉아 있는 곳 주변으로 W를 사용합니다. 정글 최소 적중 기본값은 1이라 단일 캠프에서도 동작합니다. 스테이시스가 풀리는 순간에 정확히 도착하는 Q 저격을 지원합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.6.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 20 to 21 with Orianna; the remaining 152 champions use the shared engine.
- Added 24 official-number regression contracts, bringing the total to 488, so any drift between Orianna's numbers, ranges, or radii and the official source fails the check before a build.

#### Orianna

- Promoted to a hand-tuned module. The heart of it is ball tracking: a cast-driven state machine (your manual casts included) fixes the ball at Q's arrival point, attaches it to the ally E targets, leaves it where a dead carrier stood, and treats it as returned past the official 1500 leash. While the ball is still in flight, nothing that detonates around it will ever fire.
- Q folds the ball's real flight time from wherever it currently is (official 1400 speed) into the prediction and only autocasts through the hit-reliability gate. W fires only when the target is inside the official 225 field around the settled ball with an inner margin, and R only when the configured number of enemies cannot walk out of the official 415 shockwave during its 0.5-second cast.
- R never starts automatically by default: Combo requires the minimum-enemies slider (default 2), the separate Automatic mode (default off) requires its own higher threshold (default 3). Channel interrupts near the ball, an optional dash-landing R, and killsteal are included. The G key, with the ball attached to self, Flashes to the landing covering the most enemies and detonates immediately after.
- E shields against hard CC already landed and dashes committed to land on you, plus low-health allies. Semi E sends the ball to the ally nearest the mouse or back to self. Fleeing recalls the ball with E for the shield and drops W for the official 15-45% haste field.
- Farming scores Q circles over minion groups and uses W around wherever the ball already sits; jungle minimum hits default to 1 so single camps work. A stasis snipe times the Q field to land exactly as stasis breaks.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.6.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 20 个增加到 21 个（新增奥莉安娜），其余 152 位英雄使用共用引擎。
- 新增 24 条官方数值回归约定，总数达到 488 条；奥莉安娜的任何技能数值、射程或半径与官方原始数据不一致，都会在构建前被检查拦下。

#### Orianna

- 升级为专属模块。核心是魔偶（球）位置追踪：以施法记录驱动状态机（包括你手动施放的技能），Q 将球固定在到达点，E 将球附着到目标友军，携带球的友军阵亡时球留在原地，超过官方 1500 距离则视为自动收回。球仍在飞行途中时，绝不会施放任何围绕球引爆的技能。
- Q 会把球从当前位置出发的真实飞行时间（官方 1400 速度）计入预测，并且只有通过命中可靠性判定才自动施放。W 只在目标进入球周围官方 225 范围的内侧余量时使用；R 只在设定数量的敌人无法在 0.5 秒施法期间走出官方 415 冲击波时使用。
- R 默认不自动开启：连招要求最少敌人数（默认 2），独立的自动模式（默认关闭）要求更高阈值（默认 3）。提供球附近的引导打断、突进落点 R（默认关闭）与击杀补足。G 键在球附着于自身时，闪现到能覆盖最多敌人的落点并立即引爆冲击波。
- E 对已命中的硬控和确定落在你身上的突进作出反应施加护盾，也用于低血量友军。半手动 E 将球送往离鼠标最近的友军或收回自身。逃跑时用 E 收回球获得护盾，再用 W 的官方 15-45% 加速场撤离。
- 补刀会在小兵群上为 Q 圆形评分，并围绕球当前所在位置使用 W；打野最少命中数默认为 1，单体营地照常工作。支持在凝滞解除瞬间精准落地的 Q 狙击。
<!-- MESH-AIO:RELEASE:v2.6.0:END -->

<!-- MESH-AIO:RELEASE:v2.5.0:START -->
## v2.5.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.5.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 19개에서 20개로 늘었고(제라스 추가) 나머지 153챔피언은 공용 엔진을 사용합니다.
- 공식 수치 회귀 계약을 33개 추가해 총 464개가 되었습니다. 제라스의 모든 스킬 수치·사거리·형태가 공식 원본과 어긋나면 빌드 전에 검사에서 걸립니다.

#### Xerath

- 전용 모듈로 승격했습니다. Q는 충전 상태 기계로 구현되어 750에서 1500까지 1.5초에 걸쳐 길어지는 광선을 관리합니다. 예측 지점이 사거리 안에 들어오고 명중이 확실해지는 순간 자동으로 발사하며, 3초 충전 만료 직전에는 마나를 날리지 않도록 가장 좋은 지점에 그냥 발사합니다. 광선은 관통하므로 주 대상 명중을 유지한 채 다른 챔피언까지 같이 맞는 각도를 고릅니다. 직접 충전한 Q도 이어받아 예측 발사를 도와줍니다. 충전 중에는 자신이 느려지므로 도주에서는 Q를 쓰지 않습니다.
- W는 공식 수치대로 클릭 0.75초 뒤에 떨어지는 외곽 250·중심 100 원입니다. 도착까지 경직인 대상은 정중앙(1.667배 중심 적중)을 클릭하고, 그 외에는 명중 신뢰도 판정을 통과할 때만 자동으로 씁니다. 경직 대상 자동 W, 나에게 들어오는 돌진 착지점 자동 W, 하레스 마나 하한을 제공합니다.
- E는 조준을 1050으로 제한해 실제 투사체 사거리 1125와의 여유 75를 확보합니다. 채널링 스킬 인터럽트(텔레포트는 기본 제외), 돌진 대응, 스테이시스 해제 순간 기절 저격에 연결됩니다. 세미 E는 E 키를 누르는 동안 매 틱 재시도하고, G 키는 E 사거리 밖 최대 400까지 E를 시전한 뒤 시전 동작 중에 점멸해 착지점에서 발사합니다.
- R는 절대 자동으로 시작하지 않습니다. Space 세미 키로만 10초 채널을 열고, 채널 중에는 이동·공격을 자동으로 멈춥니다(직접 이동 명령은 그대로 통과되어 원할 때 끊을 수 있습니다). 랭크별 4/5/6발을 공식 0.6초 최소 간격으로 관리하며, 한 발에 처치되는 적은 키 없이 자동 발사하고 그 외에는 Space를 누르는 동안 마우스에 가장 가까운 적에게 쏩니다. 남은 발수는 챔피언 위에 표시되고 수동으로 쏜 발까지 정확히 셉니다.
- 팜은 W 착지점을 미니언 무리에 점수화해 고르고, Q는 최소 적중 수를 이미 지나는 사선이 있을 때만 충전을 시작해 사거리가 닿는 즉시 발사합니다. 정글 최소 적중 기본값은 1이라 단일 캠프에서도 그대로 동작합니다. 킬스틸은 W → E → Q 순서로 시도합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.5.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 19 to 20 with Xerath; the remaining 153 champions use the shared engine.
- Added 33 official-number regression contracts, bringing the total to 464, so any drift between Xerath's numbers, ranges, or shapes and the official source fails the check before a build.

#### Xerath

- Promoted to a hand-tuned module. Q runs as a charge state machine managing the beam that grows from 750 to 1500 over 1.5 seconds: it releases the moment a predicted point is both reachable and confirmed to hit, and right before the 3-second expiry it dumps the beam at the best available point rather than wasting the mana. The beam pierces, so the aim ray also picks up other champions without ever costing the primary hit, and a manually started charge is adopted and released with prediction too. Q is never used while fleeing, since charging slows Xerath himself.
- W lands 0.75 seconds after the click per the official numbers, with the 250 outer and 100 sweet-spot circles. A target locked down through the arrival is clicked dead centre for the 1.667x sweet spot; everything else fires only through the hit-reliability gate. Auto W covers hard-CCed targets and the fixed landing of dashes aimed at you, and harass W has its own mana floor.
- E aims within 1050 while the missile actually travels 1125, keeping 75 units of margin. It interrupts channels (Teleport excluded by default), answers gapclosers, and snipes the wake-up stun as stasis ends. Semi E retries every tick while the E key is held, and G casts E at targets up to 400 beyond E range then Flashes inside the windup so the missile leaves from the Flash landing.
- R never starts automatically. Only the Space semi key opens the 10-second channel; movement and attacks pause automatically during it (your own move orders still pass, so you can cancel at will). The 4/5/6 shots per rank respect the official 0.6-second minimum interval: an enemy killable by one shot is fired at with no key held, everything else follows the mouse while Space is held. The shots-left counter is drawn over the champion and stays correct even for shots you fire by hand.
- Farming scores W landings over minion groups and starts a Q charge only when a line already crossing the minimum hits exists, releasing the moment the charged length covers it. Jungle minimum hits default to 1 so single camps work. Killsteal tries W, then E, then a kill-mode Q charge.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.5.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 19 个增加到 20 个（新增泽拉斯），其余 153 位英雄使用共用引擎。
- 新增 33 条官方数值回归约定，总数达到 464 条；泽拉斯的任何技能数值、射程或形状与官方原始数据不一致，都会在构建前被检查拦下。

#### Xerath

- 升级为专属模块。Q 以充能状态机实现，管理在 1.5 秒内从 750 增长到 1500 的光束：当预测点进入射程且命中得到确认的瞬间自动发射，在 3 秒充能到期前会在最佳可用位置直接发射而不浪费法力。光束可以穿透，因此瞄准射线会在保证主目标命中的前提下顺带覆盖其他英雄；玩家手动开始的充能也会被接管并以预测发射。逃跑时绝不使用 Q，因为充能会减速泽拉斯自己。
- W 按官方数值在点击后 0.75 秒落地，外圈 250、甜点区 100。到落地前被控住的目标直接点击正中心（1.667 倍甜点伤害），其余情况只有通过命中可靠性判定才会自动施放。提供受控目标自动 W、朝向自己的突进落点自动 W，以及骚扰的法力下限。
- E 的瞄准限制在 1050，而飞行物实际射程 1125，保留 75 的余量。它用于打断引导（默认不含传送）、应对突进，以及在凝滞（中娅等）解除瞬间的眩晕狙击。按住 E 键的半手动模式每帧重试；G 键可对 E 射程外最多 400 的目标先施放 E，再在前摇中闪现，使飞行物从闪现落点射出。
- R 绝不自动开启。只有 Space 半手动键才会开启 10 秒引导；引导期间自动暂停移动与攻击（你自己的移动指令仍会通过，可随时取消）。每级 4/5/6 发遵守官方 0.6 秒最小间隔：一发可击杀的敌人无需按键自动射击，其余在按住 Space 时射向离鼠标最近的敌人。剩余发数显示在英雄上方，即使手动开火也能准确计数。
- 补刀会在小兵群上为 W 落点评分，Q 只在已存在穿过最少命中数的直线时才开始充能，并在充能长度覆盖时立即发射。打野最少命中数默认为 1，单体营地照常工作。击杀补足按 W → E → Q 的顺序尝试。
<!-- MESH-AIO:RELEASE:v2.5.0:END -->

<!-- MESH-AIO:RELEASE:v2.4.2:START -->
## v2.4.2

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.4.2. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준으로 173챔피언(전용 모듈 19개, 공용 엔진 154개) 지원을 그대로 유지합니다.
- 로크 실측(F12) 기반 수정 릴리즈입니다. 콤보 첫 Q가 안 나가던 문제와 적 챔피언 위 Q 스택 표시 위치를 바로잡았습니다.

#### Locke

- 콤보에서 첫 Q가 나가지 않던 문제를 실제 원인으로 고쳤습니다. 로크 Q는 대기 상태에서 시전이 가능한데도 탄 수가 0으로 읽혀, 스크립트가 첫 발을 "탄 없음"으로 오판하고 쏘지 않았습니다(수동으로 Q를 한 번 쏘기 전까지 자동으로 안 나감). 이제 Q가 시전 가능한 상태면 최소 한 발은 보장해, 수동 선입력 없이도 콤보 첫 Q가 바로 나갑니다.
- 적 챔피언 위에 뜨는 Q 스택 숫자의 위치를 바로잡았습니다. 이전에는 발밑 화면 좌표에서 고정 픽셀만큼 올려 그려서 카메라 줌·해상도가 바뀌면 머리 위를 벗어났습니다. 이제 월드 공간의 머리 위 지점을 화면에 투영해, 줌·해상도와 무관하게 머리에 붙어 따라옵니다. 미세 조정은 그리기 메뉴의 X/Y 오프셋으로 계속 가능합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.4.2. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data (19 hand-tuned modules, 154 on the shared engine).
- An F12-driven Locke fix release: the first combo Q not firing, and the Q-stack number's position over enemy champions, are both corrected.

#### Locke

- Fixed the real cause of the first combo Q not firing. Locke's Q is castable from its resting state even though its ammo reads zero there, so the script misread the first shot as "no ammo" and never threw it (nothing fired automatically until the player cast Q manually once). The ready state is now floored at one charge, so the first combo Q fires immediately with no manual priming.
- Fixed where the Q-stack number is drawn over enemy champions. It used to be lifted a fixed number of pixels from the feet on screen, so it slid off the model whenever the camera zoom or resolution changed. It now projects a point above the head in world space, so it rides the head regardless of zoom or resolution. The Drawings X/Y offsets still fine-tune it.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.4.2。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（19 个专属模块，154 个使用共用引擎）。
- 这是一次基于 F12 实测的洛克修复：修正了连招第一个 Q 不发射，以及敌方英雄头顶 Q 层数的显示位置。

#### Locke

- 修正了连招第一个 Q 不发射的真正原因。洛克的 Q 在待机状态下即可施放，但其弹药读数为零，脚本因此把第一发误判为“没有弹药”而不发射（在玩家手动施放一次 Q 之前，自动不发射）。现在只要 Q 处于可施放状态就至少保证一发，无需手动预输入，连招第一个 Q 立即发射。
- 修正了敌方英雄头顶 Q 层数数字的绘制位置。此前它是从脚下的屏幕坐标固定抬高若干像素，因此在相机缩放或分辨率改变时会偏离模型。现在改为把世界空间中头顶上方的一个点投影到屏幕，使其无论缩放或分辨率如何都贴在头顶。绘制菜单中的 X/Y 偏移仍可微调。
<!-- MESH-AIO:RELEASE:v2.4.2:END -->

<!-- MESH-AIO:RELEASE:v2.4.1:START -->
## v2.4.1

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.4.1. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준으로 173챔피언(전용 모듈 19개, 공용 엔진 154개) 지원을 그대로 유지합니다.
- 스크립트 로딩 안정성 수정 릴리즈입니다. 예약된 메뉴 멤버 이름을 옵션 이름으로 쓰면 로드가 실패하는 문제를 바로잡고, 개발 문서의 예약어 목록에 `save`를 추가했습니다.

#### Hwei

- 흐웨이 스크립트를 불러올 때 콘솔에 `config: invalid var name "save"` 오류가 뜨며 로딩이 실패하던 문제를 고쳤습니다. R 메뉴의 "다른 스킬만으로 처치 가능하면 R 아끼기" 옵션 내부 이름이 메뉴 시스템의 예약 멤버 `save`와 겹친 것이 원인이며, 표시 이름과 기본값은 그대로 두고 내부 이름만 바꿔 해결했습니다.

#### Locke

- 콤보를 시작할 때 첫 Q가 나가지 않던 문제를 고쳤습니다. 가만히 서 있는 적은 명중 신뢰도 판정이 "정지 상태"로 인식하지 못해 첫 Q가 거부됐는데, 이제 움직이지 않는 대상은 확정 명중으로 보고 곧바로 Q를 시전합니다. 움직이는 대상에 대한 기존 신뢰도 판정과 세미 Q·점멸 연계 동작은 그대로 유지됩니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.4.1. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data (19 hand-tuned modules, 154 on the shared engine).
- A script-loading stability fix: an option whose internal name collided with a reserved menu member made loading fail; that name is corrected and `save` is documented in the reserved-name list.

#### Hwei

- Fixed the Hwei script failing to load with `config: invalid var name "save"` in the console. The R menu's "hold R when ready spells alone can finish the target" option used the internal name `save`, which clashes with a reserved menu member; only the internal name changed, leaving the label and default untouched.

#### Locke

- Fixed the first combo Q not firing. A standing enemy was not recognized as "not moving" by the hit-reliability gate, so the first Q was refused; a target that is not moving is now treated as a guaranteed hit and Q fires immediately. The existing reliability gate for moving targets and the semi Q / flash combo are unchanged.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.4.1。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（19 个专属模块，154 个使用共用引擎）。
- 这是一次脚本加载稳定性修复：当选项的内部名称与保留的菜单成员冲突时会导致加载失败，现已修正该名称，并在保留名单中加入 `save`。

#### Hwei

- 修复了加载彗脚本时控制台报出 `config: invalid var name "save"` 且加载失败的问题。R 菜单中“当仅凭其他技能已能击杀目标时保留 R”选项的内部名称 `save` 与菜单系统的保留成员冲突所致；仅更改了内部名称，显示名称与默认值保持不变。

#### Locke

- 修复了连招开始时第一个 Q 不发射的问题。静止不动的敌人未被命中判定识别为“静止”，导致第一个 Q 被拒绝；现在对不移动的目标视为必中并立即施放 Q。对移动目标的既有命中判定，以及半手动 Q 与闪现连招保持不变。
<!-- MESH-AIO:RELEASE:v2.4.1:END -->

<!-- MESH-AIO:RELEASE:v2.4.0:START -->
## v2.4.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.4.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 18개에서 19개로 늘었고(흐웨이 추가) 나머지 154챔피언은 공용 엔진을 사용합니다.
- 일자·직선 스킬의 자동 시전에 실제 명중 판정을 추가한 공용 모듈을 도입했습니다. 대상이 도착 전에 판정을 벗어날 수 없거나, 멈춰 있거나, 경로가 확정될 때만 발사하며 세미키·도주는 우회합니다. 현재 오로라와 유나라에 적용됩니다.
- 공식 수치 회귀 계약을 65개 추가해 총 431개가 되었습니다. 새 챔피언의 모든 스킬 수치가 공식 원본과 어긋나면 빌드 전에 검사에서 걸립니다.

#### Hwei

- 전용 모듈로 승격했습니다. 흐웨이는 주제(Q/W/E)를 먼저 누르고 다시 Q/W/E를 눌러 시전하는 구조라 실제 시전 가능한 스킬이 10개입니다. 각 스킬은 두 번째 키에 해당하는 물리 슬롯을 사용하므로, 예를 들어 Q-W는 Q로 주제를 연 뒤 W 슬롯을 시전합니다.
- 주제 전환을 상태 기계로 처리합니다. 전환을 요청한 뒤 해당 물리 슬롯의 실제 스킬 이름이 원하는 스킬로 바뀐 것을 확인하고 나서야 실제 시전을 보냅니다. 확인되지 않으면 아무것도 시전하지 않고, 열린 주제는 최대 유지 시간이 지나면 자동으로 취소합니다.
- 스킬 열 개에 각각 전용 설정 항목을 두었습니다. Q-Q 견제, Q-W는 시전 후 실제 도달까지 1.5초가 걸리는 만큼 대상이 속박·둔화 상태이거나 예측이 확정될 때만 사용하고 체력 비율 조건과 귀환 중인 적 조건을 제공합니다. Q-E는 거리·다중 적중 조건, E-Q는 콤보와 돌진 대응, E-W는 속박이라 채널 방해에도 사용하며, E-E는 다중 적중 우선과 자동 방해를 제공합니다.
- W 계열은 아군 전용으로 처리합니다. W-Q 이동 속도 장판은 도주에만, W-W 보호막은 적의 강한 군중 제어나 돌진이 들어올 때와 아군 체력이 낮을 때만, W-E 강화는 지정한 체력·마나 조건에서 사용합니다. 적을 향해 시전하지 않습니다.
- R는 자동 사용 기본 꺼짐입니다. 켜면 대상이 제어된 상태일 것, 다른 스킬로 처치 가능하면 아낄 것, 지정한 체력 비율 아래에서는 쓰지 않을 것, 다중 대상 조건을 확인합니다.
- 팜은 Q-E와 W-E로 라인과 정글을 정리하며 각각 최소 마나와 최소 적중 수를 둡니다. 근처에 적 챔피언이 있으면 팜을 멈추는 옵션이 있습니다.
- 공식 원본을 다시 확인해 두 가지를 바로잡았습니다. R의 지속 피해는 실제로 10/20/30이며, R의 실제 형태는 넓은 원이 아니라 폭 80의 직선으로 적 챔피언에게 처음 맞으면 터집니다. 그래서 팜에는 사용하지 않습니다.

#### Aurora

- 자동 Q1과 E가 이동하는 적에게 허공으로 나가던 문제를 고쳤습니다. 이전에는 예측 지점이 조준선 위에 있기만 하면 발사했는데, 이는 대상이 실제로 그 자리에 있을지와 무관했습니다. 이제 대상이 도착 전에 판정에서 벗어날 수 없거나, 멈춰 있거나, 예측 경로가 확정될 때만 자동으로 발사합니다. 세미키와 도주 사용은 그대로 즉시 발사합니다.

#### Yunara

- 자동 W도 같은 기준으로 고쳤습니다. 멈춰 있거나 직선으로 달려오는 적에게는 그대로 발사하고, 벗어날 수 있는 이동 대상에는 허비하지 않습니다. 도주 W는 예외로 즉시 발사합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.4.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 18 to 19 with Hwei; the remaining 154 champions use the shared engine.
- Added a shared module that puts a real hit test in front of automatic linear casts: they fire only when the target cannot leave the shape before impact, is standing still, or its path is confirmed, while semi keys and flee bypass it. Applied to Aurora and Yunara for now.
- Added 65 official-number regression contracts, bringing the total to 431, so any drift between the new champion's numbers and the official source fails the check before a build.

#### Hwei

- Promoted to a hand-tuned module. Hwei picks a subject with Q/W/E and then presses Q/W/E again, so he has ten castable spells. Each one uses the physical slot of its second key, so Q-W means opening the subject with Q and then casting the W slot.
- Subject switching runs as a state machine. After requesting the switch the module waits until that physical slot's live spell name really is the wanted spell before sending the cast. If it cannot be confirmed nothing is cast, and an open subject is cancelled automatically once its maximum hold time passes.
- All ten spells have their own settings. Q-Q pokes; Q-W takes about 1.5 seconds to land, so it fires only when the target is rooted or slowed or the prediction is confirmed, with health-percentage and recalling-enemy conditions. Q-E has distance and multi-hit conditions, E-Q covers combo and dash responses, E-W is the root and is therefore also used to interrupt channels, and E-E offers multi-target priority and automatic interrupting.
- The W family is treated as ally-only. W-Q is used for fleeing, W-W shields against incoming heavy crowd control or dashes and for a low-health ally, and W-E is used under the configured health and mana conditions. None of them are aimed at enemies.
- R ships with automatic use off. When enabled it requires the target to be impaired, holds R when other spells can already kill, skips targets below a configured health percentage, and checks the multi-target condition.
- Farming clears lanes and camps with Q-E and W-E, each with its own minimum mana and minimum hits, plus an option to stop farming while an enemy champion is nearby.
- Two corrections came out of re-deriving the official source: R's damage over time is 10/20/30, and R is not a wide circle but an 80-wide line that detonates on the first enemy champion it hits, so it is excluded from farming.

#### Aurora

- Fixed automatic Q1 and E firing into empty air at moving targets. Previously a predicted point merely sitting on the aim line was enough to fire, regardless of whether the target would actually be there. They now fire automatically only when the target cannot leave the hit shape before the shot arrives, is standing still, or the prediction path is confirmed. Semi keys and flee still fire immediately.

#### Yunara

- The automatic W got the same treatment: it still fires at a stationary or straight-line chaser but is no longer wasted on a moving target that can dodge it. Flee W is exempt and fires immediately.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.4.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 18 个增加到 19 个（新增彗），其余 154 位英雄使用共用引擎。
- 引入了共用模块，为直线技能的自动施放加入真正的命中判定：只有当目标在弹道到达前无法离开判定、处于静止、或路径已确认时才发射，半手动键与逃跑则绕过。目前应用于奥罗拉与尤娜拉。
- 新增 65 条官方数值回归约定，总数达到 431 条；新英雄的任何技能数值与官方原始数据不一致，都会在构建前被检查拦下。

#### Hwei

- 升级为专属模块。彗需要先用 Q/W/E 选择主题，再按一次 Q/W/E 才能施放，因此他实际可施放的技能有十个。每个技能使用其第二个按键对应的物理槽位，例如 Q-W 是先用 Q 打开主题，再施放 W 槽位。
- 主题切换以状态机处理：请求切换后，先确认该物理槽位的实际技能名称已变成目标技能，才发送真正的施法。无法确认时不施放任何技能；已打开的主题在超过最长保持时间后会自动取消。
- 十个技能各有独立设置。Q-Q 用于消耗；Q-W 从施放到落地约 1.5 秒，因此只在目标被定身或减速、或预测已确认时使用，并提供生命百分比与回城中敌人的条件。Q-E 提供距离与多重命中条件，E-Q 用于连招与反突进，E-W 是定身因此也用于打断引导，E-E 提供多目标优先与自动打断。
- W 系列按仅对友方处理。W-Q 用于逃跑，W-W 在敌方强控或突进来袭以及友方生命较低时提供护盾，W-E 在设定的生命与法力条件下使用，都不会朝敌人施放。
- R 默认关闭自动使用。开启后要求目标处于受控状态、其他技能已能击杀时保留、低于设定生命百分比时不使用，并检查多目标条件。
- 补刀与清野使用 Q-E 与 W-E，各自设有最低法力与最少命中数，并可在附近有敌方英雄时停止补刀。
- 重新核对官方原始数据后修正了两处：R 的持续伤害实际为 10/20/30；R 并非宽阔的圆形，而是宽度 80 的直线，击中第一名敌方英雄即引爆，因此不用于补刀。

#### Aurora

- 修复了自动 Q1 与 E 对移动目标射向空处的问题。此前只要预测点落在瞄准线上就会发射，而不管目标是否真的会在那里。现在只有当目标在弹道到达前无法离开判定范围、处于静止、或预测路径已确认时才自动发射。半手动键与逃跑仍然立即发射。

#### Yunara

- 自动 W 采用同样的判定：对静止或直线追击的目标照常发射，但不再浪费在能够躲开的移动目标上。逃跑 W 为例外，立即发射。
<!-- MESH-AIO:RELEASE:v2.4.0:END -->

<!-- MESH-AIO:RELEASE:v2.3.0:START -->
## v2.3.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.3.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 16개에서 18개로 늘었고(가렌·오로라 추가) 나머지 155챔피언은 공용 엔진을 사용합니다.
- 공식 원본의 서로 다른 필드가 같은 스킬의 크기를 다르게 적는 경우를 정리했습니다. 가렌 E는 원본 두 필드가 실제 회전 범위와 무관한 값이라 Data Dragon의 랭크별 사거리를 사용하고, 오로라 E는 실제 피해와 둔화가 적용되는 사각형 폭을 사용합니다. 두 수정 모두 근거를 코드 주석에 남겼습니다.
- 새 전용 모듈의 공식 수치 회귀 계약을 38개 추가해 총 366개가 되었고, 평타 취소 계약 검사 대상은 9개 스킬로 늘었습니다.

#### Garen

- 전용 모듈로 승격했습니다. Q 결단력의 일격은 공식 평타 초기화 스킬이므로 평타 후딜에 시전하고, 성공한 뒤에만 오브워커 공격 타이머를 초기화합니다. 구조물을 때리는 중에는 초기화 경로를 사용하지 않습니다.
- Q는 도망치는 대상을 따라잡을 때, 침묵으로 실제로 끊을 수 있는 채널을 방해할 때, 처치가 가능할 때 각각 별도 옵션으로 사용합니다. 침묵은 시전이 아니라 강화된 평타가 적중해야 걸리므로 대상이 평타 사거리 안에 있을 때만 판단합니다.
- W 용기는 적의 강한 군중 제어나 돌진이 들어올 때, 그리고 지정한 체력 비율 아래에서만 사용합니다.
- E 심판은 평타 초기화 스킬이 아니므로 자기 평타 시전 동작만 보호하고 공격 타이머는 건드리지 않습니다. 라인 정리에는 최소 적중 수 조건을 둡니다.
- R 데마시아의 정의는 공식 기본 피해와 잃은 체력 비례 처형 피해를 함께 계산해 실제로 처치 가능할 때 사용합니다.
- 참고 스크립트와 같이 포탑 아래에서 Q 사용을 허용하는 전용 키를 추가했습니다.

#### Aurora

- 전용 모듈로 승격했습니다. Q는 첫 시전과 재시전을 각각 켜고 끌 수 있고, 적에게 걸린 표식이 곧 사라질 때 재시전을 자동으로 사용하는 옵션과 남은 시간 기준을 제공합니다. 표식이 걸린 대상을 우선 노립니다.
- W 이동기는 자동 사용이 기본 꺼짐입니다. 도주와 돌진 대응에 사용할 때도 착지 지점이 회피 안전 판정, 적 포탑 구역, 착지 주변 적 수 조건을 모두 통과해야 합니다. 은신 중 평타와 스킬 사용을 막는 옵션과 남은 은신 시간 기준도 제공합니다.
- E는 사용 시 오로라 자신이 뒤로 밀려나므로 이동기와 같은 착지 안전 검사를 적용합니다. Q가 준비된 동안에는 사용하지 않는 옵션과 평타 사거리 밖에서는 사용하지 않는 옵션이 있습니다.
- R은 자동 사용 기본 꺼짐이며, 켜면 지정한 최소 적중 인원 조건을 확인합니다.
- 공식 원본을 다시 확인해 실제 값으로 맞췄습니다. R의 도약 거리는 250, W의 실제 이동 거리는 300이며, 선택 범위와 지대 크기를 이동 거리로 잘못 쓰지 않습니다.
- 오로라에게는 침묵이나 강한 군중 제어가 없어 채널 방해 기능을 넣지 않았습니다. 끊을 수 없는 채널에 궁극기를 낭비하지 않기 위해서입니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.3.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 16 to 18 with Garen and Aurora; the remaining 155 champions use the shared engine.
- Resolved cases where different official fields describe the same spell's size differently. Garen E now uses the Data Dragon per-rank range because both raw fields describe something other than the spin, and Aurora E uses the rectangle width that actually applies its damage and slow. Both corrections carry their evidence in code comments.
- Added 38 official-number regression contracts for the new modules, bringing the total to 366, and the attack-cancel contract check now covers nine spells.

#### Garen

- Promoted to a hand-tuned module. Decisive Strike is an official attack reset, so it is cast during basic-attack recovery and the orbwalker timer is reset only after a successful cast. The reset path is never used while attacking a structure.
- Q has separate options for catching a fleeing target, interrupting a channel a silence can genuinely break, and finishing a kill. Because the silence comes from the empowered basic attack rather than the cast, those checks require the target to be inside attack range.
- Courage is used when heavy enemy crowd control or a dash is incoming, and below a configurable health percentage.
- Judgment is not an attack reset, so it only protects Garen's own attack windup and never touches the attack timer. Lane clear takes a minimum-minions-hit condition.
- Demacian Justice combines the official base damage with the missing-health execute component and is used when it genuinely kills.
- Added the reference script's dedicated key that permits Q use under an enemy turret.

#### Aurora

- Promoted to a hand-tuned module. Q's first cast and its recast have separate switches, plus an option to fire the recast automatically when the enemy's mark is about to expire, with a configurable remaining-time threshold. Marked targets are prioritised.
- The W dash ships with automatic use off. Even for fleeing and anti-gapclose, the landing must pass the evade safety check, the enemy-turret area rule and the nearby-enemy limit. Options to block auto attacks and spells while stealthed, with a remaining-stealth threshold, are included.
- E knocks Aurora backwards, so it uses the same landing safety checks as the dash. It also has options to hold it while Q is available and to skip it outside basic-attack range.
- R ships with automatic use off; when enabled it requires the configured minimum number of enemies hit.
- Re-checked against the official source and corrected to the real values: R's jump distance is 250 and W's actual travel is 300, so the selection range and the zone size are no longer mistaken for travel distance.
- Aurora has no silence and no heavy crowd control, so no channel-interrupt feature was added. That avoids throwing an ultimate at channels it cannot break.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.3.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 16 个增加到 18 个（新增盖伦、奥罗拉），其余 155 位英雄使用共用引擎。
- 整理了官方原始数据中不同字段对同一技能尺寸描述不一致的情况。盖伦 E 改用 Data Dragon 的分等级距离，因为两个原始字段描述的都不是旋转本身；奥罗拉 E 改用真正造成伤害与减速的矩形宽度。两处修正都在代码注释中保留了依据。
- 为新模块增加了 38 条官方数值回归约定，总数达到 366 条；平A取消约定检查覆盖的技能增加到 9 个。

#### Garen

- 升级为专属模块。致命打击是官方普攻重置技能，因此在普攻后摇中施放，并且只有成功施放后才重置走砍计时器。攻击建筑时不会使用重置路径。
- Q 分别提供追击逃跑目标、打断沉默确实能中断的引导、以及完成击杀这三个独立选项。由于沉默来自强化后的普攻而非施法本身，这些判断都要求目标处于普攻距离之内。
- 勇气在敌方强控或突进来袭时使用，并可设定在生命百分比低于阈值时使用。
- 审判不是普攻重置技能，因此只保护盖伦自己的普攻前摇，绝不改动攻击计时器。清线设有最少命中小兵数条件。
- 德玛西亚正义结合官方基础伤害与按已损失生命计算的处决部分，只在确实能击杀时使用。
- 新增参考脚本中允许在敌方防御塔下使用 Q 的专用按键。

#### Aurora

- 升级为专属模块。Q 的首次施放与再次施放各自独立开关，并提供在敌人身上的标记即将消失时自动再次施放的选项与剩余时间阈值。会优先选择带有标记的目标。
- W 位移默认关闭自动使用。即使用于逃跑与反突进，落点也必须通过闪避安全判定、敌方防御塔区域规则与周围敌人数量限制。同时提供隐身期间封锁普攻与技能的选项及剩余隐身时间阈值。
- E 会把奥罗拉向后击退，因此采用与位移相同的落点安全检查。另有在 Q 可用时暂不使用、以及在普攻距离之外不使用的选项。
- R 默认关闭自动使用；开启后会检查设定的最少命中人数条件。
- 重新核对官方原始数据并修正为真实数值：R 的跳跃距离为 250，W 的实际位移为 300，不再把选择范围与区域大小误当作位移距离。
- 奥罗拉没有沉默也没有强控，因此没有加入引导打断功能，以免把大招浪费在无法打断的引导上。
<!-- MESH-AIO:RELEASE:v2.3.0:END -->

<!-- MESH-AIO:RELEASE:v2.2.0:START -->
## v2.2.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.2.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 모듈이 13개에서 16개로 늘었고(말자하·유나라·베인 추가) 나머지 157챔피언은 공용 엔진을 사용합니다.
- 자기 강화 스탠스 스킬을 공식 `Trait_AttackBuff_Duration` 태그로 식별해, 스킬 자체의 효과 반경이 아니라 실제 평타 사거리를 기준으로 사용하도록 고쳤습니다. 애쉬 Q(반경 400)나 유나라 Q(반경 300)처럼 평타 사거리보다 좁은 스탠스는 이전까지 적이 그 좁은 반경 안에 들어와야만 켜져서 원거리 챔피언에게는 사실상 쓰이지 않았습니다. 해당 태그를 가진 62개 스킬이 함께 개선됩니다.
- 스탠스 스킬을 평타 후딜(백스윙) 구간에 시전하도록 확장했습니다. 공식 공격 초기화 태그가 없는 스킬은 백스윙에 넣되 오브워커의 공격 타이머를 초기화하지 않습니다. 초기화가 아닌 스킬을 초기화로 처리하면 실제 공격 가능 시점보다 이른 평타를 시도하게 되기 때문입니다.
- 진짜 글로벌 스킬의 사거리가 0으로 처리되던 문제를 고쳤습니다. 원본과 Data Dragon이 모두 25000 표식을 쓰는 스킬은 사거리를 버리고 시야/적중 반경을 사거리로 오인해, 애쉬 E는 299, 애쉬 R은 130으로 잡혀 있었습니다.
- 커서 방향 최대 사거리 시전을 추가했습니다. 항상 최대 거리를 날아가는 정찰형 스킬은 커서 지점이 아니라 그 방향의 맵 끝을 조준하며, 맵 밖 좌표는 유효한 지점까지 되돌려 잡습니다.
- 채널 인터럽트에서 충전형 하드 CC를 제외하고, 미니언에 막히는 스킬은 예측 경로로 시전하도록 정리했습니다. 부분 충전 상태의 충전기는 군중 제어를 보장하지 못하고, 정중앙 시전은 중간 병사를 무시하기 때문입니다.

#### Ashe

- E 매 날리기가 공식 사거리대로 맵 전역에서 사용됩니다. 시전할 때는 커서가 가리키는 방향의 맵 끝을 조준해 매가 항상 최대 거리를 날아갑니다.
- R 마법의 수정 화살이 공식 글로벌 사거리를 되찾아 세미 R로 화면 밖 적까지 노릴 수 있습니다. 이전에는 사거리가 130으로 잡혀 사실상 사용할 수 없었습니다.
- Q 집중 사격은 공식 공격 초기화 스킬로 평타 후딜에 자동 시전되며, 반경이 아닌 평타 사거리를 기준으로 판단합니다.

#### Malzahar

- 전용 모듈로 승격했습니다. E 재앙의 환상은 해당 미니언을 실제로 처치할 수 있을 때만 사용해 환상이 다음 대상으로 전염되게 합니다. 공식 미니언 처형 기준치와 4초 지속 피해를 함께 계산하며, 보호막이 있으면 처형으로 치지 않습니다.
- Q 공허의 부름은 이미 환상이 걸린 적을 우선 조준하고, 하드 군중 제어에 걸린 적과 돌진 착지 지점에도 사용합니다. 침묵으로 실제로 끊기는 채널만 골라 방해합니다.
- R 황천의 손아귀는 자동 사용이 기본 꺼짐이며, 켜면 대상 체력 비율과 Q/W/E 쿨다운 조건을 확인합니다. 2.5초 동안 제자리에 고정되는 채널이므로 적 포탑 안이거나 주변에 적이 많으면 자동·방해 용도 모두 사용하지 않습니다. 채널 도중에는 다른 시전과 이동을 스스로 멈춰 채널이 깨지지 않게 합니다.
- 세미 R은 키를 누르는 동안 쿨다운이면 다른 판단을 막지 않고 그대로 넘깁니다.

#### Yunara

- 전용 모듈로 승격했습니다. Q 영혼 단련은 평타 후딜에 시전해 공격을 낭비하지 않으며, 공식 공격 초기화 스킬이 아니므로 오브워커 공격 타이머는 건드리지 않습니다.
- W 심판의 궤적은 공식 시전 시간과 투사체 속도로 예측하고, 가장자리에 걸치는 조준을 막는 신뢰도 기준을 적용합니다. 대상이 존야 등으로 얼어 있으면 무적이 풀리는 순간에 맞도록 시점을 계산합니다.
- E는 기본 형태에서 도주와 저체력 상황에만 쓰고, 초월 상태의 돌진은 지형·포탑·주변 적 수·회피 안전 검사를 모두 통과할 때만 사용합니다. 자동 돌진은 기본 꺼짐입니다.
- R 자기 초월은 자동 사용 기본 꺼짐이며, 켜면 지정한 범위 안 적 수 조건을 확인합니다. 초월 상태 판정은 실제로 관측 가능한 신호만 사용하고 확인되지 않으면 사용하지 않습니다.

#### Vayne

- 전용 모듈로 승격했습니다. Q 구르기는 공식 공격 초기화 스킬이므로 평타 후딜에 시전해 공격 속도를 높이며, 성공한 뒤에만 오브워커 타이머를 초기화합니다.
- 구를 방향을 여러 후보로 계산해 지형에 붙는 착지를 우선합니다. 지형에 막혀도 평타는 그대로 취소되지만 위험한 위치로 이동하지는 않기 때문입니다.
- 원거리 딜러 보호를 위해 자동 구르기는 적에게 가까워지는 착지를 사용하지 않습니다. 회피 안전 판정, 적 포탑 지역, 착지 주변 적 수 조건을 모두 통과하지 못하면 그 후딜에는 구르지 않습니다.
- E 선고는 밀려나는 경로를 지형 기준으로 계산해 실제로 벽에 부딪혀 기절이 걸릴 때만 자동으로 사용합니다. 나에게 돌진해 오는 적에게는 벽이 없어도 사용합니다.
- 점멸 후 위치에서 벽 기절이 가능한지 먼저 확인하고 가능할 때만 점멸과 선고를 순서대로 사용하는 전용 키를 추가했습니다. 기절이 불가능하면 아무것도 소모하지 않습니다.
- 현재 대상이 지금 벽으로 밀려 기절 가능한 상태인지 화면에 표시합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.2.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. Hand-tuned modules grew from 13 to 16 with Malzahar, Yunara and Vayne; the remaining 157 champions use the shared engine.
- Attack-empowering stances are now identified by Riot's official `Trait_AttackBuff_Duration` tag and gated on real basic-attack reach instead of the spell's own effect radius. Stances narrower than the attack range, such as Ashe Q at 400 and Yunara Q at 300, previously required the enemy to stand inside that small radius and were effectively unusable on ranged champions. All 62 spells carrying the tag improve together.
- Stances are also cast during basic-attack recovery. A spell without the official attack-reset tag is woven into the backswing but never resets the orbwalker's attack timer, because treating a non-reset spell as a reset makes the orbwalker attack before the real timer is up.
- Fixed genuinely global spells collapsing to zero range. When both the raw data and Data Dragon report the 25000 sentinel, the range was discarded and the vision or hit radius was mistaken for it, leaving Ashe E at 299 and Ashe R at 130.
- Added direction-extended casting. A scouting spell that always travels its full distance now aims at the map edge along the cursor direction instead of the cursor itself, and a coordinate past the map edge is walked back to a valid point.
- Channel interrupting now excludes charge-held crowd control and routes minion-collision skillshots through prediction, because a partially charged spell does not guarantee its crowd control and a dead-center cast ignores the wave in between.

#### Ashe

- Hawkshot is usable across the map at its official range, and casting it aims at the map edge along the cursor direction so the hawk always flies its full distance.
- Enchanted Crystal Arrow regains its official global range, so the semi-manual key can target enemies off screen. It was previously limited to 130 units and effectively unusable.
- Ranger's Focus is an official attack reset, so it is cast during basic-attack recovery and judged by attack range rather than its own radius.

#### Malzahar

- Promoted to a hand-tuned module. Malefic Visions is cast only when it actually kills that minion so the visions spread, combining the official minion execute threshold with the four-second damage total, and a shielded minion is not counted as executed.
- Call of the Void prioritises an enemy already carrying the visions and is also used on hard-crowd-controlled targets and on dash landing points. It interrupts only the channels a silence genuinely cancels.
- Nether Grasp ships with automatic use off; when enabled it checks the target's health percentage and the Q/W/E cooldown conditions. Because the channel roots Malzahar for 2.5 seconds, it is skipped for both automatic and interrupt use while standing under an enemy turret or with too many enemies nearby. During the channel the module stops its own casts and movement so the channel is not broken.
- The semi-manual R key no longer swallows the tick while the spell is on cooldown.

#### Yunara

- Promoted to a hand-tuned module. Spirit Tempering is cast during basic-attack recovery so no attack is wasted, and because it is not an official attack reset the orbwalker's attack timer is left alone.
- Judgment's Path is predicted with the official cast time and projectile speed and uses the reliability standard that refuses edge-of-hitbox aiming. Against an enemy frozen by a stasis effect the timing is computed so the shot lands as the invulnerability ends.
- The base E form is reserved for fleeing and low-health situations, while the Transcendent dash requires terrain, turret, nearby-enemy and evade safety checks to all pass. Automatic dashing ships off.
- Self Transcendence ships with automatic use off; when enabled it checks the configured nearby-enemy condition. The Transcendent state is judged only from observable signals and is never assumed.

#### Vayne

- Promoted to a hand-tuned module. Tumble is an official attack reset, so it is cast during basic-attack recovery to raise attack speed, and the orbwalker timer is reset only after a successful cast.
- Several tumble directions are evaluated and a landing that ends against terrain is preferred, because terrain still cancels the attack without repositioning Vayne into danger.
- To protect the marksman, an automatic tumble never uses a landing that moves closer to an enemy. If the evade safety check, the enemy-turret area rule and the nearby-enemy limit are not all satisfied, that recovery window simply does not tumble.
- Condemn samples the knockback path against terrain and is used automatically only when the target genuinely hits a wall and is stunned. Against an enemy dashing at Vayne it is used even without a wall.
- A dedicated key first checks whether a wall stun becomes possible from the post-Flash position and only then uses Flash followed by Condemn in order. Nothing is spent when the stun is not achievable.
- The interface shows whether the current target can be wall-stunned by Condemn right now.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.2.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。专属模块从 13 个增加到 16 个（新增玛尔扎哈、尤娜拉、薇恩），其余 157 位英雄使用共用引擎。
- 现在通过 Riot 官方的 `Trait_AttackBuff_Duration` 标签识别强化普攻的姿态类技能，并以真实的普攻距离而不是技能自身的效果半径作为判定。像艾希 Q 的 400 和尤娜拉 Q 的 300 这类比普攻距离更短的姿态，此前必须等敌人进入那个很小的半径才会开启，对远程英雄几乎无法使用。带有该标签的 62 个技能一并改善。
- 姿态类技能也会在普攻后摇期间施放。没有官方普攻重置标签的技能只在后摇中释放，绝不重置走砍系统的攻击计时器，因为把非重置技能当作重置会让系统在真实计时结束前就尝试攻击。
- 修复了真正的全图技能距离被判为 0 的问题。当原始数据与 Data Dragon 都使用 25000 标记时，距离会被丢弃并把视野或命中半径误当作距离，导致艾希 E 只有 299、艾希 R 只有 130。
- 新增沿光标方向的最远距离施放。始终飞行满距离的侦察类技能现在瞄准该方向的地图边缘而不是光标位置，超出地图的坐标会回退到有效位置。
- 引导打断现在排除蓄力型硬控，并让会被小兵阻挡的技能走预测路径，因为部分蓄力无法保证控制效果，而直接命中中心会忽略中间的兵线。

#### Ashe

- 鹰击长空恢复官方距离，可在全图使用；施放时瞄准光标方向的地图边缘，让神鹰始终飞满全程。
- 魔法水晶箭恢复官方全图距离，半手动键可以瞄准屏幕外的敌人。此前距离被限制为 130，实际上无法使用。
- 集中打击是官方普攻重置技能，因此在普攻后摇中施放，并以普攻距离而非自身半径作为判定。

#### Malzahar

- 升级为专属模块。虚空幻象只在确实能击杀该小兵时施放，让幻象传播到下一个目标；判定同时结合官方小兵处决阈值与 4 秒总伤害，带护盾的小兵不计入处决。
- 虚空之力优先瞄准已带有幻象的敌人，也会用于被硬控的目标和突进落点，并且只打断沉默确实能中断的引导。
- 虚空掌握默认关闭自动使用；开启后会检查目标生命百分比与 Q/W/E 冷却条件。由于引导会让玛尔扎哈原地固定 2.5 秒，在敌方防御塔范围内或周围敌人过多时，自动与打断两种用途都不会施放。引导期间模块会停止自己的施法与移动，避免引导被打断。
- 半手动 R 在技能冷却时不再吞掉该帧的其他判断。

#### Yunara

- 升级为专属模块。淬魂在普攻后摇中施放，不浪费任何一次攻击；由于它不是官方普攻重置技能，走砍系统的攻击计时器保持不变。
- 裁决之轨使用官方施法时间与弹道速度进行预测，并采用拒绝擦边瞄准的可靠性标准。面对被凝滞效果冻结的敌人，会计算时机让技能在无敌结束的瞬间命中。
- E 的基础形态仅用于逃跑与低生命情况，超越状态下的突进则必须同时通过地形、防御塔、周围敌人数量与闪避安全检查。自动突进默认关闭。
- 自我超越默认关闭自动使用；开启后会检查设定范围内的敌人数量条件。超越状态只依据可观测的信号判定，绝不凭猜测。

#### Vayne

- 升级为专属模块。翻滚是官方普攻重置技能，因此在普攻后摇中施放以提高输出速度，并且只有在施放成功后才重置走砍计时器。
- 会评估多个翻滚方向并优先选择贴着地形结束的落点，因为撞到地形同样能取消普攻，却不会把薇恩送到危险位置。
- 为保护射手，自动翻滚绝不使用会拉近与敌人距离的落点。如果闪避安全判定、敌方防御塔区域规则与周围敌人数量限制没有全部满足，该后摇就不翻滚。
- 精准圣弩会沿击退路径对地形取样，只有目标确实撞墙并被击晕时才自动使用；面对向薇恩突进的敌人则即使没有墙也会使用。
- 新增专用按键：先判断从闪现后的位置是否真能造成撞墙击晕，只有可行时才依次使用闪现与精准圣弩；无法击晕时不消耗任何技能。
- 界面会显示当前目标此刻是否可以被精准圣弩撞墙击晕。
<!-- MESH-AIO:RELEASE:v2.2.0:END -->

<!-- MESH-AIO:RELEASE:v2.1.0:START -->
## v2.1.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.1.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다. 전용 13챔피언의 동작은 이번 버전에서 바뀌지 않았고, 공용 엔진을 쓰는 일반 160챔피언에 아래 세 가지 반응 기능이 추가됐습니다.
- 스테이시스 저격을 추가했습니다(General, 기본 ON). 존야/초시계/바드 R/리산드라 자기 R로 얼어 있는 적은 대상 지정이 불가능하지만 움직일 수도 없으므로, 시전 시간과 투사체 이동 시간을 역산해 무적이 풀리는 순간 정확히 착탄하도록 논타겟 대미지 스킬을 미리 발사합니다. 대상 지정형·돌진·충전·미니언 충돌 스킬은 확정 명중을 보장할 수 없어 제외되며, R은 사용자가 R Combo 옵션을 켠 경우에만 참여합니다.
- 채널링/차징 인터럽트를 추가했습니다(별도 Interrupt 메뉴, 기본 ON). 전 챔피언 전수 조사 인터럽트 DB에서 하드 CC로 실제로 끊기는 채널(갈리오 R, 쉔 R, 카타리나 R, 미스 포츈 R 등)을 감지하면 준비된 하드 CC 스킬을 자동 시전합니다. 고정 채널은 정중앙으로, 이동 가능한 채널과 미니언 충돌형 스킬샷(아리 E류)은 예측 경로로 시전해 중간 웨이브 차단을 검사합니다. 부분 충전 시 CC가 보장되지 않는 충전형 CC(사이온 Q류)와 돌진형은 제외합니다. R 사용은 별도 옵션(기본 OFF), 텔레포트/귀환 인터럽트도 별도 옵션(기본 OFF)입니다.
- 자동 스킬샷 신뢰도 게이트를 추가했습니다(General, 기본 ON). 대상이 도착 전에 걸어서 명중 범위를 벗어날 수 있는 예측 샷은 예측 trace가 확정 경로를 보증할 때만 발사하고, 원형 스킬의 예측 착지점이 대상의 히트 원 밖으로 벗어난 경우는 낡은 경로 리드로 보고 기각합니다. 세미 수동키·Flee·팜 정중앙 시전·AA reset 위빙·충전 해제는 게이트를 거치지 않아 수동 입력과 리셋 창을 잡아먹지 않습니다.
- 충전 스킬은 시작 시 유효한 착지점이 없으면 충전을 시작하지 않으며, 이미 잡고 있는 충전은 게이트와 무관하게 항상 해제됩니다.

#### Ahri

- 매혹(E)이 채널링 인터럽트에 참여합니다. 미니언에 막히는 스킬이므로 정중앙 우회 없이 예측·충돌 검사를 거쳐, 중간 웨이브가 있으면 발사하지 않고 쿨다운을 아낍니다. 콤보/하레스의 Q·E 자동 시전은 신뢰도 게이트를 통과할 때만 발사됩니다.

#### Sion

- 결의의 강타(Q)는 하드 CC 스킬이지만 부분 충전 시 에어본이 보장되지 않아 자동 인터럽트에서 의도적으로 제외했습니다. 수동 사용은 기존과 동일합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.1.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data. The 13 bespoke champions are unchanged in this release; the three reactive features below were added to the shared engine used by the 160 generic champions.
- Added stasis sniping (General, default ON). An enemy frozen by Zhonya/Stopwatch/Bard R/Lissandra self-R is untargetable but cannot move, so the engine back-times cast delay plus projectile travel and fires a non-targeted damage form to land the instant the stasis breaks. Targeted, dash, charge, and minion-collision forms are excluded because they cannot promise the hit, and R joins only when the user has enabled R in Combo.
- Added channel/charge interrupting (its own Interrupt menu, default ON). When an enemy channels something the all-champion interrupt database confirms hard CC actually cancels (Galio R, Shen R, Katarina R, Miss Fortune R and more), the first ready hard-CC form fires automatically. Stationary channels take a dead-center cast; movable channels and minion-collision skillshots (the Ahri E class) go through prediction so a blocking wave is respected. Charge-hold CC (the Sion Q class) is excluded since a partial charge does not guarantee its CC; using R is a separate option (default OFF), and Teleport/Recall interrupting is a separate option (default OFF).
- Added a reliability gate for automatic skillshots (General, default ON). A predicted shot the target can simply walk out of before impact fires only when the prediction trace confirms a committed path, and circular landings that drifted off the target's own hit circle are rejected as stale-path leads. Semi keys, Flee, farm center-casts, AA-reset weaves, and charge releases bypass the gate, so no manual intent or reset window is ever eaten by it.
- Charge spells no longer start charging without a valid landing point, and a held charge always releases regardless of the gate.

#### Ahri

- Charm (E) now participates in channel interrupting. As a minion-collision skillshot it goes through prediction and the collision check instead of a dead-center bypass, so it holds its cooldown when a wave is in the way. Automatic Q/E casts in Combo/Harass fire only after passing the reliability gate.

#### Sion

- Decimating Smash (Q) is a hard-CC spell, but a partial charge does not guarantee the knock-up, so it is deliberately excluded from automatic interrupts. Manual use is unchanged.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.1.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄。本版本 13 位专属英雄的行为没有变化；以下三项反应功能加入了 160 位通用英雄共用的引擎。
- 新增凝滞狙击（General，默认开启）。被中娅沙漏/秒表/巴德 R/丽桑卓自身 R 冻结的敌人无法被选取但也无法移动，引擎会倒推施法时间与弹道飞行时间，提前发射非指向性伤害技能，让其在无敌解除的瞬间准确命中。指向性、突进、蓄力与会被小兵阻挡的技能因无法保证命中而被排除；只有当用户在 Combo 中启用了 R，R 才会参与。
- 新增引导/蓄力打断（独立 Interrupt 菜单，默认开启）。当敌人引导的技能在全英雄打断数据库中确认可被硬控打断（加里奥 R、慎 R、卡特琳娜 R、厄运小姐 R 等）时，自动施放第一个就绪的硬控技能。静止引导直接命中中心；可移动引导与会被小兵阻挡的技能（阿狸 E 类）走预测路径，以尊重中间兵线的阻挡。部分蓄力无法保证控制效果的蓄力型硬控（塞恩 Q 类）与突进型被排除；使用 R 为独立选项（默认关闭），打断传送/回城也是独立选项（默认关闭）。
- 新增自动技能弹道可靠性门槛（General，默认开启）。目标在命中前能够走出判定范围的预测弹道，只有在预测轨迹确认其路径已锁定时才会发射；圆形技能的预测落点偏离目标自身判定圆时视为过期路径提前量并被拒绝。半手动键、逃跑、补刀中心施放、平A重置衔接与蓄力释放不经过该门槛，不会吞掉任何手动意图或重置窗口。
- 蓄力技能在没有有效落点时不再开始蓄力；已经握住的蓄力无论门槛如何都会始终释放。


#### Ahri

- 魅惑（E）现已参与引导打断。作为会被小兵阻挡的技能，它经过预测与碰撞检查而不是直接命中中心，兵线挡路时会保留冷却不发射。连招/骚扰中的 Q/E 自动施放只有通过可靠性门槛后才会发射。

#### Sion

- 破魂斩（Q）虽是硬控技能，但部分蓄力无法保证击飞效果，因此被有意排除在自动打断之外。手动使用不受影响。
<!-- MESH-AIO:RELEASE:v2.1.0:END -->

<!-- MESH-AIO:RELEASE:v2.0.1:START -->
## v2.0.1

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- 버전: v2.0.1. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지합니다.
- 챔피언 173명을 모두 `mesh/<champion>/` 개별 폴더로 분리했습니다. 각 폴더에는 해당 챔피언의 공식 스킬 프로필과 진입 파일이 있어 수치·폼·오류 경로를 챔피언 단위로 추적할 수 있습니다. 일반 160개는 중복 없는 공용 내부 엔진을 호출하고, 전용 13개는 챔피언별 세부 로직을 사용합니다. 루트 디스패처와 샤드 등록표도 같은 생성 라우팅을 사용해 현재 챔피언 폴더 하나만 로드합니다.
- 공식 생성기는 173개 프로필에서 1,004개 exact form과 269개 재시전 형태를 생성·검증합니다. Rengar 강화 W와 Talon R 재시전처럼 기본 슬롯명만으로 구분할 수 없는 형태도 명시적으로 라우팅하며, 동일 이름이 여러 형태에 걸치거나 live 이름이 확인되지 않은 자동 경로는 추측하지 않고 닫힙니다. 지형 전용 Talon E/E2와 시전 폼이 아닌 `RengarEMis` 미사일 객체도 수동·비안전 형태로 고정해 공용/빌린 폼 경로가 전용 안전 검사를 우회하지 못합니다.
- self형 평타 reset 버프는 위빙 옵션이 켜져 있고 실제 대상이 현재 AA 사거리 안에 있을 때만 첫 평타 뒤로 미룹니다. Kayle E처럼 사거리 확장·접근에 쓰는 버프의 AA 사거리 밖 선시전은 유지합니다. 미룬 reset은 windup이 끝난 첫 백스윙에서 즉시 요청하고, 성공한 요청 뒤에만 오브워커 공격 타이머를 reset합니다.
- 평타 대상을 영웅, 라인 미니언, 정글 몬스터, 적 타워로 상호 배타 분류해 Farm 토글, 마나 제한, Lane/Jungle 옵션, 식물 제외 조건이 다른 대상 경로로 새지 않도록 수정했습니다.
- windup 중에는 0.25초 콜백 간격 폴백이 가짜 백스윙을 만들지 않습니다. 별도 windup-transition 신호를 보존해 `cb.spell` 이벤트가 누락돼도 실제 windup 종료 뒤 첫 콜백을 복구하며, 0.12초 신선도 창, 1ms 로컬 재시도 하한, spell-lock 및 server pause를 함께 유지합니다.
- 타워 평타 reset은 AttackReset 태그 전체가 아니라 exact live 스킬 7개만 허용합니다. 해당 스킬 메뉴에 적 타워용 옵션을 기본 ON으로 추가했고 Tower Combat T와 분리했습니다. Riot raw의 구조물 modifier는 Fizz W, Jax W, Rengar Q, Skarner Q에서 확인됐습니다. Fiora E, Jayce 캐논 W, Malphite W는 사용자 제공 동작 계약으로 허용했으며 실제 타워 적용·타이밍은 연습 도구/F12 검증이 남아 있습니다. 억제기와 넥서스도 별도 실측 전까지 제외됩니다.
- 구형 Hanbot 챔피언 예제 7개를 읽기 전용으로 감사해 콤보·재시전·구체·귀환 지점 아이디어만 추출했습니다. 구형 API·2019 수치·orb 교체·동적 로드 코드는 가져오지 않았고, Akali/Leblanc/Qiyana/Rengar/Talon/Syndra/Riven을 Riot 16.15 공식 수치와 현재 안전 계약으로 독립 구현했습니다. 각 메뉴에는 실제 Q/W/E/R 이미지와 연결된 옵션만 표시합니다.
- 새 전용 7명은 자동 처치 시 무적·불사·주문 방어막을 거르고, 팜에서 라인 미니언/실제 몬스터만 세며 와드·트랩·식물을 제외합니다. Tower Combat T는 Combo/Harass/세미처럼 명시된 전투 경로에만 적용되고 Farm/Flee/자동 처치에는 새지 않습니다. 돌진은 공식 의도 종점과 네비게이션이 돌려준 실제 스냅 종점을 각각 검사하고 진행 방향·횡오차가 일치할 때만 통행 가능 위치, 벽/구조물, 사용자 지정 최대 적 수와 Evade `is_action_safe`를 통과시킵니다. Evade가 활성인 틱에는 수동키를 포함한 모든 샤드 이동·시전이 양보하며, Dance `1`/Laugh `2`는 기본 50ms·최소 10ms로 통일했습니다.

#### Akali

- Q, W 조건부 생존, E1/E2 표식 추적, R1/R2 처형을 exact live form으로 분리했습니다. 공식 targeter 기준 Q 폭 145와 선형 R2 거리 750·폭 90을 고정했습니다. Q/R2 다중 적중은 주 대상이 가장자리 35유닛 안쪽이거나 실제 도착 때까지 하드 CC일 때만 후보를 채택하고, 조건을 못 채우면 주 대상 중심으로 복귀합니다. E와 R은 의도 종점·스냅 종점의 방향 일치까지 검사하며, R1은 live 종점이 확정되기 전까지 대상 뒤 150유닛과 공식 715유닛 두 가설이 모두 안전할 때만 자동 사용합니다. E 표식 버프명과 실제 R1 착지 모델은 F12 검증 대상으로 남겼습니다.

#### Leblanc

- Q/W/E와 RQ/RW/RE를 각각 판정하고 W/RW 원점을 따로 보존해 안전 복귀, 형태별 킬스틸, 콤보·하레스·팜·도주·세미 R을 구현했습니다. Q/RQ 표식은 미사일 예상 도착 전에는 소비하지 않고 W/E의 예상 적중까지 pending 상태로 유지합니다. W/RW 다중 적중은 주 대상이 반경 35유닛 안쪽이거나 도착까지 하드 CC일 때만 후보를 채택하고, 아니면 원래 주 대상 중심으로 복귀합니다. 복귀는 원점이 현재 위치보다 실제로 안전할 때만 허용합니다. 공식 cast frame을 반영한 W 0.25초 예측과 실제 return 이벤트/버프 노출은 F12 검증이 남아 있습니다.

#### Qiyana

- E 대상 상태를 보존해 수동 W 뒤 강화 Q로 이어가고, Q/W/E/R은 확인된 exact live 이름으로만 판정합니다. W는 지형 선택 사거리 1,100과 실제 돌진 거리 300을 분리해 계산하고, 300유닛 착지점과 스냅 종점의 거리·방향·횡오차 및 벽/구조물·포탑·적 수·Evade 안전을 모두 확인합니다. 공식 Q 기본/강화 폭 60/80과 R 폭 140을 사용하며, Q 팜과 R 다중 적중은 35유닛 안쪽 여유 또는 도착 시점 하드 CC를 요구합니다. E 실제 종점과 지형 W/R 서버 타이밍은 인게임 검증이 남아 있습니다.

#### Talon

- 패시브 중첩 평타 우선, 근접 AA-Q-AA 0.12초/1ms 위빙, R 은신 중 평타 보존, 수동/Flee E 벽넘기를 구현했습니다. W는 exact `TalonW`일 때만 시전하고 공식 출발탄 2500 속도·75 폭과 복귀탄 3000 속도를 분리하며, 다중 적중은 주 대상의 35유닛 안쪽 여유 또는 도착 시점 하드 CC를 요구합니다. E는 의도 종점과 스냅 종점 모두에서 전방성·횡오차·최대 사거리·실제 벽 횡단을 확인합니다. 라인 팜 Q는 마나 제한을 지키고 Last Hit에서는 근접 Q로 죽는 미니언에만 사용합니다. R 시작 대상을 저장해 은신 종료 후 우선 복귀하되 안전하지 않으면 정상 후보로 폴백합니다. Wall Hop 기본키는 `X1MB`이며 Q reset은 구조물에 금지됩니다.

#### Syndra

- 구체를 provisional/confirmed/held 상태로 추적하고 W 집기·던지기, 다음 틱 Q→E, 기존 구체 E 기절, 인터럽트·안티갭을 구현했습니다. Q/W 전투와 팜은 중심·쌍 중점·원 교점 후보를 적중 수→총 체력 순으로 평가합니다. W1은 구체를 우선 집고, 고정된 W2 팜 착지 반경 안에 이미 센 미니언/몬스터는 집지 않아 선택한 다중 적중 수를 W2까지 보존합니다. 자동 반응과 킬스틸은 평타 windup보다 먼저 처리하며, R은 화이트리스트·구체 수·타워·주문 방어막·과잉 사용을 확인합니다. 구체 callback과 QE 서버 시점은 F12 검증이 남아 있습니다.

#### Riven

- Q1/Q2/Q3 복합 상태, AA-Q-AA 0.12초/1ms 위빙, E→R1→W→Q, AA→Q→W→E 하레스, 실제 E→Flash→W/Q G키, Flee와 팜을 구현했습니다. Q는 검증된 스냅 착지점으로만 시전하고, R2는 각 대상의 `0.25초 + 거리/1450` 실제 도착 시점을 예측합니다. 다중 적중은 주 대상의 35유닛 안쪽 여유 또는 도착까지 하드 CC를 요구하며 실패하면 주 대상 중심으로 복귀합니다. after-attack은 Flee/세미/E-Flash/Evade에서 즉시 닫고 T 허용은 Combo/Harass로만 제한합니다. Q 이동 취소와 E-Flash 서버 타이밍은 F12 검증이 남아 있습니다.

#### Teemo

- Q AA 위빙이 평타 windup 중 콜백 간격 폴백으로 잘못 시작되지 않도록 막고, 실제 백스윙 첫 콜백의 빠른 시전만 유지했습니다.

#### Jax

- W의 exact live form에 적 타워 AA reset 옵션을 추가했습니다. 다른 Jax 형태나 일반 AttackReset 태그는 이 타워 경로를 열 수 없습니다.

#### Malphite

- W 메뉴에 적 타워 AA-W-AA reset 옵션을 기본 ON으로 추가하고, 방금 공격한 실제 타워를 확인한 뒤 오브워커 모드 키가 눌린 동안만 1ms fast path를 사용합니다. 사용자 제공 동작 계약을 구현한 것이며 실제 타워 적용·타이밍은 연습 도구/F12 검증이 남아 있습니다.
- W 팜 위빙은 실제 공격한 라인 미니언 또는 식물이 아닌 정글 몬스터만 허용합니다. E는 계속 평캔이나 after-attack 스킬이 아닙니다.

#### Skarner

- Q의 공식 TurretDamageMod와 exact live form을 기준으로 적 타워 AA reset 옵션을 추가했습니다.

#### Fizz

- W의 공식 TurretMod와 exact live form을 기준으로 적 타워 AA reset 옵션을 추가했습니다.

#### Rengar

- 기본 Q의 공식 TowerMod와 exact live form에만 적 타워 AA reset 옵션을 추가했습니다. 강화 Q는 별도 실측 전까지 제외합니다.
- 4 Ferocity에서는 해제/생존이 필요하면 W, 평타 밖이면 E, 근접이면 Q를 우선하고, R 위장 중에는 도약 전 자동 스킬을 억제한 뒤 도약이 시작된 경우에만 E를 허용합니다. 기본/강화 Q·W·E와 R self-cast는 exact live 이름 allowlist를 통과해야 합니다. 확인되지 않은 `RengarQEmpowered`와 미사일 객체 `RengarEMis`는 F12에서 실제 live slot이 확인될 때까지 자동 시전을 닫고, 수동 E는 대상이 없거나 예측이 거부돼도 그 틱을 소비해 다음 틱에 안전하게 재시도합니다. R 탐색/드로우는 공식 랭크별 2500/3000/3500을 사용하며 도약은 스냅 방향·통행 가능 위치·벽/구조물·포탑·최대 적 수·Evade 안전을 통과해야 합니다.

#### Fiora

- E의 exact live form에 적 타워 AA reset 옵션을 추가했습니다. self 스킬 raw 반경과 무관하게 실제 타워 평타 뒤에만 시전합니다. 사용자 제공 동작 계약을 구현한 것이며 실제 타워 적용·타이밍은 연습 도구/F12 검증이 남아 있습니다.

#### Jayce

- 캐논폼 W Hyper Charge에만 적 타워 AA reset 옵션을 추가했습니다. 해머폼 W Static Field는 exact form 대조에서 제외되며, 캐논 평타 거리에서 raw self 반경 285 때문에 시전이 막히던 문제도 수정했습니다. 사용자 제공 동작 계약을 구현한 것이며 실제 타워 적용·타이밍은 연습 도구/F12 검증이 남아 있습니다.

#### Pyke

- Q 이후 AA-E 위빙이 평타 windup 중 가짜 백스윙으로 시작되지 않도록 막고, 실제 백스윙 첫 콜백의 빠른 E만 유지했습니다.

#### Locke

- Q AA 위빙이 평타 windup을 취소하지 않도록 콜백 간격 폴백을 windup 종료 뒤로 제한하면서 기존 1ms fast path를 유지했습니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Version: v2.0.1. Support remains pinned to all 173 champions from Riot Data Dragon 16.15.1 and the patch-fixed 16.15 client export.
- All 173 champions now have separate `mesh/<champion>/` folders. Each folder owns that champion's official spell profile and entry files, making values, forms, and error paths traceable per champion. The 160 generated modules call one shared internal engine without code duplication, while 13 champions use hand-tuned logic. The root dispatcher and shard manifest use the same generated routes and load only the current champion folder.
- The official generator now creates and verifies 1,004 exact forms and 269 recast forms across all 173 profiles. Forms that cannot be distinguished from their base slot name, including empowered Rengar W and the Talon R toggle, have explicit routes; ambiguous names and unverified live forms fail closed instead of being guessed for automatic casts. Terrain-only Talon E/E2 and the non-cast `RengarEMis` missile object are fixed as manual/unsafe so shared or borrowed-form paths cannot bypass bespoke safety.
- Self-cast attack-reset buffs are deferred only when a real target is already inside the current AA radius. Reach or engage buffs such as Kayle E keep their pre-cast path outside that radius. A deferred reset is requested on the first post-windup callback, and the orbwalker timer is reset only after a successful cast.
- Attack targets are now classified exclusively as champion, lane minion, jungle monster, or enemy turret. Farm toggle, mana, Lane/Jungle switches, and plant filtering can no longer fall through into another target path.
- The 0.25-second callback-gap fallback can no longer create a false backswing during windup. A separate windup-transition signal recovers the first post-windup callback even when `cb.spell` is missing, while the 0.12-second freshness window, 1 ms local retry floor, spell lock, and server pause remain enforced together.
- Turret attack resets are no longer inferred from every AttackReset tag. Only seven exact live forms are allowed, each with a default-on enemy-turret option separate from Tower Combat T. Riot raw structure modifiers exist for Fizz W, Jax W, Rengar Q, and Skarner Q. Fiora E, Jayce cannon W, and Malphite W are enabled from the user-provided behavior contract, with live turret application and timing still pending Practice Tool/F12 verification. Inhibitors and the Nexus stay excluded until separately verified.
- Seven legacy Hanbot champion examples were audited read-only for combo, recast, sphere, and return-point ideas. Old APIs, 2019 values, orbwalker replacement, and dynamic loading were not imported; Akali, Leblanc, Qiyana, Rengar, Talon, Syndra, and Riven were independently implemented against Riot 16.15 data and the current safety contract. Each menu exposes only connected options and live Q/W/E/R icons.
- The seven promoted modules reject invulnerability, death protection, and spell shields for automatic executes; farm paths accept only lane minions or real monsters and exclude wards, traps, and plants. Tower Combat T is restricted to explicit Combo/Harass/Semi paths and cannot leak into Farm, Flee, or automatic killsteal. Dashes validate both the intended endpoint and the navigation-snapped endpoint, require direction and lateral-error agreement, then check passability, walls/structures, the configurable enemy cap, and Evade `is_action_safe`. While Evade owns a tick, every shard movement or cast yields, including manual hotkeys. Dance `1` and Laugh `2` use a shared 50 ms default and 10 ms minimum.

#### Akali

- Split Q, conditional defensive W, marked E1/E2, and R1/R2 execute paths by exact live form. Official targeters pin Q width to 145 and linear R2 to 750 range/90 width. Q/R2 multi-hit candidates are accepted only when the primary target is 35 units inside the edge or remains hard-CC'd through impact; otherwise aim returns to the primary center. E and R validate intended-versus-snapped direction, and automatic R1 conservatively requires both the target-plus-150 and official 715-unit endpoint hypotheses to be safe until the live model is known. The E mark name and live R1 landing model still require F12 validation.

#### Leblanc

- Distinguishes Q/W/E from RQ/RW/RE and stores W and RW origins separately for safe return, form-specific killsteal, Combo, Harass, Farm, Flee, and Semi R. Q/RQ marks cannot be consumed before estimated missile impact, and W/E consumption remains pending until expected impact. W/RW multi-hit candidates require the primary target to be 35 units inside the radius or hard-CC'd through impact; otherwise they fall back to the primary center. Return is allowed only when the origin is actually safer. The official-cast-frame 0.25-second W prediction, live return events, and exposed buffs still need F12 validation.

#### Qiyana

- Preserves the E target for a manual W into empowered Q, while Q/W/E/R accept only verified exact live names. W separates the 1,100 terrain-selection range from the real 300-unit dash and verifies distance, direction, lateral error, walls/structures, turret policy, enemy cap, and Evade safety on the 300-unit and snapped endpoints. Official targeters drive base/empowered Q widths of 60/80 and R width 140; Q farm and R multi-hit require a 35-unit inner margin or hard CC through impact. The live E endpoint and terrain W/R server timing remain pending validation.

#### Talon

- Added passive-stack AA priority, melee AA-Q-AA with the 0.12-second/1 ms weave contract, AA preservation during R stealth, and manual/Flee-only safe E wall hops. W casts only on exact `TalonW`, separates the official 2500-speed/75-width outbound missile from the 3000-speed return, and requires a 35-unit primary margin or hard CC through arrival for multi-hit. E validates forward direction, lateral error, maximum range, and actual wall crossing on both intended and snapped endpoints. Lane Q respects mana and Last Hit uses melee Q only when lethal. R stores and reacquires its start target after stealth when still safe, with normal fallback otherwise. Wall Hop defaults to `X1MB`, and Q reset remains blocked on structures.

#### Syndra

- Tracks spheres as provisional, confirmed, or held and implements W pickup/throw, next-tick Q→E, existing-sphere E stuns, interrupts, and anti-gapclose. Combat and farm Q/W evaluate centers, pair midpoints, and circle intersections by hit count then total health. W1 prioritizes a sphere and excludes minions or monsters already counted inside the fixed W2 farm radius, so pickup cannot lower the planned hit count before the stored W2 landing. Reactive actions and killsteal run before the attack-windup gate; R checks whitelist, sphere count, turret safety, spell shields, and overkill. Sphere callbacks and live QE timing still require F12 validation.

#### Riven

- Added composite Q1/Q2/Q3 state, 0.12-second/1 ms AA-Q-AA weaving, E→R1→W→Q, AA→Q→W→E harass, a real E→Flash→W/Q G key, Flee, and farming. Q casts only at the validated snapped landing. R2 predicts each target at the real `0.25 s + distance / 1450` arrival and accepts multi-hit only with a 35-unit primary margin or hard CC through impact, otherwise falling back to the primary center. After-attack closes immediately for Flee/Semi/E-Flash/Evade, and T permission remains exact Combo/Harass only. Q move-cancel and E-Flash timing remain pending F12 validation.

#### Teemo

- Q weaving can no longer start from the callback-gap fallback during attack windup; only the fast first valid backswing cast remains.

#### Jax

- Added an enemy-turret AA-reset option to the exact live W form. Other Jax forms and generic AttackReset tags cannot open this turret path.

#### Malphite

- Added a default-on enemy-turret AA-W-AA option. It verifies the actual attacked turret and uses the 1 ms fast path only while an orbwalker mode key is active. This implements the user-provided behavior contract; live turret application and timing still require Practice Tool/F12 verification.
- Farm W now accepts only the lane minion or non-plant jungle monster that was actually attacked. E remains excluded from all after-attack and AA-reset logic.

#### Skarner

- Added an enemy-turret AA-reset option to the exact Q form backed by Riot's TurretDamageMod data.

#### Fizz

- Added an enemy-turret AA-reset option to the exact W form backed by Riot's TurretMod data.

#### Rengar

- Added an enemy-turret AA-reset option only to the base Q form backed by Riot's TowerMod data. Empowered Q remains excluded pending separate validation.
- At four Ferocity, W is prioritized for cleanse/survival, E outside AA range, and Q in melee. Automatic spells are held before an R leap and only E is allowed after the leap starts. Base/empowered Q, W, E, and R self-casts require exact live-name allowlists. Unverified `RengarQEmpowered` and the `RengarEMis` missile object stay closed to automatic casts until F12 confirms a live slot, and manual E consumes a rejected/no-target tick so it retries safely on the next tick. R uses the official rank values 2500/3000/3500; leap landings require snapped-direction, passability, wall/structure, turret, enemy-cap, and Evade safety checks.

#### Fiora

- Added an enemy-turret AA-reset option to the exact E form. The self-spell raw radius no longer blocks a cast after a confirmed turret attack. This implements the user-provided behavior contract; live turret application and timing still require Practice Tool/F12 verification.

#### Jayce

- Added the enemy-turret AA-reset option only to cannon-form W Hyper Charge. Hammer-form W Static Field is rejected by exact-form matching, and the raw 285-unit self radius no longer blocks a valid ranged turret weave. This implements the user-provided behavior contract; live turret application and timing still require Practice Tool/F12 verification.

#### Pyke

- The post-Q AA-E weave can no longer begin from a false backswing during windup; only the fast first valid backswing E remains.

#### Locke

- Q weaving now delays the callback-gap fallback until windup has ended, preserving the existing 1 ms fast path without cancelling the attack.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 版本：v2.0.1。继续支持 Riot Data Dragon 16.15.1 与固定 16.15 客户端数据中的全部 173 名英雄。
- 现已将 173 名英雄全部拆分到独立的 `mesh/<champion>/` 文件夹。每个文件夹都拥有该英雄的官方技能配置与入口文件，便于按英雄追踪数值、技能形态和错误路径。160 个生成模块共用一套内部引擎且不复制代码，13 名英雄使用精调逻辑。根分发器与 shard 清单共用同一份生成路由，每局只加载当前英雄文件夹。
- 官方生成器会为 173 份配置生成并验证 1,004 个精确技能形态与 269 个再施法形态。Rengar 强化 W、Talon R 再施法等无法仅靠基础槽位名区分的形态也有显式路由；重名或尚未确认实时名称的自动施法路径会安全关闭，不进行猜测。仅用于地形翻墙的 Talon E/E2 与非施法形态的 `RengarEMis` 飞行物被固定为手动/不安全，防止共享或借用形态路径绕过精调安全检查。
- 自身施放型普攻重置增益只会在真实目标已处于当前普攻范围内时延后；Kayle E 这类扩展距离或接近用增益在普攻范围外仍保留预施放路径。延后的重置会在前摇结束后的首个回调立即请求，并且仅在施法成功后重置走砍计时。
- 普攻目标现在互斥分类为英雄、线上小兵、野怪或敌方防御塔，清线开关、法力限制、线上/野区选项以及植物过滤不会再串入其他目标路径。
- 普攻前摇期间，0.25 秒回调间隔后备逻辑不再制造错误的后摇。独立的前摇转换信号会在 `cb.spell` 事件缺失时恢复真实前摇结束后的首个回调，同时保留 0.12 秒新鲜度窗口、1 毫秒本地重试下限、技能锁与服务器暂停保护。
- 防御塔普攻重置不再根据全部 AttackReset 标签推断，只允许 7 个精确实时技能形态；每个技能都有默认开启的敌方防御塔选项，并与 Tower Combat T 分离。Riot 原始数据只为 Fizz W、Jax W、Rengar Q、Skarner Q 提供结构物修正值。Fiora E、Jayce 炮形态 W、Malphite W 按用户提供的行为契约启用，真实防御塔效果与时序仍需训练模式/F12 验证。高地塔后建筑与水晶枢纽在独立实测前保持排除。
- 以只读方式审计了 7 份旧 Hanbot 英雄示例，仅提取连招、再施法、法球与返回点思路。未引入旧 API、2019 数值、走砍替换或动态加载代码；Akali、Leblanc、Qiyana、Rengar、Talon、Syndra、Riven 均基于 Riot 16.15 数据和当前安全契约独立实现。每个菜单只显示已连接的选项与真实 Q/W/E/R 图标。
- 这 7 个精调模块会在自动斩杀时排除无敌、死亡保护与法术护盾；清线只接受线上小兵或真实野怪，并排除眼、陷阱与植物。Tower Combat T 仅作用于明确的连招/消耗/半自动路径，不会泄漏到清线、逃跑或自动抢杀。位移会分别验证意图终点与导航吸附终点，要求方向和横向误差一致，再检查可通行位置、墙体/建筑、最大敌人数和 Evade `is_action_safe`。Evade 接管当前 tick 时，包括手动热键在内的所有 shard 移动与施法都会让路。Dance `1` 与 Laugh `2` 统一为默认 50 毫秒、最小 10 毫秒。

#### Akali

- 按精确实时形态拆分 Q、条件防御 W、带标记的 E1/E2 与 R1/R2 斩杀。官方 targeter 将 Q 宽度固定为 145，并将线性 R2 固定为 750 距离/90 宽度。Q/R2 多目标候选只有在主目标位于边缘内侧 35 单位，或硬控持续到命中时才会采用，否则回到主目标中心。E/R 会验证意图终点与吸附终点方向；在实时模型确认前，自动 R1 必须同时通过“目标后 150”与官方 715 两种终点假设的安全检查。E 标记名与 R1 实际落点模型仍需 F12 验证。

#### Leblanc

- 分别识别 Q/W/E 与 RQ/RW/RE，并独立保存 W/RW 原点，用于安全返回、形态化抢杀、连招、消耗、清线、逃跑和半自动 R。Q/RQ 标记在预计弹道命中前不会被消费，W/E 的消费会保持 pending 直到预计命中。W/RW 多目标候选要求主目标位于半径内侧 35 单位或硬控持续到命中，否则回退到主目标中心；只有原点确实更安全时才允许返回。基于官方施法帧的 0.25 秒 W 预测、实时返回事件与增益暴露仍待 F12 验证。

#### Qiyana

- 保存 E 目标，使手动 W 后可衔接强化 Q，并且 Q/W/E/R 只接受已确认的精确实时名称。W 将 1,100 地形选择距离与实际 300 位移分开，针对 300 位移终点及吸附终点检查距离、方向、横向误差、墙体/建筑、防塔、敌人数和 Evade 安全。官方 targeter 提供基础/强化 Q 宽度 60/80 与 R 宽度 140；Q 清线和 R 多目标均要求 35 单位内侧余量或硬控持续到命中。E 实际终点及地形 W/R 服务器时序仍待验证。

#### Talon

- 新增被动层数普攻优先、遵循 0.12 秒/1 毫秒契约的近战 AA-Q-AA、R 隐身期间保留普攻，以及仅手动/逃跑使用的安全 E 翻墙。W 只在精确 `TalonW` 形态施放，分开预测官方 2500 速度/75 宽度出发弹与 3000 速度回程弹，多目标必须满足主目标 35 单位余量或命中时硬控。E 在意图与吸附终点都检查前向性、横向误差、最大距离和真实穿墙。线上 Q 遵守法力限制，Last Hit 只在近战 Q 可击杀时使用。R 会记录开大目标，隐身结束后安全时优先重新锁定，否则正常回退。Wall Hop 默认 `X1MB`，Q 重置仍禁止用于建筑。

#### Syndra

- 将法球追踪为临时、确认或持有状态，实现 W 抓取/投掷、下一 tick Q→E、已有法球 E 眩晕、打断与反突进。战斗与清线 Q/W 会按命中数→总生命值评估中心、两点中点和圆交点。W1 优先抓球，并排除固定 W2 清线半径内已计数的小兵/野怪，避免抓取动作减少计划命中数，再将落点保存到 W2。反应动作与抢杀会先于普攻前摇门槛处理；R 会检查白名单、法球数、防塔、法术护盾与过度消耗。法球回调与 QE 实际时序仍需 F12 验证。

#### Riven

- 新增 Q1/Q2/Q3 复合状态、0.12 秒/1 毫秒 AA-Q-AA、E→R1→W→Q、AA→Q→W→E 消耗、真实 E→Flash→W/Q 的 G 键、逃跑和清线。Q 只会朝验证后的吸附落点施放；R2 按每个目标真实的 `0.25 秒 + 距离/1450` 到达时刻预测，多目标必须满足主目标 35 单位余量或硬控持续到命中，否则回退到主目标中心。Flee/半自动/E-Flash/Evade 会立即关闭 after-attack，T 权限仍仅限连招/消耗。Q 移动取消与 E-Flash 时序仍待 F12 验证。

#### Teemo

- Q 普攻编织不会再在普攻前摇期间由回调间隔后备逻辑错误启动，只保留首个有效后摇回调的快速施法。

#### Jax

- 为 W 的精确实时形态加入敌方防御塔普攻重置选项，其他 Jax 形态和通用 AttackReset 标签不能开启该路径。

#### Malphite

- 新增默认开启的敌方防御塔 AA-W-AA 选项；确认刚刚攻击的真实防御塔后，仅在走砍模式键生效时使用 1 毫秒快速路径。该功能按用户提供的行为契约实现，真实防御塔效果与时序仍需训练模式/F12 验证。
- W 清线编织只接受实际攻击的线上小兵或非植物野怪；E 仍然不是平取消、普攻重置或 after-attack 技能。

#### Skarner

- 根据 Riot 官方 TurretDamageMod 与精确 Q 形态加入敌方防御塔普攻重置选项。

#### Fizz

- 根据 Riot 官方 TurretMod 与精确 W 形态加入敌方防御塔普攻重置选项。

#### Rengar

- 仅为带有 Riot 官方 TowerMod 的基础 Q 精确形态加入敌方防御塔普攻重置；强化 Q 在独立实测前保持排除。
- 4 层残暴值时，解控/生存优先 W，普攻范围外优先 E，近战优先 Q；R 伪装跳跃前抑制自动技能，跳跃开始后仅允许 E。基础/强化 Q、W、E 与 R 自施法都必须通过精确实时名称白名单；尚未确认的 `RengarQEmpowered` 与飞行物对象 `RengarEMis` 在 F12 证明为实时槽位前禁止自动施法。手动 E 即使无目标或预测被拒，也会消费当前 tick 并在下一 tick 安全重试。R 使用官方等级距离 2500/3000/3500；跳跃落点必须通过吸附方向、可通行、墙体/建筑、防御塔、最大敌人数和 Evade 安全检查。

#### Fiora

- 为 E 的精确实时形态加入敌方防御塔普攻重置选项；确认防御塔普攻后，自身技能的原始半径不再阻止施法。该功能按用户提供的行为契约实现，真实防御塔效果与时序仍需训练模式/F12 验证。

#### Jayce

- 仅为炮形态 W Hyper Charge 加入敌方防御塔普攻重置。锤形态 W Static Field 会被精确形态检查排除，原始 285 范围也不再阻止远程防御塔编织。该功能按用户提供的行为契约实现，真实防御塔效果与时序仍需训练模式/F12 验证。

#### Pyke

- Q 后 AA-E 编织不会再在普攻前摇期间产生错误后摇，只保留首个有效后摇回调的快速 E。

#### Locke

- Q 普攻编织把回调间隔后备逻辑限制在前摇结束后，保留原有 1 毫秒快速路径且不会取消普攻。
<!-- MESH-AIO:RELEASE:v2.0.1:END -->

<!-- MESH-AIO:RELEASE:v2.0.0:START -->
## v2.0.0

### 한국어

#### 지원 챔피언

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 핵심 및 메뉴

- Riot 16.15.1 Data Dragon과 패치 고정 16.15 클라이언트 원본을 기준으로 173챔피언 전체를 인식하고, 기존 6개 전용 모듈을 제외한 167챔피언에 공용 AIO를 추가했습니다.
- 현재 스킬 슬롯 이름을 공식 raw 형태 1,002개(재시전 268·변신/강화 23·충전 23·평타 리셋 75)와 매 틱 대조하고, 동일 alias는 정확한 mScriptName을 우선해 각 시전 방식으로 분기합니다.
- Elise·Jayce·Nidalee 양방향 변신, Rek'Sai 잠복, Aphelios 무기 전환, Hwei 팔레트뿐 아니라 Sylas의 훔친 궁과 Viego 빙의 슬롯도 공식 전체 카탈로그에서 현재 이름으로 찾습니다.
- 공식 타게팅 계약이 불명확한 형태는 자동 시전을 막고 세미키만 허용하며, 궁극기와 변신 자동 사용은 기본 OFF로 두었습니다.
- 공식 평타 리셋 태그가 있는 형태는 평타 선딜을 보존한 뒤 첫 유효 백스윙에서 요청하고, 거부된 유효 요청만 1ms 스크립트 하한으로 재시도합니다.
- OP.GG 16.15 공개 페이지의 173챔피언 스킬 우선순위와 사용자 팁을 robots.txt 허용 확인 후 별도 보조 캐시에 저장했으며, 수치와 시전 형태는 Riot 원본만 기준으로 사용합니다.

#### Annie

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Olaf

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Galio

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### TwistedFate

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### XinZhao

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Urgot

- 공식 형태 6개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Leblanc

- 공식 형태 10개(재시전 8·변신/강화 5·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vladimir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fiddlesticks

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kayle

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MasterYi

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Alistar

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ryze

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sion

- 공식 형태 5개(재시전 3·변신/강화 0·충전 2·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sivir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Tristana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Warwick

- 공식 형태 5개(재시전 1·변신/강화 0·충전 2·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nunu

- 공식 형태 7개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MissFortune

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ashe

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Tryndamere

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jax

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Morgana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zilean

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Singed

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Evelynn

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Twitch

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Karthus

- 공식 형태 15개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Chogath

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Amumu

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rammus

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Anivia

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shaco

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### DrMundo

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sona

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kassadin

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Irelia

- 공식 형태 8개(재시전 5·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Janna

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gangplank

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Corki

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Karma

- 공식 형태 4개(재시전 0·변신/강화 1·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Taric

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Veigar

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Trundle

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Swain

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Caitlyn

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Blitzcrank

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Katarina

- 공식 형태 8개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nocturne

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Maokai

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Renekton

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### JarvanIV

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Elise

- 공식 형태 11개(재시전 5·변신/강화 2·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Orianna

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MonkeyKing

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Brand

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### LeeSin

- 공식 형태 7개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vayne

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rumble

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Cassiopeia

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Skarner

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Heimerdinger

- 공식 형태 9개(재시전 1·변신/강화 1·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nasus

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nidalee

- 공식 형태 7개(재시전 1·변신/강화 1·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Udyr

- 공식 형태 4개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Poppy

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gragas

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Pantheon

- 공식 형태 7개(재시전 4·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ezreal

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Mordekaiser

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yorick

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Akali

- 공식 형태 10개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kennen

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Garen

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Leona

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Malzahar

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Talon

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Riven

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### KogMaw

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shen

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lux

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Xerath

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shyvana

- 공식 형태 6개(재시전 0·변신/강화 1·충전 0·평타 리셋 3)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ahri

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Graves

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fizz

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Volibear

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rengar

- 공식 형태 8개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Varus

- 공식 형태 4개(재시전 1·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nautilus

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Viktor

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sejuani

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fiora

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ziggs

- 공식 형태 7개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lulu

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Draven

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Hecarim

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Khazix

- 공식 형태 10개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Darius

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jayce

- 공식 형태 8개(재시전 3·변신/강화 2·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lissandra

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Diana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Quinn

- 공식 형태 6개(재시전 2·변신/강화 3·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Syndra

- 공식 형태 9개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### AurelionSol

- 공식 형태 6개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kayn

- 공식 형태 6개(재시전 3·변신/강화 3·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zoe

- 공식 형태 16개(재시전 8·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zyra

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kaisa

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Seraphine

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gnar

- 공식 형태 7개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zac

- 공식 형태 5개(재시전 2·변신/강화 0·충전 2·평타 리셋 2)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yasuo

- 공식 형태 13개(재시전 10·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Velkoz

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Taliyah

- 공식 형태 9개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Camille

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Akshan

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Belveth

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Braum

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kindred

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zeri

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jinx

- 공식 형태 4개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### TahmKench

- 공식 형태 6개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Briar

- 공식 형태 5개(재시전 0·변신/강화 0·충전 1·평타 리셋 3)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Viego

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Senna

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lucian

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zed

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kled

- 공식 형태 8개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ekko

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Qiyana

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vi

- 공식 형태 4개(재시전 1·변신/강화 0·충전 1·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aatrox

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nami

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Azir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yuumi

- 공식 형태 13개(재시전 10·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Samira

- 공식 형태 7개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Thresh

- 공식 형태 8개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Illaoi

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### RekSai

- 공식 형태 10개(재시전 3·변신/강화 3·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ivern

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kalista

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Bard

- 공식 형태 14개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rakan

- 공식 형태 8개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Xayah

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ornn

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sylas

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 3)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Neeko

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aphelios

- 공식 형태 11개(재시전 5·변신/강화 1·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rell

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vex

- 공식 형태 6개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yone

- 공식 형태 6개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ambessa

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Mel

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yunara

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sett

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lillia

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gwen

- 공식 형태 10개(재시전 7·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Renata

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aurora

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nilah

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### KSante

- 공식 형태 13개(재시전 3·변신/강화 0·충전 2·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Smolder

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Milio

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zaahen

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Hwei

- 공식 형태 14개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Naafiri

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Added full 173-champion recognition from Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client export, preserving the six hand-tuned modules and adding the shared AIO baseline to the other 167 champions.
- Matches each live slot name against 1,002 official raw forms (recast 268, transform/upgrade 23, charge 23, attack reset 75) every tick, preferring an exact mScriptName when aliases overlap.
- Covers both directions of Elise, Jayce, and Nidalee transformations, Rek'Sai burrow, Aphelios weapon swaps, Hwei palettes, Sylas stolen ultimates, and Viego possession slots through the full official catalog.
- Forms with an ambiguous official targeting contract stay semi-manual only, while automatic ultimates and transformations remain disabled by default.
- Official attack-reset forms preserve the auto-attack windup, cast on the first valid backswing callback, and retry only valid rejected requests with a 1 ms script-local floor.
- Archived skill priorities and user-tip summaries for all 173 champions from OP.GG 16.15 after verifying robots.txt permission; Riot data remains the sole authority for numbers and cast forms.

#### Annie

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Olaf

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Galio

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### TwistedFate

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### XinZhao

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Urgot

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Leblanc

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 8, transform/upgrade 5, charge 0, attack reset 0) and W→Q→E→R priority.

#### Vladimir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Fiddlesticks

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Kayle

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### MasterYi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Alistar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ryze

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Sion

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 3, transform/upgrade 0, charge 2, attack reset 0) and Q→W→E→R priority.

#### Sivir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Tristana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Warwick

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 2, attack reset 0) and W→Q→E→R priority.

#### Nunu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### MissFortune

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ashe

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→Q→E→R priority.

#### Tryndamere

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Jax

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Morgana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Zilean

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Singed

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Evelynn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Twitch

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Karthus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 15 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Chogath

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### Amumu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Rammus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Anivia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Shaco

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### DrMundo

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Sona

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Kassadin

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Irelia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Janna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Gangplank

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Corki

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Karma

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 1, charge 0, attack reset 0) and Q→E→W→R priority.

#### Taric

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Veigar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Trundle

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Swain

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Caitlyn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Blitzcrank

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Katarina

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Nocturne

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Maokai

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Renekton

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### JarvanIV

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Elise

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 11 official forms (recast 5, transform/upgrade 2, charge 0, attack reset 1) and Q→W→E→R priority.

#### Orianna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### MonkeyKing

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Brand

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### LeeSin

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Vayne

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Rumble

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Cassiopeia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Skarner

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Heimerdinger

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 1, transform/upgrade 1, charge 0, attack reset 0) and Q→W→E→R priority.

#### Nasus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Nidalee

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 1, transform/upgrade 1, charge 0, attack reset 1) and Q→E→W→R priority.

#### Udyr

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Poppy

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Gragas

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Pantheon

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Ezreal

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Mordekaiser

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Yorick

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Akali

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kennen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Garen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### Leona

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Malzahar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Talon

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→Q→E→R priority.

#### Riven

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### KogMaw

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Shen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Lux

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Xerath

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Shyvana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 1, charge 0, attack reset 3) and Q→W→E→R priority.

#### Ahri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Graves

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Fizz

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Volibear

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and W→Q→E→R priority.

#### Rengar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Varus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Nautilus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Viktor

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Sejuani

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Fiora

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Ziggs

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Lulu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Draven

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Hecarim

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Khazix

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Darius

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Jayce

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 2, charge 0, attack reset 1) and Q→W→E→R priority.

#### Lissandra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Diana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Quinn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 3, charge 0, attack reset 1) and Q→W→E→R priority.

#### Syndra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### AurelionSol

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Kayn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 3, charge 1, attack reset 0) and Q→W→E→R priority.

#### Zoe

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 16 official forms (recast 8, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Zyra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Kaisa

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Seraphine

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Gnar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Zac

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 2, attack reset 2) and E→W→Q→R priority.

#### Yasuo

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 10, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Velkoz

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Taliyah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Camille

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Akshan

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Belveth

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Braum

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kindred

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→W→E→R priority.

#### Zeri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Jinx

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### TahmKench

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Briar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 3) and W→Q→E→R priority.

#### Viego

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 1) and Q→E→W→R priority.

#### Senna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Lucian

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Zed

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kled

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ekko

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Qiyana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Vi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 1, attack reset 1) and Q→E→W→R priority.

#### Aatrox

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Nami

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Azir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Yuumi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 10, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Samira

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Thresh

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Illaoi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### RekSai

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 3, transform/upgrade 3, charge 0, attack reset 2) and Q→E→W→R priority.

#### Ivern

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Kalista

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Bard

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 14 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Rakan

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Xayah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Ornn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Sylas

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 3) and W→E→Q→R priority.

#### Neeko

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Aphelios

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 11 official forms (recast 5, transform/upgrade 1, charge 0, attack reset 0) and Q→E→W→R priority.

#### Rell

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Vex

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Yone

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Ambessa

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Mel

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Yunara

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Sett

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→W→E→R priority.

#### Lillia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Gwen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 7, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Renata

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Aurora

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Nilah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### KSante

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 3, transform/upgrade 0, charge 2, attack reset 1) and Q→W→E→R priority.

#### Smolder

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Milio

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Zaahen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Hwei

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 14 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Naafiri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

### 简体中文

#### 支持英雄

- Annie
- Olaf
- Galio
- TwistedFate
- XinZhao
- Urgot
- Leblanc
- Vladimir
- Fiddlesticks
- Kayle
- MasterYi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu
- MissFortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Chogath
- Amumu
- Rammus
- Anivia
- Shaco
- DrMundo
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
- JarvanIV
- Elise
- Orianna
- MonkeyKing
- Brand
- LeeSin
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
- KogMaw
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
- Khazix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- AurelionSol
- Kayn
- Zoe
- Zyra
- Kaisa
- Seraphine
- Gnar
- Zac
- Yasuo
- Velkoz
- Taliyah
- Camille
- Akshan
- Belveth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- TahmKench
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
- RekSai
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
- Renata
- Aurora
- Nilah
- KSante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### 核心与菜单

- 依据 Riot Data Dragon 16.15.1 和固定版本的 16.15 客户端原始数据支持全部 173 位英雄；保留 6 个手工专用模块，并为其余 167 位英雄加入通用 AIO 基线。
- 每个 tick 将当前技能槽名称与 1,002 个官方 raw 形态（再施法 268、变身/强化 23、蓄力 23、普攻重置 75）匹配；别名重叠时优先精确 mScriptName。
- 通过完整官方目录覆盖伊莉丝、杰斯、奈德丽双向变身、雷克塞遁地、厄斐琉斯换枪、慧的画板、塞拉斯偷取终极技能和佛耶戈附身后的技能槽。
- 官方目标类型不明确的形态只允许半自动按键，自动使用终极技能和自动变身默认关闭。
- 带官方普攻重置标签的形态会保留普攻前摇，在第一个有效后摇回调施法，并仅对有效但被拒绝的请求按 1 毫秒脚本下限重试。
- 在确认 robots.txt 允许后，离线保存 OP.GG 16.15 的 173 位英雄技能优先级和用户技巧摘要；技能数值与施法形态仍只以 Riot 原始数据为准。

#### Annie

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Olaf

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Galio

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### TwistedFate

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### XinZhao

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Urgot

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Leblanc

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 10 个官方形态（再施法 8、变身/强化 5、蓄力 0、普攻重置 0）。

#### Vladimir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 0）。

#### Fiddlesticks

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kayle

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### MasterYi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Alistar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ryze

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sion

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 3、变身/强化 0、蓄力 2、普攻重置 0）。

#### Sivir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Tristana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Warwick

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 2、普攻重置 0）。

#### Nunu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### MissFortune

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ashe

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Tryndamere

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Jax

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Morgana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zilean

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Singed

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Evelynn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Twitch

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Karthus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 15 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Chogath

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Amumu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Rammus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Anivia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Shaco

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### DrMundo

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Sona

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kassadin

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Irelia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 1、普攻重置 0）。

#### Janna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gangplank

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Corki

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Karma

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 1、蓄力 0、普攻重置 0）。

#### Taric

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Veigar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Trundle

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Swain

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Caitlyn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Blitzcrank

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Katarina

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Nocturne

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Maokai

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Renekton

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### JarvanIV

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Elise

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 11 个官方形态（再施法 5、变身/强化 2、蓄力 0、普攻重置 1）。

#### Orianna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### MonkeyKing

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Brand

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### LeeSin

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Vayne

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Rumble

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Cassiopeia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Skarner

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Heimerdinger

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 9 个官方形态（再施法 1、变身/强化 1、蓄力 0、普攻重置 0）。

#### Nasus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Nidalee

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 1、变身/强化 1、蓄力 0、普攻重置 1）。

#### Udyr

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Poppy

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 0）。

#### Gragas

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Pantheon

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 1、普攻重置 0）。

#### Ezreal

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Mordekaiser

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yorick

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Akali

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kennen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Garen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Leona

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Malzahar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Talon

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Riven

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### KogMaw

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Shen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lux

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Xerath

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Shyvana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 0、变身/强化 1、蓄力 0、普攻重置 3）。

#### Ahri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Graves

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Fizz

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 1）。

#### Volibear

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Rengar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Varus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 1、普攻重置 0）。

#### Nautilus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Viktor

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sejuani

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Fiora

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Ziggs

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lulu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Draven

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Hecarim

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Khazix

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 10 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Darius

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Jayce

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 3、变身/强化 2、蓄力 0、普攻重置 1）。

#### Lissandra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Diana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Quinn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 2、变身/强化 3、蓄力 0、普攻重置 1）。

#### Syndra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 9 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### AurelionSol

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Kayn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 3、变身/强化 3、蓄力 1、普攻重置 0）。

#### Zoe

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 16 个官方形态（再施法 8、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zyra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kaisa

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Seraphine

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gnar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zac

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 2、普攻重置 2）。

#### Yasuo

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 13 个官方形态（再施法 10、变身/强化 0、蓄力 0、普攻重置 0）。

#### Velkoz

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Taliyah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 9 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Camille

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 2）。

#### Akshan

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Belveth

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Braum

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kindred

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Zeri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Jinx

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### TahmKench

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Briar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 3）。

#### Viego

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 1）。

#### Senna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lucian

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Zed

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kled

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ekko

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Qiyana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Vi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 1、普攻重置 1）。

#### Aatrox

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 1）。

#### Nami

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Azir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yuumi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 13 个官方形态（再施法 10、变身/强化 0、蓄力 1、普攻重置 0）。

#### Samira

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Thresh

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Illaoi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### RekSai

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 3、变身/强化 3、蓄力 0、普攻重置 2）。

#### Ivern

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kalista

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Bard

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 14 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Rakan

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Xayah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Ornn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sylas

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 3）。

#### Neeko

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Aphelios

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 11 个官方形态（再施法 5、变身/强化 1、蓄力 0、普攻重置 0）。

#### Rell

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Vex

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yone

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ambessa

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Mel

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yunara

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Sett

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Lillia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gwen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 7、变身/强化 0、蓄力 0、普攻重置 1）。

#### Renata

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Aurora

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Nilah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### KSante

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 13 个官方形态（再施法 3、变身/强化 0、蓄力 2、普攻重置 1）。

#### Smolder

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Milio

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zaahen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Hwei

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 14 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Naafiri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。
<!-- MESH-AIO:RELEASE:v2.0.0:END -->

<!-- MESH-AIO:RELEASE:v1.1.15:START -->
## v1.1.15

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 실제 평타 위빙 경로를 전수 점검해 평타 선딜은 보존하고, 선딜 종료가 확인된 첫 백스윙 콜백에서 스킬을 즉시 요청하도록 통일했습니다.
- 위빙 전용 fast-cast는 기존 90ms 공통 시전 제한만 우회하고, 서버 스킬 잠금·쿨다운·사거리·대상 안전·서버 pause는 그대로 유지합니다.
- 첫 요청이 잠금 등으로 거부되면 스크립트 내부 최소 1ms 간격으로 재시도합니다. 실제 요청 속도는 Hanbot 틱/콜백과 게임 서버 처리 주기의 제한을 받습니다.
- 새 챔피언의 평타 위빙도 같은 안전·속도 계약을 따르도록 전용 정적 검사와 CI 게이트를 추가했습니다.

#### Locke

- Combo/Harass AA→Q 위빙이 최근 다른 스킬 사용 때문에 90ms 동안 막히지 않고 첫 유효 백스윙 콜백에서 즉시 Q를 요청합니다.
- Q 요청이 일시적으로 거부될 때만 0.12초의 신선도 창 안에서 1ms 최소 간격으로 재시도하며, 옵션 OFF·도주·Evade·대상 소실 시 콜백 스트림을 즉시 닫습니다.

#### Teemo

- Combo/Harass와 정글 AA→Q→AA가 첫 유효 백스윙 콜백에서 즉시 Q를 요청하도록 변경했습니다.
- Q가 준비되지 않았거나 Farm/도주/대상 조건이 끝나면 재호출 스트림을 즉시 종료해 늦은 백스윙에서 Q가 낭비되는 상황을 막았습니다.

#### Malphite

- 실제 평타 리셋인 AA→W→AA가 백스윙 첫 콜백에서 즉시 W를 요청하고, 성공 직후 `orb.core.reset()`을 실행하도록 가속했습니다.
- E는 기존 계약대로 평타 위빙·캔슬·리셋에 포함하지 않았으며, W가 불가능한 상황에서는 after-attack 스트림을 즉시 닫습니다.

#### Pyke

- 기본 Q→평타→E 콤보의 E를 첫 유효 백스윙 콜백에서 즉시 요청하도록 가속했습니다.
- Q 대상·Combo 상태·E 준비·타워 안전 조건이 무효가 되면 재호출을 즉시 종료하고, 유효한 거부만 1ms 최소 간격으로 재시도합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Audited every real auto-attack weave path and standardized it to preserve the attack windup, then request the spell on the first callback that confirms the backswing has begun.
- The weave-only fast-cast path bypasses only the former 90 ms generic cast throttle; server spell lock, cooldown, range, target safety, and server pause remain enforced.
- A rejected first request is retried with a 1 ms script-local minimum interval. Actual issue speed remains bounded by Hanbot's tick/callback rate and the game server.
- Added a dedicated static contract test and CI gate so future champion weaves must keep the same speed and safety rules.

#### Locke

- Combo/Harass AA-to-Q weaving no longer waits behind the 90 ms generic throttle after another recent spell and requests Q on the first valid backswing callback.
- Only temporarily rejected Q requests retry inside the 0.12-second freshness window with a 1 ms floor; disabled weaving, escape/Evade modes, or a lost target close the callback stream immediately.

#### Teemo

- Combo/Harass and jungle AA-to-Q-to-AA now request Q on the first valid backswing callback.
- The re-invoke stream closes immediately when Q, Farm, escape, or target conditions are unavailable, preventing a late Q from being wasted near the end of recovery.

#### Malphite

- The real AA-to-W-to-AA reset now requests W on the first backswing callback and calls `orb.core.reset()` immediately after a successful cast.
- E remains excluded from weaving, animation-cancel, and reset logic, while an unusable W now closes the after-attack stream immediately.

#### Pyke

- Accelerated the E in the normal charged-Q-to-AA-to-E combo so it is requested on the first valid backswing callback.
- Invalid Q target, Combo state, E readiness, or turret safety closes the stream immediately; only valid transient rejections retry with the 1 ms local floor.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 全面检查了所有真正的普攻穿插路径：保留普攻前摇，并在确认进入后摇的第一个回调中立即请求技能。
- 穿插专用 fast-cast 只绕过原有 90 毫秒通用施法限制，服务器技能锁、冷却、距离、目标安全和服务器 pause 仍然保留。
- 首次请求被拒绝时，脚本内部以最低 1 毫秒间隔重试；实际请求速度仍受 Hanbot tick/回调频率和游戏服务器限制。
- 新增专用静态契约检查和 CI 门禁，今后新增英雄的普攻穿插也必须遵守相同的速度与安全规则。

#### Locke

- 连招/消耗的普攻接 Q 不再因近期其他技能触发的 90 毫秒通用限制而等待，会在第一个有效后摇回调中立即请求 Q。
- 只有暂时被拒绝的 Q 才会在 0.12 秒新鲜度窗口内以最低 1 毫秒间隔重试；关闭穿插、逃跑/Evade 或目标丢失时会立即关闭回调流。

#### Teemo

- 连招/消耗和打野的普攻→Q→普攻现在都会在第一个有效后摇回调中立即请求 Q。
- 当 Q、Farm、逃跑或目标条件不成立时立即结束重复回调，防止 Q 在后摇末段过晚释放。

#### Malphite

- 真正的普攻→W→普攻重置现在会在第一个后摇回调中立即请求 W，并在施法成功后立刻执行 `orb.core.reset()`。
- E 依旧不属于普攻穿插、动画取消或普攻重置；W 无法使用时会立即关闭 after-attack 回调流。

#### Pyke

- 加速了标准蓄力 Q→普攻→E 连招中的 E，使其在第一个有效后摇回调中立即请求。
- Q 目标、连招状态、E 准备状态或防御塔安全条件失效时立即停止回调；只有有效的临时拒绝才按最低 1 毫秒间隔重试。
<!-- MESH-AIO:RELEASE:v1.1.15:END -->

<!-- MESH-AIO:RELEASE:v1.1.14:START -->
## v1.1.14

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 진 W 자동 사용 조건을 CC 우선과 표식 폴백으로 분리하고, 실제 유효 사거리 안전 여유를 세부 조절할 수 있게 했습니다.
- W 드로우가 메뉴 최대치가 아닌 안전 여유를 반영한 실제 자동 시전 범위를 표시하도록 동기화했습니다.

#### Jhin

- 자동 W는 투사체 도착까지 유지되는 하드 CC 대상을 먼저 전수 검사합니다. 시전 가능한 CC 대상이 없을 때만 진 표식(`jhinespotteddebuff`)이 있는 적에게 즉시 폴백합니다.
- 기존 안전 계약을 유지해 자동·Combo·Harass·Killsteal W는 평타 사거리 안에서 사용하지 않으며, Semi W만 해당 제한을 우회합니다.
- 공식 3000 사거리 끝에서 발생하는 실패를 줄이도록 25~200유닛, 기본 75유닛의 `Edge safety buffer` 옵션을 추가했습니다.
- 최근 0.5초 안에 경로를 바꾸고 예측 이동량이 120유닛 이하인 잔무빙 대상은 과하게 앞을 예측하지 않고 현재 위치 정중앙에 W를 조준합니다. 돌진이나 확실한 장거리 이동에는 기존 선형 예측을 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Split Jhin's automatic W policy into hard-CC priority and a mark fallback, with a configurable effective-range safety margin.
- Synchronized the W drawing with the real automatic cast range after applying the edge buffer.

#### Jhin

- Automatic W first scans every target for hard CC that lasts through impact. It falls back immediately to an enemy carrying Jhin's mark (`jhinespotteddebuff`) only when no connectable CC target exists.
- Preserved the established safety rule: automatic, Combo, Harass, and Killsteal W remain blocked inside auto-attack range, while directly held Semi W may bypass it.
- Added an `Edge safety buffer` of 25-200 units, default 75, to prevent failures at the edge of the official 3000 range.
- A target that changed path within the last 0.5 seconds with no more than 120 units of predicted lead is aimed at its current center, preventing over-leading against short jitter movement. Dashes and committed long movement retain linear prediction.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 将烬的自动 W 逻辑拆分为硬控优先和标记后备，并加入可调节的实际施法距离安全边距。
- W 范围绘制现在会扣除边缘安全值，与自动施法的真实有效范围保持一致。

#### Jhin

- 自动 W 会先检查所有目标，优先选择硬控持续时间足以覆盖命中时刻的敌人。只有没有可命中的硬控目标时，才会立即改为攻击带有烬标记（`jhinespotteddebuff`）的敌人。
- 保留既有安全规则：自动、连招、消耗和斩杀 W 在普攻范围内仍被禁止，只有按住 Semi W 时可以绕过该限制。
- 新增 25~200 单位、默认 75 单位的 `Edge safety buffer`，减少在官方 3000 最大距离边缘施放失败的情况。
- 若目标在最近 0.5 秒内改变路径，且预测提前量不超过 120 单位，则 W 会瞄准目标当前位置中心，避免对小幅来回移动过度预判；冲刺和明确的长距离移动仍使用线性预测。
<!-- MESH-AIO:RELEASE:v1.1.14:END -->

<!-- MESH-AIO:RELEASE:v1.1.13:START -->
## v1.1.13

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 신규 지원 챔피언 Pyke를 추가하고 실제 스킬 아이콘이 있는 세부 메뉴를 구성했습니다.
- 공식 Riot 16.15.1/16.15 Pyke 수치 21개와 챔피언 레벨별 처형 breakpoint를 자동 회귀 검사에 연결했습니다.

#### Pyke

- 기본 Combo를 차징 Q → 평타 → E로 구현했습니다. Harass는 차징 Q만 사용하고, 짧은 Q는 공식 400 사거리 안에서 Q 한 발로 처치 가능한 경우에만 사용합니다.
- W 접근 → E → Q 기습 콤보와 커서 방향으로 빠진 뒤 Q로 당기는 Delivery E → Q 전용 키를 추가했습니다.
- Q-Flash 키는 현재 차징 사거리와 점멸 400을 함께 계산하고, 직접 Q가 맞으면 점멸을 낭비하지 않습니다. 점멸 후 위치에서 예측·충돌을 다시 계산해 Q를 해제합니다.
- E-Flash 키는 공식 1초 그림자 회수 직전 기본 50ms에만 점멸합니다. 기존 E 선에는 안 맞고 원점→점멸 착지 선에는 맞는 대상만 선택하며 포탑 안전 옵션을 적용합니다.
- Flee는 E와 W가 모두 준비됐을 때 반드시 E를 먼저 사용한 뒤 W를 사용합니다.
- R은 공식 챔피언 레벨 처형 기준과 0.8 추가 공격력·1.5 물리 관통력 계수를 사용합니다. 보호 버프가 없는 처형 대상만 예측하며, Q 차징 중에도 Q를 중단하고 R을 매 틱 최우선 시도합니다.
- Farm MMB의 Q 막타·선택적 라인 클리어·정글 클리어와 실시간 Q 차징/E/R 범위, 처형 표시, Q+E 체력바 피해 표시를 추가했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Added Pyke as a newly supported champion with detailed collapsible menus and live spell icons.
- Connected 21 official Riot 16.15.1/16.15 Pyke values and his champion-level execute breakpoints to the automatic regression gate.

#### Pyke

- Implemented the standard charged Q → auto attack → E Combo. Harass uses charged Q only, while tap Q is reserved for a target killable by one Q inside the official 400 range.
- Added the W approach → E → Q ambush and a dedicated Delivery E → Q key that dashes toward the cursor before pulling the stored target.
- Q-Flash combines live charge range with the 400 Flash range, avoids wasting Flash when Q already connects, then recalculates prediction and collision from the post-Flash position before release.
- E-Flash casts only during the final 50 ms by default before the official one-second shadow return. It requires a target missed by the original E line but crossed by the origin-to-Flash segment and respects turret safety.
- Flee always uses E first and W second when both abilities are ready.
- R uses the official champion-level execute base plus 0.8 bonus AD and 1.5 lethality. It skips protected targets and interrupts a charged Q to retry an executable R target every pre-tick.
- Added Farm MMB tap-Q last hit, optional lane clear and jungle clear, plus live Q-charge/E/R ranges, execute markers, and Q+E health-bar damage.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 新增派克支持，并加入带实时技能图标的详细折叠菜单。
- 将 Riot 16.15.1/16.15 的 21 项派克官方数据及按英雄等级变化的斩杀 breakpoint 接入自动回归检查。

#### Pyke

- 实现标准蓄力 Q → 普攻 → E 连招。消耗模式仅使用蓄力 Q；短 Q 只会在官方 400 范围内且一发 Q 能击杀目标时使用。
- 新增 W 接近 → E → Q 突袭连招，以及向鼠标方向位移后拉回已记录目标的 Delivery E → Q 专用按键。
- Q-Flash 会同时计算实时蓄力距离与 400 闪现距离；Q 本身能够命中时不会浪费闪现，并在闪现后位置重新进行预测与碰撞检测再释放 Q。
- E-Flash 默认只在官方一秒影子返回前最后 50 毫秒使用。目标必须不会被原 E 线命中、但会被起点到闪现落点的线段命中，并遵守防御塔安全设置。
- 当 E 与 W 都可用时，逃跑模式始终先使用 E，再使用 W。
- R 使用官方按英雄等级计算的斩杀基础值，以及 0.8 额外攻击力和 1.5 穿甲系数。它会跳过受保护目标，并在 Q 蓄力期间中断 Q，每个 pre-tick 优先重试可斩杀目标。
- 新增 Farm MMB 的短 Q 补刀、可选清线与打野，并加入实时 Q 蓄力/E/R 范围、斩杀标记和 Q+E 血条伤害显示。
<!-- MESH-AIO:RELEASE:v1.1.13:END -->

<!-- MESH-AIO:RELEASE:v1.1.11:START -->
## v1.1.11

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 궁극기 조준과 치명타 재시도 안전 조건을 함께 개선했습니다.

#### Jhin

- R 채널 중 일반 한 발 피해로 처치 가능한 적을 먼저 찾습니다. 선형 예측과 챔피언·벽 충돌 계산을 통과해 실제로 맞힐 수 있을 때만 키 입력 없이 자동 발사하며 공식 1초 로컬 간격도 유지합니다.
- 처치 대상이 없으면 Semi R 또는 Combo 키를 누르는 동안에만 발사하며, 충돌 없이 맞힐 수 있는 적 중 마우스에 가장 가까운 대상을 선택합니다. 처치 가능 적이 있으면 수동 대상보다 항상 우선합니다.
- R 채널 최초 시작은 기존처럼 Semi R로만 수행하며 시작 방향도 마우스에 가장 가까운 적을 기준으로 합니다. 기존 전체 자동 조준 옵션은 `Auto-fire R on one-shot kill` 옵션으로 교체했습니다.
- 치명타 재시도 간격은 메뉴 설정 없이 1ms로 고정했습니다. `Anti-stuck timeout`은 100~500ms만 설정할 수 있고 기본값은 100ms이며, 제한에 도달하면 진행 중인 취소·재공격 상태도 즉시 종료합니다.
- 치명타 재시도 활성 기준을 30~100%로 확장하고 기본값을 30%로 낮췄습니다. 이전 저장값과 충돌하지 않도록 새 설정 키를 사용합니다.
- 일반 평타 한 발의 온힛 포함 실제 피해로 현재 체력과 공용·물리 보호막을 모두 제거할 수 있으면 치명타 재시도를 건너뛰고 그 평타로 바로 처치합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Improved both Jhin's Curtain Call targeting and critical-retry safety rules.

#### Jhin

- While Curtain Call is active, the script first searches for an enemy killable by one conservative regular shot. It auto-fires without a key only when linear prediction plus champion/wall collision confirms the shot can connect, while preserving the conservative local one-second gate.
- Without a killable target, shots fire only while Semi R or Combo is held and select the collision-free hittable enemy closest to the mouse. A killable target always takes priority over the manual target.
- Curtain Call still starts only from Semi R, now aimed toward the enemy closest to the mouse. The former full auto-aim option was replaced by `Auto-fire R on one-shot kill`.
- The critical-retry pulse is now fixed at 1 ms with no menu setting. `Anti-stuck timeout` is limited to 100-500 ms and defaults to 100 ms; reaching it immediately clears any active cancel/retry state.
- The critical-retry activation threshold now ranges from 30% to 100% and defaults to 30%. A new setting key prevents an older saved threshold from overriding it.
- If one ordinary auto attack's actual damage, including on-hit effects, can remove the target's current health and all/physical shields, that attack is allowed to land instead of being cancelled for a critical retry.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 同时改进烬的大招瞄准与暴击重试安全规则。

#### Jhin

- 大招引导期间，脚本会优先寻找能被一发保守普通大招子弹击杀的敌人。只有线性预测以及英雄、墙体碰撞检测确认能够命中时，才会无需按键自动发射，并保留保守的本地一秒间隔。
- 没有可击杀目标时，仅在按住 Semi R 或 Combo 键期间发射，并选择鼠标附近能够无碰撞命中的最近敌人。可击杀目标始终优先于手动目标。
- 大招仍然只能通过 Semi R 开始，现在会朝鼠标附近最近的敌人开启。原来的完整自动瞄准选项已替换为 `Auto-fire R on one-shot kill`。
- 暴击重试 pulse 现在固定为 1 毫秒，不再提供菜单设置。`Anti-stuck timeout` 只能设置为 100~500 毫秒，默认 100 毫秒；达到限制时会立即清除正在进行的取消与重试状态。
- 暴击重试启用阈值现已扩展为 30%~100%，默认值降至 30%。使用新的设置键，避免旧保存值覆盖新默认值。
- 如果一次普通攻击包含攻击特效后的实际伤害足以清空目标当前生命值以及通用、物理护盾，则不会为了暴击重试而取消这次攻击，而是直接完成击杀。
<!-- MESH-AIO:RELEASE:v1.1.11:END -->

<!-- MESH-AIO:RELEASE:v1.1.10:START -->
## v1.1.10

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 재시도 기본 간격을 1ms로 낮추고 고착 기본 시간을 300ms로 단축했습니다.

#### Jhin

- `Retry pulse` 기본값을 5ms에서 1ms로 낮췄습니다. 범위는 1~50ms를 유지하며 실제 속도는 게임 pre-tick 해상도 안에서 가장 빠르게 동작합니다.
- `Anti-stuck timeout` 최소값을 500ms에서 100ms로 낮추고 기본값을 3000ms에서 300ms로 변경했습니다. 현재 pending/confirmed 상태까지 즉시 종료하는 전체 hard limit라 100ms 설정이 실제로 120ms까지 늘어나지 않습니다.
- 기존 저장된 5ms/3000ms 값이 새 기본값을 덮지 않도록 두 슬라이더 모두 새 설정 키로 분리했습니다. 치명타 기준 최소·기본 60%와 Crit/보장 4타 보호는 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Reduced Jhin's default retry pulse to 1 ms and shortened the default anti-stuck duration to 300 ms.

#### Jhin

- Reduced the `Retry pulse` default from 5 ms to 1 ms. Its 1-50 ms range remains, with effective speed bounded only by the game's pre-tick resolution.
- Reduced the `Anti-stuck timeout` minimum from 500 ms to 100 ms and its default from 3000 ms to 300 ms. It is a hard whole-chain deadline that immediately clears pending/confirmed state, so a 100 ms setting cannot stretch to the separate 120 ms cancellation timeout.
- Both sliders use new setting keys so saved 5 ms/3000 ms values cannot override the new defaults. The 60% minimum/default threshold and random-crit/fourth-shot protection remain unchanged.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的默认重试 pulse 降至 1 毫秒，并将默认防卡死时间缩短至 300 毫秒。

#### Jhin

- 将 `Retry pulse` 默认值从 5 毫秒降至 1 毫秒，范围仍为 1~50 毫秒，实际速度仅受游戏 pre-tick 精度限制。
- 将 `Anti-stuck timeout` 最低值从 500 毫秒降至 100 毫秒，默认值从 3000 毫秒改为 300 毫秒。它是整个链的硬性截止时间，会立即清除 pending/confirmed 状态，因此 100 毫秒设置不会被单次取消的 120 毫秒超时延长。
- 两个滑块都改用新的设置键，防止旧的 5 毫秒/3000 毫秒保存值覆盖新默认值。最低/默认 60% 暴击阈值以及随机暴击、第四发保护保持不变。
<!-- MESH-AIO:RELEASE:v1.1.10:END -->

<!-- MESH-AIO:RELEASE:v1.1.9:START -->
## v1.1.9

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 재시도 속도·고착 시간을 메뉴에서 직접 조절할 수 있게 하고 기본 속도를 5ms로 높였습니다.

#### Jhin

- 치명타 활성 기준을 최소·기본 60%로 변경했습니다. 기존 저장값과 충돌하지 않도록 새 설정 키를 사용합니다.
- `Retry pulse` 슬라이더를 추가했습니다. 1~50ms 범위에서 실시간 조절할 수 있으며 기본값은 5ms입니다. 취소 확인 뒤 설정한 pulse가 만료되는 첫 pre-tick에 즉시 재공격합니다.
- `Anti-stuck timeout` 슬라이더를 추가했습니다. 500~10000ms 범위, 기본 3000ms이며 고정 횟수 제한 없이 이 시간 안에서 성공할 때까지 반복합니다. Crit과 보장 4타는 계속 즉시 통과합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Added user controls for Jhin's retry speed and anti-stuck duration, with a faster 5 ms default pulse.

#### Jhin

- Changed the critical activation threshold to a 60% minimum and default. A new setting key avoids conflicts with previously saved values.
- Added a `Retry pulse` slider, adjustable live from 1 to 50 ms and defaulting to 5 ms. The reattack is issued on the first pre-tick after the configured pulse expires.
- Added an `Anti-stuck timeout` slider from 500 to 10000 ms, defaulting to 3000 ms. With no fixed attempt cap, retries continue until success within this duration. Random crits and the guaranteed fourth shot still pass immediately.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 添加烬的重试速度与防卡死时间自定义设置，并将默认 pulse 提升为 5 毫秒。

#### Jhin

- 将暴击启用阈值的最低值和默认值改为 60%。使用新的设置键，避免与旧保存值冲突。
- 新增 `Retry pulse` 滑块，可在 1~50 毫秒之间实时调整，默认 5 毫秒。配置的 pulse 到期后的第一个 pre-tick 会立即重新攻击。
- 新增 `Anti-stuck timeout` 滑块，范围 500~10000 毫秒，默认 3000 毫秒。没有固定次数上限，会在该时间内持续重试直到成功。随机暴击和必定暴击第四发仍会立即放行。
<!-- MESH-AIO:RELEASE:v1.1.9:END -->

<!-- MESH-AIO:RELEASE:v1.1.8:START -->
## v1.1.8

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반탄 취소 후 재공격 대기 시간을 대폭 줄이고 고정 12회 제한을 제거했습니다.

#### Jhin

- 인게임에서 이동 취소가 정상 작동하는 것을 확인한 뒤, 취소 확인과 재공격을 기다리던 최소 시간을 80ms에서 10ms로 줄였습니다. 실제로는 다음 pre-tick에서 바로 같은 대상을 다시 공격합니다.
- 공격 잠금 pulse도 80/50ms에서 10ms로 줄이고 취소 실패 제한을 200ms에서 120ms로 단축해 실패 상태에서도 오래 멈추지 않습니다.
- 고정 12회 재시도 제한을 제거했습니다. 이제 성공할 때까지 빠르게 반복하며, 비정상 고착만 막는 대상별 전체 3초 제한을 유지합니다. Crit과 보장 4타는 계속 즉시 통과합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Greatly reduced Jhin's post-cancel reattack delay and removed the fixed 12-attempt limit.

#### Jhin

- After in-game confirmation that movement cancellation works, the minimum cancellation-to-reattack wait was reduced from 80 ms to 10 ms. The same target is now reattacked on the next available pre-tick.
- The attack-lock pulse was reduced from 80/50 ms to 10 ms, and the failed-cancellation timeout from 200 ms to 120 ms, preventing unnecessary stalls even on failure.
- Removed the fixed 12-attempt retry cap. Retries now continue rapidly until success, with only a three-second per-target anti-stuck timeout. Random crits and the guaranteed fourth shot still pass immediately.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 大幅缩短烬取消普通子弹后的重新攻击延迟，并移除固定 12 次限制。

#### Jhin

- 在游戏内确认移动取消正常工作后，将取消到重新攻击的最短等待时间从 80 毫秒缩短到 10 毫秒。现在会在下一个可用 pre-tick 立即重新攻击同一目标。
- 攻击锁定 pulse 从 80/50 毫秒缩短到 10 毫秒，取消失败超时从 200 毫秒缩短到 120 毫秒，即使失败也不会长时间停顿。
- 移除固定 12 次重试上限。现在会高速重试直到成功，仅保留每个目标 3 秒的防卡死总超时。随机暴击和必定暴击第四发仍会立即放行。
<!-- MESH-AIO:RELEASE:v1.1.8:END -->

<!-- MESH-AIO:RELEASE:v1.1.7:START -->
## v1.1.7

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반탄 감지는 정상이나 정지 명령이 windup을 끊지 못하던 런타임 문제를 실제 이동 취소 경로로 교체했습니다.

#### Jhin

- 새 F12 로그에서 일반탄 감지와 임계값 통과는 정상이나, `player:stop()` 이후 `attack_cancel` 없이 매번 0.2초 timeout이 발생하는 것을 확인했습니다. 메뉴 옵션 문제가 아니라 Hanbot Stop 명령이 진의 평타 windup을 끊지 못한 것이 원인이었습니다.
- 일반탄의 실제 `cb.spell` 시점부터 공격만 짧게 막고 마우스 방향 이동 명령을 반복해 windup을 취소합니다. 취소 확인 후 공격 pause가 자연 만료되면 같은 대상을 다시 공격합니다.
- 비평타 주문에서 남아 있던 이전 `cur_attack_name` 때문에 Q가 4타로 기록되던 진단 오분류도 수정했습니다. 이제 실제 기본 공격 이벤트에서만 보조 이름을 사용하며 Crit과 보장 4타 보호는 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ineffective windup Stop path with real movement cancellation after confirming that ordinary-round detection itself was correct.

#### Jhin

- New F12 logs confirmed that ordinary-round detection and the threshold gate worked, but every `player:stop()` reached the 200 ms timeout without `attack_cancel`. The menu setup was correct; Hanbot's Stop command did not cancel Jhin's attack windup.
- Starting at the real ordinary-attack `cb.spell`, the script now briefly pauses attacks and repeatedly issues a movement order toward the mouse to cancel the windup. It reattacks the same target only after cancellation is confirmed and the attack pause expires naturally.
- Fixed stale `cur_attack_name` making Q appear as a fourth shot in diagnostics. The auxiliary orb attack name is now trusted only on a real basic-attack event, while random crit and guaranteed fourth-shot protection remains intact.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 在确认普通子弹识别正常后，将无法中断前摇的 Stop 流程改为真实移动取消流程。

#### Jhin

- 新的 F12 日志确认普通子弹识别和阈值判断都正常，但每次 `player:stop()` 都没有触发 `attack_cancel`，并在 200 毫秒后超时。菜单设置没有问题，原因是 Hanbot 的 Stop 命令无法中断烬的攻击前摇。
- 从真实普通攻击的 `cb.spell` 开始，现在会短暂暂停攻击并持续向鼠标方向发送移动命令来取消前摇。只有确认取消且攻击暂停自然结束后，才会重新攻击同一个目标。
- 修复旧的 `cur_attack_name` 导致 Q 在诊断中被误记为第四发的问题。现在仅在真实基本攻击事件中使用该辅助名称，同时继续保护随机暴击和必定暴击第四发。
<!-- MESH-AIO:RELEASE:v1.1.7:END -->

<!-- MESH-AIO:RELEASE:v1.1.6:START -->
## v1.1.6

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반 평타 취소 감지를 애니메이션 이벤트에서 실제 공격 시작 이벤트로 교체했습니다.

#### Jhin

- F12 로그에서 일반 평타의 `Attack1/2/3` 애니메이션 이벤트가 한 번도 오지 않고 `Reload_Recoil`만 들어오는 것을 확인했습니다. 애니메이션 콜백은 이제 진단 로그만 남기며 취소 상태를 변경하지 않습니다.
- 자기 `cb.spell`의 공식 공격 이름으로 일반탄을 감지해 80ms 전체 정지와 `player:stop()`을 즉시 발행합니다. 실제 `spell.target`만 저장하며, 대상이 없는 이벤트는 안전하게 무시합니다.
- `JhinCritAttack`, `JhinPassiveAttack`, `JhinBasicAttack4`, 현재 4타 버프와 오브워커 공격 이름을 함께 확인해 확률 치명타와 보장 4타는 절대 중단하지 않습니다. 80ms 재공격보다 길었던 120ms 제한도 제거해 성공 또는 안전 제한까지 연속 재시도할 수 있습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ordinary-attack cancellation trigger from animation events to the real attack-start event.

#### Jhin

- F12 logs confirmed that ordinary attacks never emitted `Attack1/2/3` animation events and only emitted `Reload_Recoil`. Animation callbacks are now diagnostic-only and cannot mutate retry state.
- Ordinary rounds are detected from Jhin's official attack names in his own `cb.spell`; the script immediately applies an 80 ms full pause and `player:stop()`. Only the exact `spell.target` is retained, and targetless events fail safely.
- `JhinCritAttack`, `JhinPassiveAttack`, `JhinBasicAttack4`, the live fourth-shot buff, and the orbwalker attack name jointly protect random crits and the guaranteed fourth shot. The obsolete 120 ms gate that blocked the 80 ms retry chain was removed so retries can continue until success or a safety cap.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的普通攻击取消触发方式从动画事件改为真实的攻击开始事件。

#### Jhin

- F12 日志确认普通攻击从未触发 `Attack1/2/3` 动画事件，只出现了 `Reload_Recoil`。动画回调现在仅用于诊断日志，不再修改重试状态。
- 现在通过烬自身 `cb.spell` 中的官方攻击名称识别普通子弹，并立即执行 80 毫秒整体暂停与 `player:stop()`。只保存准确的 `spell.target`，没有目标的事件会安全忽略。
- 同时检查 `JhinCritAttack`、`JhinPassiveAttack`、`JhinBasicAttack4`、当前第四发增益和走砍攻击名称，确保随机暴击及必定暴击第四发绝不被中断。已移除会阻断 80 毫秒重试链的旧 120 毫秒限制，使其能够持续重试直到成功或触发安全上限。
<!-- MESH-AIO:RELEASE:v1.1.6:END -->

<!-- MESH-AIO:RELEASE:v1.1.5:START -->
## v1.1.5

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반 평타 취소 방식을 실제 전체 행동 정지 명령으로 교체했습니다.

#### Jhin

- 이동 명령으로는 일반 Attack1~3 평타가 취소되지 않던 문제를 수정했습니다. 이제 전체 오브워커를 잠깐 정지하고 `player:stop()`을 발행해 현재 행동을 직접 중단합니다.
- 진 본인의 `attack_cancel` 또는 Stop 원점 80ms 뒤 windup 종료로 취소를 확인합니다. 유한 전체 정지가 자연 만료되면 reset 후 같은 유효 대상을 재공격하며, 중간 사용자 주문·200ms Stop 실패·사망·R 채널에서는 재공격하지 않습니다. Crit과 보장 4타 Attack4는 그대로 공격합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ordinary-attack cancellation with the actual full action-stop command path.

#### Jhin

- Fixed ordinary Attack1-3 attacks not cancelling when only a movement order was used. The script now briefly pauses the full orbwalker and issues `player:stop()` to stop the current action directly.
- Cancellation is confirmed by Jhin's own `attack_cancel` or a stopped windup 80 ms from the original Stop. Once the finite full pause expires naturally, it resets and reattacks the same valid target; a manual user order, 200 ms stop failure, death, or Curtain Call discards the retry. `Crit` and guaranteed fourth-shot `Attack4` continue normally.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的普通攻击取消方式改为实际的“停止所有行动”命令流程。

#### Jhin

- 修复仅使用移动命令时无法取消普通 Attack1-3 攻击的问题。现在会短暂暂停整个走砍系统，并发送 `player:stop()` 直接停止当前行动。
- 通过烬自身的 `attack_cancel`，或从原始 Stop 起 80 毫秒后攻击前摇已经结束来确认取消。有限的整体暂停自然结束后，脚本会重置走砍并重新攻击同一个有效目标；若期间出现玩家手动命令、200 毫秒内 Stop 失败、角色死亡或开启大招，则放弃重试。`Crit` 与必定暴击的第四发 `Attack4` 会正常放行。
<!-- MESH-AIO:RELEASE:v1.1.5:END -->

<!-- MESH-AIO:RELEASE:v1.1.4:START -->
## v1.1.4

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 애니메이션 취소 후 재공격이 빠졌던 문제를 긴급 수정했습니다.

#### Jhin

- 일반 Attack1~3 모션을 취소한 뒤 다음 공격을 발행하지 않아 재시도가 멈추던 문제를 수정했습니다. 실제 `attack_cancel` 확인 50ms 뒤 첫 안전한 틱에서 오브워커를 초기화하고 같은 유효 대상을 재공격합니다.
- 진 본인의 취소 이벤트만 허용하고 대상별 한 체인을 최대 12회·1.5초로 제한하며, 한도 이후에는 초기화 조건까지 일반 공격을 허용합니다. Crit과 보장 4타 Attack4는 계속 보존합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Hotfixed Jhin's missing reattack after a critical-animation cancellation.

#### Jhin

- Fixed the retry stopping after cancelling an ordinary Attack1-3 animation because no replacement attack was issued. The first safe tick 50 ms after a confirmed `attack_cancel` now resets the orbwalker and reattacks the same valid target.
- Only Jhin's own cancel event is accepted. Each target-specific chain is capped at 12 attempts or 1.5 seconds, after which ordinary attacks are allowed until a reset condition. `Crit` and the guaranteed fourth-shot `Attack4` remain protected.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 紧急修复烬取消暴击动画后没有重新发起普攻的问题。

#### Jhin

- 修复取消普通 Attack1-3 动画后未发出替代攻击，导致重试停止的问题。现在会在确认 `attack_cancel` 后 50 毫秒的第一个安全 tick 重置走砍，并重新攻击同一个有效目标。
- 仅接受烬自身的取消事件。每个目标的重试链最多 12 次或 1.5 秒，达到上限后会允许普通攻击，直到满足重置条件。继续保护 `Crit` 与必定暴击的第四发 `Attack4`。
<!-- MESH-AIO:RELEASE:v1.1.4:END -->

<!-- MESH-AIO:RELEASE:v1.1.3:START -->
## v1.1.3

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 궁 재사용, 치명타 재시도, W 평타 사거리 규칙을 실제 입력 상태에 맞게 교정했습니다.

#### Jhin

- R2 슬롯이 준비되지 않은 요청 때문에 다음 탄환이 약 2초까지 늦어질 수 있던 문제를 수정했습니다. 서버 강제 공식 1초는 유지하며, Auto는 보수적 간격을 지키고 Semi R 또는 Combo 키를 누르는 동안에는 슬롯이 준비되는 첫 틱부터 성공할 때까지 빠르게 재시도합니다.
- 치명타 재시도 기본 기준을 45%로 바로잡고 새로운 저장 키를 사용합니다. 문자열과 숫자 해시 애니메이션을 모두 식별하며 F12 진단에 실제 분류와 차단 조건을 표시합니다.
- 챔피언이 평타 사거리 안에 있으면 CC 상태여도 Combo, Harass, Auto, Killsteal에서 W를 사용하지 않습니다. 평타 사거리 안 W는 사용자가 Semi W 키를 누른 경우에만 허용됩니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Corrected Jhin's Curtain Call recast, critical retry, and W attack-range rules against live input state.

#### Jhin

- Fixed non-ready R2 requests delaying the next shot by up to roughly two seconds. The server-enforced official one-second minimum remains; Auto keeps its conservative interval, while a held Semi R or Combo input retries every tick from the first ready slot until the request succeeds.
- Corrected the critical-retry default threshold to 45% with a fresh save key. Both string and numeric-hash animation events are recognized, and F12 diagnostics now show the classification and active gates.
- W is never cast by Combo, Harass, Auto, or Killsteal against a champion inside attack range, even when the target is crowd controlled. Only a directly held Semi W may bypass this rule.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 根据实时输入状态修正了烬的大招再次施放、暴击重试以及 W 普攻距离规则。

#### Jhin

- 修复 R2 尚未就绪的请求导致下一发可能延迟到约两秒的问题。保留服务器强制的一秒官方最低间隔；自动模式维持保守间隔，按住 Semi R 或连招键时则从技能槽就绪的第一帧开始逐帧重试，直到请求成功。
- 将暴击重试默认阈值修正为 45%，并使用新的保存键。现在可识别字符串与数字哈希动画事件，F12 调试会显示实际分类与拦截条件。
- 当英雄位于普攻距离内时，即使目标处于控制状态，连招、消耗、自动逻辑和斩杀也不会使用 W；只有玩家直接按住 Semi W 时才允许例外。
<!-- MESH-AIO:RELEASE:v1.1.3:END -->

<!-- MESH-AIO:RELEASE:v1.1.2:START -->
## v1.1.2

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 체력바를 가리던 상단 패시브/치명타 상태 표시와 해당 설정 메뉴를 제거했습니다.

#### Jhin

- 챔피언 위에 표시되던 `CRIT xx% | E n | R ...` 텍스트를 제거해 체력바와 겹치지 않게 했습니다.
- 챔피언 아래의 기존 세로 핫키/상태 목록은 그대로 유지됩니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Removed Jhin's upper passive/critical status display and its settings menu because it overlapped the health bar.

#### Jhin

- Removed the `CRIT xx% | E n | R ...` text previously drawn above Jhin so it no longer covers the health bar.
- Kept the existing vertical hotkey/status list below the champion unchanged.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 移除了会遮挡烬生命条的上方被动/暴击状态显示及其设置菜单。

#### Jhin

- 移除了原先显示在烬上方的 `CRIT xx% | E n | R ...` 文本，使其不再遮挡生命条。
- 保留英雄下方现有的纵向快捷键/状态列表。
<!-- MESH-AIO:RELEASE:v1.1.2:END -->

<!-- MESH-AIO:RELEASE:v1.1.1:START -->
## v1.1.1

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 직선 예측 입력을 공식 Hanbot 스키마로 교정하고 같은 필드 오류를 차단하는 회귀 계약을 추가했습니다.

#### Jhin

- W 또는 R 탄환 예측 시 `pred/collision` 내부에서 `vec2 nil` 치명 오류가 발생하던 문제를 수정했습니다.
- W와 R의 실제 투사체 폭은 유지하면서 직선 충돌 판정이 요구하는 `width` 필드를 사용하도록 변경했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Corrected Jhin's linear prediction inputs to the Hanbot schema and added regression contracts that reject the same field mismatch.

#### Jhin

- Fixed the fatal `vec2 nil` error inside `pred/collision` when predicting W or Curtain Call shots.
- Preserved the official projectile widths while supplying the required `width` field for linear collision prediction.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的直线预测输入修正为 Hanbot 所需格式，并新增回归契约以阻止相同字段错误再次出现。

#### Jhin

- 修复 W 或大招子弹预测进入 `pred/collision` 时触发的 `vec2 nil` 致命错误。
- 保留官方弹道宽度数值，同时改用直线碰撞预测所要求的 `width` 字段。
<!-- MESH-AIO:RELEASE:v1.1.1:END -->

<!-- MESH-AIO:RELEASE:v1.1.0:START -->
## v1.1.0

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- mesh-aio에 다섯 번째 챔피언 Jhin을 추가하고, 실제 Q/W/E/R 아이콘이 표시되는 접이식 메뉴와 사용자 지정 단축키를 연결했습니다.
- Riot 16.15.1/16.15 공식 데이터로 진의 피해량·사거리·시전 시간·투사체·함정·궁 탄환 계약을 고정하고 F12 진단을 추가했습니다.

#### Jhin

- Combo와 Harass에 Q/W/E 사용, 평타 사거리 안 비활성화, W 하드 CC 조건, 자동 처치·CC·정지 대상 반응을 각각 조절할 수 있게 했습니다.
- `MMB` Farm 토글에 Q/W/E 라인·정글 옵션과 최소 적중 조건을 추가하고, Q 연쇄 대상과 W 관통 경로를 보수적으로 선택하도록 했습니다.
- Semi W와 Semi R 키를 추가했습니다. R은 자동으로 시작하지 않으며, Semi R로 커튼 콜을 연 뒤 채널 중 실제 3500 사거리 탄환만 예측 조준합니다.
- 일반 치명타 `Crit` 모션과 보장 4타 `Attack4`를 분리하는 실험적 치명타 재시도 옵션을 추가했습니다. 기본값은 꺼짐이며 활성 기준은 45~100%로 설정할 수 있고, 보장 4타와 이미 치명타인 공격은 취소하지 않습니다.
- Q/W/E/R 실시간 범위, 패시브·치명타 상태, 콤보 피해 체력바, 처치 가능 표시와 세로형 핫키 상태줄을 추가했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Added Jhin as the fifth mesh-aio champion with collapsible menus, live Q/W/E/R icons, and rebindable hotkeys.
- Locked Jhin's damage, range, cast-time, projectile, trap, and Curtain Call shot contracts to Riot 16.15.1/16.15 data and added F12 diagnostics.

#### Jhin

- Added separate Combo and Harass controls for Q/W/E, disable-inside-AA-range rules, hard-CC-only W behavior, killsteal, and automatic CC/immobile reactions.
- Added Q/W/E lane and jungle controls under the `MMB` Farm toggle, including minimum-hit settings and conservative Q-bounce/W-line selection.
- Added rebindable Semi W and Semi R. Curtain Call never starts automatically; Semi R opens it and only the active 3500-range shots are prediction-aimed during the channel.
- Added an experimental critical retry option that distinguishes random `Crit` attacks from the guaranteed fourth-shot `Attack4`. It is off by default, supports a 45-100% activation threshold, and never cancels an already-critical or guaranteed fourth shot.
- Added live Q/W/E/R ranges, passive and critical state text, combo-damage health bars, killable indicators, and the standard vertical hotkey status list.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- mesh-aio 新增第五名英雄 Jhin，并加入可折叠菜单、实时 Q/W/E/R 图标与可重新绑定的快捷键。
- 根据 Riot 16.15.1/16.15 官方数据固定烬的伤害、距离、施法时间、弹道、陷阱与大招子弹规则，并加入 F12 调试信息。

#### Jhin

- 为连招与消耗分别加入 Q/W/E 控制、普攻范围内禁用、W 仅对硬控目标、斩杀以及自动控制/静止目标反应选项。
- 在 `MMB` 清线开关中加入 Q/W/E 对线与野怪选项、最低命中数，以及保守的 Q 弹跳和 W 穿透路径选择。
- 新增可改键的半自动 W 与半自动 R。脚本不会自动开启谢幕；只有按下 Semi R 开启后，才会在引导期间预测瞄准实际 3500 距离的子弹。
- 新增实验性暴击重试选项，区分随机 `Crit` 与必定暴击的第四发 `Attack4`。默认关闭，可设置 45-100% 的启用阈值，并且不会取消已经暴击或必定暴击的第四发。
- 新增 Q/W/E/R 实时范围、被动与暴击状态、连招伤害生命条、可击杀提示以及标准纵向快捷键状态列表。
<!-- MESH-AIO:RELEASE:v1.1.0:END -->

<!-- MESH-AIO:RELEASE:v1.0.2:START -->
## v1.0.2

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- 기존 메뉴 설정과 사용자 X/Y 보정값을 유지하면서 티모 화면 표시 위치를 교정했습니다.

#### Teemo

- 패시브 `STEALTH`·공격 속도·은신 대기시간 표시가 체력바에 붙던 문제를 수정해, 다시 챔피언 머리 위 전용 위치에 표시되도록 했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- Corrected Teemo's on-screen indicator position while preserving existing menu settings and user X/Y offsets.

#### Teemo

- Fixed the passive `STEALTH`, attack-speed, and stealth-countdown text appearing on the health bar; it now uses the dedicated above-champion position again.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- 在保留现有菜单设置与用户 X/Y 偏移的同时，修正了提莫屏幕提示的位置。

#### Teemo

- 修复被动 `STEALTH`、攻速与隐身倒计时文字贴在生命条上的问题，现在会重新显示在英雄头顶的专用位置。
<!-- MESH-AIO:RELEASE:v1.0.2:END -->

<!-- MESH-AIO:RELEASE:v1.0.1:START -->
## v1.0.1

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- Riot 공식 챔피언 캐시와 네 챔피언의 핵심 피해 상수·계수·사거리·시전 시간을 자동 대조하는 회귀 검사를 추가했습니다.
- 파밍과 CC 판정에 사용하는 스킬 도착 시간을 공식 castFrame과 투사체 속도 기준으로 교정했습니다.

#### Locke

- R의 다중 적중 판정과 실제 시전이 동일한 예측 착지점을 사용하도록 통합했습니다.
- R 가장자리 적은 35유닛 안전 여유 또는 충분한 하드 CC가 있을 때만 계산하며, 선택한 대상은 중앙 단일 조준을 유지합니다.

#### Teemo

- Q 파밍 체력 예측에 공식 0.493초 시전시간과 투사체 이동시간을 반영했습니다.
- Semi R은 기본적으로 챔피언에게만 사용하며, 챔피언이 없을 때 정글 몬스터에 사용하는 동작을 별도 기본 OFF 옵션으로 분리했습니다.
- 샤드를 다시 불러온 뒤에도 실제 아군 버섯을 검사해 기존 버섯 주변에 중복 설치하지 않도록 수정했습니다.

#### Malphite

- 현재 방관 규칙에 맞게 구형 레벨 비례 물리 관통 계산을 제거해 W 피해 예측을 교정했습니다.
- 자동 R과 Semi Multi R의 최소 적중값을 2명으로 고정하고, R 착지시간·하드 CC·이동 여유·선택 타겟 중앙 조준을 반영했습니다.
- Tower Combat 토글을 두 Semi R 경로에도 적용하고 Q 파밍 예측 시간을 공식 0.333초로 교정했습니다.

#### Soraka

- Q-only 자동 Combo/Harass 계약에 맞게 킬 가능 원과 체력바 예상 피해를 Q 단독 피해로 수정했습니다.
- Q 시전시간을 공식 0.283초로 교정하고, 거리별 투사체 이동시간을 하드 CC·예측·스테이시스 판정에 반영했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- Added an automated regression check that compares the four champions' core damage constants, ratios, ranges, and cast timings against the local Riot-authoritative cache.
- Corrected farm and crowd-control impact timing to use official cast frames and missile speeds.

#### Locke

- Unified R multi-hit evaluation and casting so both use the same predicted landing point.
- Edge targets now count only with a 35-unit safety margin or sufficient hard CC, while a selected target stays centered as a single-target cast.

#### Teemo

- Updated Q farm-health prediction to include the official 0.493-second cast time and missile travel.
- Semi R is champion-only by default; jungle fallback is now a separate opt-in option that remains disabled by default.
- Live allied mushrooms are checked after shard reloads to prevent duplicate trap placement near existing mushrooms.

#### Malphite

- Removed the obsolete level-scaled lethality conversion so W physical-damage prediction follows the current penetration rule.
- Enforced a two-target minimum for Auto R and Semi Multi R and added landing-time, hard-CC, movement-margin, and selected-target centering checks.
- Applied Tower Combat gating to both Semi R paths and corrected Q farm prediction to the official 0.333-second cast time.

#### Soraka

- Aligned the killable circle and health-bar estimate with the Q-only automatic Combo/Harass contract.
- Corrected Q to the official 0.283-second cast time and included distance-based missile travel in hard-CC, prediction, and stasis timing.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- 新增自动回归检查，将四名英雄的核心伤害常量、系数、距离与施法时间和本地 Riot 官方缓存进行对照。
- 清线与控制判定的命中时间现在使用官方施法帧和飞行速度。

#### Locke

- R 的多目标判定与实际施放现在共用同一个预测落点。
- 边缘目标只有在保留 35 单位安全距离或拥有足够硬控时才会计入；选定目标时保持中央单目标施放。

#### Teemo

- Q 的补刀生命预测现在包含官方 0.493 秒施法时间和飞行时间。
- Semi R 默认只对英雄使用；无英雄时对野怪使用的逻辑已拆分为独立选项，并默认关闭。
- 重新载入分片后会直接检查场上的友方蘑菇，避免在已有蘑菇附近重复放置。

#### Malphite

- 移除过时的等级缩放穿甲换算，使 W 的物理伤害预测符合当前穿甲规则。
- Auto R 与 Semi Multi R 最少要求命中两名敌人，并加入落地时间、硬控、移动余量与选定目标中央瞄准判定。
- 两种 Semi R 都会遵守 Tower Combat 开关，Q 补刀预测时间修正为官方 0.333 秒。

#### Soraka

- 按照自动 Combo/Harass 只使用 Q 的规则，将可击杀圆圈与血条预估改为仅计算 Q 伤害。
- Q 施法时间修正为官方 0.283 秒，并在硬控、预测和凝滞计时中加入按距离计算的飞行时间。
<!-- MESH-AIO:RELEASE:v1.0.1:END -->

<!-- MESH-AIO:RELEASE:v1.0.0:START -->
## v1.0.0

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- mesh-aio 단일 샤드에서 4개 챔피언을 자동 분기하고, 공용 인터럽트·스테이시스 모듈과 실시간 상태 표시 규칙을 모든 모듈에 일관되게 적용했습니다.
- 접을 수 있는 챔피언별 메뉴, 실제 스킬 아이콘, 사용자 지정 단축키와 쿨다운 연동 범위 표시를 유지하면서 런타임 충돌 방어 규칙을 보강했습니다.

#### Locke

- Q 위빙을 평타 백스윙 시작 후 0.12초 안에서만 허용하고, 사용할 수 없을 때 호출 스트림을 닫아 후반에 위빙이 영구 정지하던 문제를 수정했습니다.
- 존야·바드 R·리산드라 R로 정지된 적에게 무적 해제 순간 Q가 도착하도록 스테이시스 저격 로직을 추가했습니다.

#### Teemo

- AA → Q → AA 위빙 신호를 이중화하고 평타 사거리 밖에서는 Q를 직접 사용해, 공속이 높아진 뒤 콤보 Q가 멈추던 문제를 수정했습니다.
- 스테이시스 중 적 발밑에 R을 미리 설치하도록 추가하고, 비행시간과 1초 장전시간을 모두 반영해 해제 직후 확실하게 작동하도록 보정했습니다.
- Laugh Attack을 평타당 한 번으로 제한하고, 부활 후 상태 초기화와 만료된 독 추적 데이터 정리를 추가했습니다.

#### Malphite

- 전투 순서를 R → 착지 E → Q → AA-W-AA로 정리했으며, 평타 리셋이 아닌 E를 after-attack 경로에서 제거하고 W만 실제 평타 리셋으로 유지했습니다.
- R 다중 적중 반경을 325에서 공식 수치 270으로, 팜 Q 투사체 속도를 1400에서 1200으로 교정했습니다.
- 스테이시스 해제 순간 E가 맞도록 도착 시간을 0.242초로 보정하고 자동 저격 옵션을 추가했습니다.

#### Soraka

- 자동 Combo와 Harass는 Q만 사용하도록 정리하고, E는 수동 Force E·인터럽트·하드 CC·갭클로저·스테이시스·킬스틸 조건에서만 사용하도록 제한했습니다.
- 전 챔피언 채널링·차징 인터럽트 데이터베이스를 연결하고, 스테이시스 해제 순간 Q와 E가 도착해 점멸과 대시를 막도록 추가했습니다.
- 동일 챔피언 아군이 여러 명일 때도 각 아군의 W 우선순위와 체력 슬라이더가 독립적으로 적용되도록 수정했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- The single mesh-aio shard now dispatches all four champions while sharing the interrupt, stasis, and live status-display rules consistently across modules.
- Preserved collapsible champion menus, live spell icons, rebindable hotkeys, and cooldown-aware range drawings while strengthening runtime compatibility guards.

#### Locke

- Q weaving is now accepted only within 0.12 seconds of a fresh auto-attack backswing, and the invoke stream closes when Q cannot be used, preventing permanent late-game weave stalls.
- Added stasis timing so Q lands as Zhonya, Bard R, or Lissandra R invulnerability expires.

#### Teemo

- Reinforced the AA → Q → AA signal path and added direct Q casting outside auto range, fixing combo Q stalls at higher attack speeds.
- Added pre-placement of R under stasis targets and corrected the timing to include missile travel plus the full one-second arm time.
- Limited Laugh Attack to once per auto, reset runtime state after respawn, and cleaned expired poison tracking entries.

#### Malphite

- Standardized combat to R → landing E → Q → AA-W-AA, removed E from the after-attack path, and kept W as the only true auto-attack reset.
- Corrected the R multi-hit radius from 325 to the official 270 value and Q farm missile speed from 1400 to 1200.
- Added E stasis sniping with a corrected 0.242-second impact time so it hits immediately after invulnerability ends.

#### Soraka

- Automatic Combo and Harass now use Q only, while E is restricted to configured Force E, interrupt, hard-CC, gapcloser, stasis, and killsteal reactions.
- Connected the all-champion channel and charge interrupt database and added Q/E stasis timing that blocks immediate Flash or dash escapes.
- Fixed per-ally W priority and health sliders when multiple allied units use the same champion.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- mesh-aio 单一分片现在会自动分配四名英雄，并在全部模块中统一使用打断、凝滞与实时状态显示规则。
- 保留可折叠的英雄菜单、真实技能图标、自定义快捷键和冷却联动范围显示，同时加强运行时兼容保护。

#### Locke

- Q 技能只会在普通攻击后摇开始后的 0.12 秒内衔接，无法施放时会关闭调用流，修复后期连招永久停止的问题。
- 新增凝滞结束狙击逻辑，使 Q 在中娅、巴德 R 或丽桑卓 R 的无敌结束瞬间命中。

#### Teemo

- 强化 AA → Q → AA 的双重触发信号，并在普攻距离外直接施放 Q，修复高攻速时连招 Q 停止的问题。
- 新增在凝滞目标脚下预先放置 R，并同时计算飞行时间与完整的一秒启用时间。
- 嘲笑动作现在每次普攻最多触发一次，同时新增复活状态重置与过期毒素记录清理。

#### Malphite

- 连招统一为 R → 落地 E → Q → AA-W-AA，E 不再进入攻击后触发路径，只有 W 保留真正的普攻重置。
- R 的多目标判定半径从 325 修正为官方数值 270，清线 Q 的飞行速度从 1400 修正为 1200。
- 新增 E 凝滞结束狙击，并把命中时间修正为 0.242 秒，使技能在无敌结束后立即命中。

#### Soraka

- 自动连招与消耗模式只使用 Q，E 仅在已配置的强制施放、打断、硬控、突进、凝滞和斩杀条件下使用。
- 接入全英雄引导与蓄力技能打断数据库，并新增 Q/E 凝滞结束计时以阻止目标立即闪现或位移。
- 修复队伍中存在多个相同英雄时，每个友军的 W 优先级与生命值滑块无法独立生效的问题。
<!-- MESH-AIO:RELEASE:v1.0.0:END -->
<!-- MESH-AIO:UPDATES:END -->
