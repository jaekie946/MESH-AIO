<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.19.0:START -->
## v2.19.0

### 한국어

#### 지원 챔피언

공식 16.15 데이터 기준 173챔피언 전체를 지원합니다. 아래는 세부 로직을 직접 제작한 전용 모듈 27개이며, 나머지 챔피언은 공용 엔진 베이스라인으로 동작합니다.

- 아리
- 아칼리
- 오로라
- 이즈리얼
- 갱플랭크
- 가렌
- 흐웨이
- 진
- 징크스
- 칼리스타
- 코그모
- 르블랑
- 로크
- 말파이트
- 말자하
- 오리아나
- 파이크
- 키아나
- 렝가
- 리븐
- 소라카
- 신드라
- 탈론
- 티모
- 베인
- 제라스
- 유나라

#### 핵심 및 메뉴

- 버전: v2.19.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원을 유지하며, 전용 모듈이 27개(공용 146)로 늘었습니다.
- Jinx가 27번째 전용 모듈로 승격되었습니다. 공식 16.15 원본 수치 21개 항목이 자동 회귀 검사에 고정되었습니다.
- 릴리즈 노트의 지원 챔피언 목록이 직접 제작한 전용 모듈만 나열하도록 바뀌었습니다(어떤 챔피언이 수제작인지 한눈에 보이도록). 나머지 챔피언의 공용 엔진 지원은 그대로입니다.

#### Jinx

- 신규 전용 모듈: **거리 기반 Q 폼 전환이 핵심**입니다. 미니건이 닿는 대상은 미니건(최대 DPS·공속 스택), 미니건 밖·로켓 사거리(기본 525+랭크별 100~200) 안 대상은 로켓으로 자동 전환합니다. 전환은 0.4초 스로틀과 평타 윈드업 보호를 지킵니다.
- 팜 폼 관리: 웨이브가 미니건 안이면 미니건 유지, 로켓으로만 닿는 막타/스플래시(250, 최소 명중 슬라이더) 상황에서만 마나 게이트 하에 로켓. 전투 대상이 없으면 미니건 복귀(패시브 절약).
- W(1450, 첫 유닛 정지)는 평타가 닿는 대상에게 쓰지 않는 옵션(기본 켜짐)과 함께 콤보/견제/킬스틸/스테이시스 저격을 담당합니다. 수동 W는 T.
- E 와작와작 덫은 반응 전용입니다: 나에게 착지하는 돌진 길목, 하드 CC 대상, 채널링 인터럽트, Flee 추격 저지. 수동 E는 G.
- R는 글로벌 처형입니다: 사거리 슬라이더(기본 2300) 안에서 거리 램프(바닥→최대)+잃은 체력 비례를 정직하게 계산해 처치 확정일 때만 발사합니다. 수동 R는 Space.

#### Soraka

- 칼바람 실전 피드백: 자동 R가 체력 조건만으로 나가지 않도록, R를 받을 아군이 **전투 중일 때만**(최근 2.5초 내 피해를 입었거나 주변 900 안에 적 챔피언) 발동하는 게이트를 추가했습니다(기본 켜짐, 끌 수 있음).

### English

#### Supported Champions

All 173 champions are supported on the official 16.15 data. The list below is the 27 hand-tuned dedicated modules; every other champion runs on the shared-engine baseline.

- Ahri
- Akali
- Aurora
- Ezreal
- Gangplank
- Garen
- Hwei
- Jhin
- Jinx
- Kalista
- Kog'Maw
- LeBlanc
- Locke
- Malphite
- Malzahar
- Orianna
- Pyke
- Qiyana
- Rengar
- Riven
- Soraka
- Syndra
- Talon
- Teemo
- Vayne
- Xerath
- Yunara

#### Core & Menu

- Version: v2.19.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data; hand-tuned modules grow to 27 (shared-engine 146).
- Jinx is promoted to the 27th dedicated module. 21 official 16.15 raw values are pinned into the automated regression checks.
- The Supported-Champions list in these notes now names only the hand-tuned dedicated modules, so it is obvious which champions are hand-made; shared-engine coverage for everyone else is unchanged.

#### Jinx

- New dedicated module where the **distance-based Q form switch is the core**: minigun on anything the minigun reaches (max DPS, attack-speed stacks), rockets only for targets between minigun reach and the rocket range (base 525 + rank 100..200), throttled and windup-protected.
- Farm form management: stay on the minigun while the wave is in minigun reach; rockets only for last hits or splash clears (official 250, minimum-hits slider) beyond it, behind a mana gate; return to minigun when idle.
- W (1450, stops on the first unit) covers combo/harass/killsteal/stasis snipes with an option (default on) to never W a target the basic attack reaches. Manual W on T.
- The E chompers are reactive only: the landing of a dash onto Jinx, hard-CCed targets, channel interrupts, and Flee peel. Manual E on G.
- R is the global execute: inside the range slider (2300 default) it computes the distance ramp (floor to max) plus the missing-health payout honestly and fires only on a confirmed kill. Manual R on Space.

#### Soraka

- ARAM field feedback: automatic R no longer fires on the HP condition alone - the ally receiving it must be IN COMBAT (damaged within the last 2.5 s or an enemy champion within 900), default on and toggleable.

### 简体中文

#### 支持英雄

基于官方 16.15 数据支持全部 173 位英雄。下方为 27 个手工制作的专属模块；其余英雄由共用引擎基线驱动。

- 九尾妖狐
- 离群之刺
- 双界灵兔
- 探险家
- 海洋之灾
- 德玛西亚之力
- 异画师
- 戏命师
- 暴走萝莉
- 复仇之矛
- 深渊巨口
- 诡术妖姬
- 灰烬驱魔人
- 熔岩巨兽
- 虚空先知
- 发条魔灵
- 血港鬼影
- 元素女皇
- 傲之追猎者
- 放逐之刃
- 众星之子
- 暗黑元首
- 刀锋之影
- 迅捷斥候
- 暗夜猎手
- 远古巫灵
- 不破之誓

#### 核心与菜单

- 版本：v2.19.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄；专属模块增至 27 个（共用引擎 146 个）。
- 金克丝晋升为第 27 个专属模块，21 项官方 16.15 原始数值已固定进自动回归检查。
- 更新说明中的支持英雄列表现在只列出手工制作的专属模块，一眼可见哪些英雄是手工打造；其余英雄的共用引擎支持不变。

#### Jinx

- 新专属模块，**按距离切换 Q 形态是核心**：机枪够得着的目标用机枪（最大 DPS、攻速叠层），仅在机枪射程外、火箭射程（基础 525 + 每级 100~200）内的目标切换火箭；切换有 0.4 秒节流并保护普攻前摇。
- 清线形态管理：兵线在机枪范围内保持机枪；只有火箭才够得着的补刀/溅射清线（官方 250，最少命中滑条）才在蓝量门槛下切火箭；空闲时切回机枪。
- W（1450，命中第一个单位即停）负责连招/骚扰/抢头/凝滞狙击，并有默认开启的"普攻可及目标不放 W"选项。手动 W 为 T。
- E 火焰咀嚼者仅作反应使用：扑向金克丝的突进落点、硬控目标、打断引导、Flee 反追。手动 E 为 G。
- R 是全图处决：在射程滑条（默认 2300）内诚实计算距离斜坡（下限到上限）加已损生命加成，仅在确定击杀时发射。手动 R 为空格。

#### Soraka

- 大乱斗实战反馈：自动 R 不再仅凭血量条件释放——接受 R 的队友必须**处于战斗中**（最近 2.5 秒内受到伤害，或 900 范围内有敌方英雄），默认开启且可关闭。
<!-- MESH-AIO:RELEASE:v2.19.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
