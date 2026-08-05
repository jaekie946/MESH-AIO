<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.16.0:START -->
## v2.16.0

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

- 버전: v2.16.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지하며, 전용 모듈이 25개(공용 148)로 늘었습니다.
- Kalista가 25번째 전용 모듈로 승격되었습니다. 공식 16.15 원본 수치 15개 항목이 자동 회귀 검사에 고정되었습니다.

#### Kalista

- 신규 전용 모듈: 평-Q-평 위빙으로 파열의 창을 쌓고, **E는 처치 확정일 때** 나갑니다. 창 스택은 적 버프 스캔 우선에 자체 4초 평타 추적 폴백입니다.
- E 경로: 챔피언 처치(항상), 표식 미니언을 E로 죽여 쿨 초기화하면서 표식 챔피언에게 피해+슬로우를 함께 넣는 루난 추격 콤보(콤보 중 자동), E 사거리(1000)를 벗어나려는 표식 챔피언 대상 창 개수 기반 덤프, 견제 덤프(옵션), 그리고 최소 처치 수 기반 팜 E(정글 포함, 에픽 몬스터 공식 50% 반영)입니다.
- Q는 첫 유닛에 막히지만 처치 시 창이 관통·전이되므로, 경로의 미니언이 **전부 Q에 죽으면** 자동 Q를 통과시키는 관통 게이트가 있습니다(스택 전이 콤보).
- 추격(Pursuit): 콤보 대상이 평타 사거리 밖이면 주변 미니언/정글/식물(타워는 옵션, 기본 꺼짐)을 공격해 패시브 도약으로 계속 따라갑니다.
- 벽넘기 키(X): 커서 방향으로 이동하며 도약 거리(330) 안에 벽과 반대편 착지점이 있으면 Q를 시전해 패시브 도약으로 벽을 넘습니다(착지 미리보기 드로우 포함).
- W는 5000 사거리 시야 파수꾼입니다: Semi W(G)는 바론/드래곤 둥지 중 가까운 곳으로 발사하고, 자동 모드(기본 꺼짐)는 주변 적 없음 확인+둥지 거리 슬라이더+둥지별 60초 스로틀을 지킵니다.
- R는 결속(서약) 아군 소환입니다: 결속 아군이 1000 사거리 안에서 체력 슬라이더 이하 + 주변 적 수 조건일 때 자동 구출하고, Semi R(Space)도 제공합니다.
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

- Version: v2.16.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data; hand-tuned modules grow to 25 (shared-engine 148).
- Kalista is promoted to the 25th dedicated module. 15 official 16.15 raw values are pinned into the automated regression checks.

#### Kalista

- New dedicated module: AA-Q-AA weaving stacks Rend spears, and **E fires when the payout kills**. Spear counts read the enemy buff first with an own-attack 4-second tracker as fallback.
- E paths: champion kill (always), the Runaan chase combo - killing a marked minion with E resets the cooldown while the marked champion eats the damage and slow (automatic inside Combo) - a spear-count dump on a marked champion escaping the 1000 tether, an optional harass dump, and farm E at the minimum-kills slider (jungle included, epic monsters at the official 50%).
- Q stops on the first unit, but a kill passes the spear on - so the pierce gate lets automatic Q through blocking minions when they ALL die to it (the stack-transfer combo).
- Pursuit: when the Combo champion is out of attack reach, nearby minions/jungle/plants (turrets optional, off by default) are attacked so the Martial Poise hop keeps chasing.
- Wall key (X): walks toward the cursor and casts Q when a wall with a passable landing sits inside the 330 hop, jumping thin walls on the passive hop (with a landing preview drawing).
- W is the 5000-range vision sentinel: Semi W (G) fires at the nearest Baron/Dragon pit, and the default-off auto mode adds a no-enemy guard, a pit-distance slider, and a per-pit 60-second throttle.
- R recalls the Oath-sworn ally: auto rescue when the bound ally inside the 1000 range drops under the HP slider with enough enemies around, plus Semi R (Space).
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

- 版本：v2.16.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄；专属模块增至 25 个（共用引擎 148 个）。
- 卡莉丝塔晋升为第 25 个专属模块，15 项官方 16.15 原始数值已固定进自动回归检查。

#### Kalista

- 新专属模块：普攻-Q-普攻编织叠加撕裂之矛，**E 在确定击杀时释放**。矛层数优先读取敌方 Buff，并以自身 4 秒普攻跟踪作为兜底。
- E 的路径：击杀英雄（始终）、卢安追击连招——用 E 杀死带矛小兵刷新冷却，同时带矛英雄吃到伤害和减速（连招中自动）——对将要脱离 1000 范围的带矛英雄按矛数滑条倾泻、可选的骚扰倾泻，以及按最少击杀数的清线 E（含野怪，史诗野怪按官方 50% 计算）。
- Q 会被第一个单位挡住，但击杀后长矛会穿透传递——因此当路径上的小兵**全部会被 Q 击杀**时，穿透门允许自动 Q 通过（层数传递连招）。
- 追击（Pursuit）：连招目标超出普攻距离时，攻击附近的小兵/野怪/植物（防御塔为选项，默认关闭），借助战争律动的跳跃持续追击。
- 翻墙键（X）：朝光标移动，当 330 跳跃距离内存在墙体且对面有可落地点时施放 Q，借被动跳跃翻越薄墙（附落点预览绘制）。
- W 是 5000 射程的视野哨兵：Semi W（G）射向最近的男爵/巨龙巢穴；自动模式（默认关闭）附带无敌人确认、巢穴距离滑条和每巢穴 60 秒节流。
- R 召回誓约绑定的队友：绑定队友在 1000 范围内、血量低于滑条且周围敌人数达标时自动救援，另有 Semi R（空格）。
<!-- MESH-AIO:RELEASE:v2.16.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
