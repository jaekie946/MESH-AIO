<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.21.1:START -->
## v2.21.1

### 한국어

#### 지원 챔피언

공식 16.15 데이터 기준 173챔피언 전체를 지원합니다. 아래는 세부 로직을 직접 제작한 전용 모듈 28개이며, 나머지 챔피언은 공용 엔진 베이스라인으로 동작합니다.

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
- 트리스타나
- 베인
- 제라스
- 유나라

#### 핵심 및 메뉴

- 버전: v2.21.1. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준 173챔피언 지원에서 전용 모듈이 28개(공용 145)로 늘었습니다.
- Tristana가 28번째 전용 모듈로 승격되었습니다. 공식 16.15 원본 수치 15개 항목이 자동 회귀 검사에 고정되었습니다.
- 파이크 Q가 신뢰도 게이트를 얻었습니다: 명중 확정 각이 없으면 풀차지 후에도 유지하다가 각이 나오면 발사하고, 끝까지 없으면 공식 3초 만료(마나 환급)로 흘려보냅니다. 허공 발사가 구조적으로 사라집니다.

#### Tristana

- 신규 전용 모듈(28번째): **W는 도주기 전용**입니다(사용자 계약). Flee(Z) 중 커서 방향, Semi 키 N에서만 공식 900으로 점프하며 콤보/갭클로즈 사용은 없습니다.
- E 폭발 화약: 550 대상 시전 후 **내 평타 4번으로 기폭**(스택당 +25%, 치명타 계수 0.4). 시전+자기 평타 카운트로 자체 추적하고 버프 스캔으로 보정하며, **부착 대상 머리 위에 실시간 스택(E n/4)을 표시**합니다 — R+기폭 합계로 처치 가능하면 빨간색.
- Q 속사: 공속 버프 순수 시전(평타 리셋 아님). 콤보/견제(사거리 내 적), 라인클리어(웨이브 수 슬라이더), 구조물 공격 중에 윈드업을 보호하며 사용합니다.
- R 대구경 탄환: 처치 확정(E→R 기폭 합산 옵션), 저체력 셀프 필(넉백), 나에게 착지하는 돌진 밀쳐내기, 채널 인터럽트(공유 DB), Flee 저체력, Semi R(Space). 구조물 공격 중 E 타워 옵션도 있습니다.
- 공식 수치 15개 계약 고정: Q 공속 60~120%/7초, W 70~210+1.0추가AD+0.5AP(350 광역), E 60~160+0.8추가AD+0.5AP·스택당 25%·처치 폭발 45~105, R 225/275/325+1.0AP·넉백 600/800/1000.

#### Pyke

- Q 작살이 신뢰도 게이트를 얻었습니다: 명중 확정 각(정지/탈출 불가/경로 확정)이 없으면 **풀차지 후에도 홀드**하며 매 틱 재평가하고, 각이 나오는 순간 발사합니다. 끝까지 없으면 공식 3초 만료로 흘려 마나를 환급받습니다 — 기존의 풀차지 즉시 허공 발사가 사라집니다(옵션 기본 켜짐).

#### Gangplank

- 콤보 Q가 정상 로테이션으로 돌아왔습니다: 기존의 "처형 전용" 제한(통이 하나라도 있으면 챔피언 직접 Q 금지)을 제거해, 통 플레이가 없는 틱마다 Q 견제가 나갑니다(통 우선 옵션은 유지).
- 연계 통 선설치를 완전히 제거했습니다: 기존 통이 풀피일 때 미리 깔린 연장 통은 적이 부수거나 보고 피했습니다. 이제 모든 연장 통은 기존 통이 피 1을 읽는 순간의 E-Q-E 변환으로만, Q/퓨즈가 이미 날아가는 중에 착지합니다.
- 3개 이상 통 연쇄를 지원합니다: 충전이 있으면 사거리에 필요한 만큼(최대 3연장) 퓨즈 진행에 맞춰 공식 0.5초 간격으로 이어 설치하며, 각 다음 통은 실시간 대상 방향으로 한 링크씩 나아갑니다.

### English

#### Supported Champions

All 173 champions are supported on the official 16.15 data. The list below is the 28 hand-tuned dedicated modules; every other champion runs on the shared-engine baseline.

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
- Tristana
- Vayne
- Xerath
- Yunara

#### Core & Menu

- Version: v2.21.1. On Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data, the dedicated modules grow to 28 (shared-engine 145) out of the 173 supported champions.
- Tristana is promoted to the 28th dedicated module. 15 official 16.15 raw values are pinned into the automated regression checks.
- Pyke Q gains a reliability gate: with no confirmed-hit angle the charge HOLDS past full growth, releases the moment an angle shows, and otherwise lets the official 3 s expiry refund the mana - open-air hooks are structurally gone.

#### Tristana

- New dedicated module (the 28th): **W is an ESCAPE TOOL only** (user contract) - it jumps the official 900 toward the cursor in Flee (Z) and on the Semi key N; no combo or gapclose W exists.
- E Explosive Charge: a 550 unit cast that **four of OUR basic attacks detonate** (+25% per stack, 0.4 x crit modifier). Self-tracked from the cast plus own-attack counting with a buff-scan correction, and the **live stack count draws over the charged target's head** (E n/4) - red once the R + detonation total kills.
- Q Rapid Fire is cast purely as the attack-speed buff (not an attack reset): Combo/Harass with an enemy in attack reach, lane clear at the wave-size slider, and while attacking structures, always protecting the windup.
- R Buster Shot: confirmed kills (optionally counting the attached E detonation, E -> R), low-health self peel (knockback), knocking back dashes landing on Tristana, channel interrupts (shared DB), Flee under an HP slider, and Semi R (Space). E also lands on structures while attacking them.
- 15 official values pinned: Q attack speed 60-120% for 7 s, W 70-210 +1.0 bonus AD +0.5 AP (350 splash), E 60-160 +0.8 bonus AD +0.5 AP with 25% per stack and the 45-105 death explosion, R 225/275/325 +1.0 AP with 600/800/1000 knockback.

#### Pyke

- Q gains a reliability gate: with no confirmed-hit angle (stationary / cannot-escape / committed path) the charge **HOLDS past full growth**, re-evaluating every tick and releasing the moment an angle shows. If none ever does, the official 3 s expiry refunds the mana - the old full-charge dump into open air is gone (option default on).

#### Gangplank

- Combo Q is back in the normal rotation: the old execute-only gate (no direct Q on champions while any keg existed) is removed, so Q pokes whenever no keg play fires this tick (the barrel-first preference stays).
- Early extension kegs are gone entirely: a follow-up keg on the ground while the anchor was still full HP got broken or side-stepped. Every extension keg now lands ONLY through the E-Q-E conversion at the moment the anchor reads 1 HP, while the Q/fuse is already in the air.
- Chains of three or more kegs connect: with the charges available, follow-ups keep landing on the official 0.5 s spacing along the LIVE target direction, one link at a time, up to three extensions.

### 简体中文

#### 支持英雄

基于官方 16.15 数据支持全部 173 位英雄。下方为 28 个手工制作的专属模块；其余英雄由共用引擎基线驱动。

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
- 麦林炮手
- 暗夜猎手
- 远古巫灵
- 不破之誓

#### 核心与菜单

- 版本：v2.21.1。基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄，专属模块增至 28 个（共用引擎 145 个）。
- 麦林炮手晋升为第 28 个专属模块，15 项官方 16.15 原始数值已固定进自动回归检查。
- 圣枪游侠的 Q 获得可靠性门槛：没有确定命中的角度时满蓄力也继续保持，出现角度立即释放；始终没有则交给官方 3 秒到期退还法力——结构性消灭对空放钩。

#### Tristana

- 新专属模块（第 28 个）：**W 仅作逃生技**（用户契约）——只在 Flee（Z）朝光标方向、以及 Semi 键 N 上按官方 900 跳跃，不存在连招/突进用法。
- E 爆炸火药：550 码单位施放后**由我方 4 次普攻引爆**（每层 +25%，暴击系数 0.4）。以施放+自身普攻计数自行跟踪并用 buff 扫描校正，**在被附着目标头顶实时显示层数（E n/4）**——R+引爆总伤足以击杀时变红。
- Q 急速射击为纯攻速增益施放（非普攻重置）：连招/骚扰（攻击范围内有敌人）、清线（兵数滑条）、攻击建筑时使用，始终保护普攻前摇。
- R 大口径弹头：确认击杀（可选计入附着 E 引爆，E→R）、低血量自保击退、击退扑向自己的突进、打断引导（共享数据库）、Flee 低血量、Semi R（空格）。攻击建筑时也可对建筑上 E。
- 固定 15 项官方数值：Q 攻速 60~120%/7 秒，W 70~210 +1.0 额外 AD +0.5 AP（350 溅射），E 60~160 +0.8 额外 AD +0.5 AP、每层 25%、死亡爆炸 45~105，R 225/275/325 +1.0 AP、击退 600/800/1000。

#### Pyke

- Q 获得可靠性门槛：没有确定命中角度（静止/无法逃离/路径已定）时**满蓄力也继续保持**，每帧重估，出现角度立即释放；始终没有则交给官方 3 秒到期退还法力——旧的满蓄力对空放钩不复存在（选项默认开启）。
#### Gangplank

- 连招 Q 回归正常循环：移除旧的"仅处决"限制（场上有桶时禁止对英雄直接 Q），当帧没有火药桶连携时即可用 Q 消耗（保留桶优先选项）。
- 彻底移除提前铺设的衔接桶：锚桶还是满血时提前放的延长桶会被敌人打掉或绕开。现在所有延长桶只通过 E-Q-E 转换落地——即锚桶读到 1 血、Q/引信已在空中的那一刻。
- 支持三个以上火药桶连锁：充能足够时按官方 0.5 秒间隔沿实时目标方向逐节续放，最多三节延长。
<!-- MESH-AIO:RELEASE:v2.21.1:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
