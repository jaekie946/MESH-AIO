<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.15.0:START -->
## v2.15.0

### 한국어

#### 지원 챔피언


<details>
<summary>지원 챔피언 173명 펼치기</summary>

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

</details>

#### 핵심 및 메뉴

- 버전: v2.15.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지하며, 전용 모듈이 24개(공용 149)로 늘었습니다.
- KogMaw가 24번째 전용 모듈로 승격되었습니다. 공식 16.15 원본 수치 26개 항목이 자동 회귀 검사에 고정되었습니다.

#### KogMaw

- 신규 전용 모듈: W(사거리 +130~210, 8초, %최대체력 온힛 강화 자기 버프)가 핵심 교리입니다. 콤보에서 대상이 W 확장 사거리 안에 들어오는 순간 W를 켜고, W가 도는 동안 실공속이 임계값(기본 3.0, 슬라이더) 이상이면 자동 Q/E/R 시전을 스킬별 토글로 억제해 기관총 평타를 스킬이 끊지 않게 합니다. 킬스틸·세미 키·스테이시스 저격은 억제에서 제외됩니다.
- Q(1175 사거리, 방어력/마저 감쇄)는 콤보 선두로 나가고, E(1200 사거리, 관통 슬로우)는 콤보 슬로우·돌진 착지 반응 피격 저지·Flee(Z)를 담당합니다.
- R는 랭크별 1300/1550/1800 포격입니다: 콤보 R는 대상 체력 %(기본 65) 이하 + 코스트 스택 상한(기본 2) + 평타 도달 대상 제외 옵션을 모두 지켜야 나가고, Auto R 토글(U)은 자체 스택 상한(기본 3)에 공격 가능한 적이 하나라도 있으면 쏘지 않습니다. 코스트 스택은 공식 8초 창에서 자기 시전을 추적해 스택당 +40, 상한 400 마나를 항상 확인합니다.
- 처형 수학 내장: 잃은 체력 1%당 +0.833%(최대 ×1.5), 체력 40% 미만은 공식 ×2를 그대로 반영해 킬스틸 R가 정확히 계산합니다. W 온힛(%최대체력, 몬스터 상한 100)도 처치 가능 표시에 포함됩니다.
- 처치 확정 Q 막타 팜(대포/슈퍼 우선, 평타 도달 스킵 옵션, 정글 포함)과 최소 명중 수 기반 E 라인 클리어, Semi R(Space)/Semi E(G), W 가동 중 확장 사거리 원 드로우를 제공합니다.
### English

#### Supported Champions


<details>
<summary>Expand the 173 supported champions</summary>

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

</details>

#### Core & Menu

- Version: v2.15.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data; hand-tuned modules grow to 24 (shared-engine 149).
- KogMaw is promoted to the 24th dedicated module. 26 official 16.15 raw values are pinned into the automated regression checks.

#### KogMaw

- New dedicated module built around W - the self-buff that adds 130..210 attack range for 8 seconds plus the %-max-health on-hit. Combo turns W on the moment the target enters the extended reach, and while W runs with the live attack speed above the threshold slider (3.0 default), automatic Q/E/R casts are suppressed per spell so nothing interrupts the machine-gun window. Killsteal, semi keys, and stasis snipes stay exempt.
- Q (1175 range, armor/MR shred) opens the combo; E (1200 range, piercing slow) covers the combo slow, peeling a dash that lands on Kog'Maw, and Flee (Z).
- R is the rank-ranged 1300/1550/1800 artillery: combo R requires the target-HP slider (65 default), the cost-stack cap (2 default), and the option that skips targets the basic attack already reaches; the Auto R toggle (U) has its own stack cap (3 default) and never fires while any attackable enemy exists. Cost stacks are tracked from own casts over the official 8-second window (+40 per stack, 400 cap) and every automatic R checks affordability.
- The execute math is built in: +0.833% per 1% missing health up to x1.5, and the official x2 below 40% health, so the R killsteal computes exactly. The W on-hit (%-max-health, 100 monster cap) is part of the killable indicator.
- Ships kill-secured Q last hits (cannon/super first, AA-reach skip option, jungle included), an E lane clear at the minimum-hits slider, Semi R (Space) / Semi E (G), and the extended-attack-range circle drawn while W runs.
### 简体中文

#### 支持英雄


<details>
<summary>展开 173 位支持英雄</summary>

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

</details>

#### 核心与菜单

- 版本：v2.15.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄；专属模块增至 24 个（共用引擎 149 个）。
- 克格莫晋升为第 24 个专属模块，26 项官方 16.15 原始数值已固定进自动回归检查。

#### KogMaw

- 新专属模块，以 W 为核心——这个自身增益提供 130~210 攻击距离加成（8 秒）和 %最大生命值的攻击特效。连招在目标进入扩展射程的瞬间开 W；W 期间若实时攻速超过阈值滑条（默认 3.0），自动 Q/E/R 将按技能开关被抑制，确保没有技能打断机枪普攻窗口。抢头、手动键与凝滞狙击不受抑制。
- Q（1175 射程，护甲/魔抗削减）作为连招起手；E（1200 射程，穿透减速）负责连招减速、敌方突进落点的反打减速以及 Flee（Z）。
- R 是按等级 1300/1550/1800 射程的炮击：连招 R 需同时满足目标血量 %（默认 65）、耗蓝层数上限（默认 2）以及跳过普攻可及目标的选项；Auto R 开关（U）有独立层数上限（默认 3），且只要存在任何可普攻的敌人就不会发射。耗蓝层数通过官方 8 秒窗口跟踪自身施放（每层 +40，上限 400），每次自动 R 都检查蓝量是否足够。
- 处决数学内置：每 1% 已损失生命值 +0.833%（最高 ×1.5），40% 生命值以下按官方 ×2 计算，R 抢头因此精确。W 攻击特效（%最大生命值，野怪上限 100）也计入可击杀指示。
- 附带确定击杀的 Q 补刀（炮车/超级兵优先，可跳过普攻可及小兵，含野怪）、按最少命中数的 E 清线、Semi R（空格）/Semi E（G），以及 W 期间的扩展攻击距离圆圈绘制。
<!-- MESH-AIO:RELEASE:v2.15.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
