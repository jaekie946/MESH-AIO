<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

<!-- MESH-AIO:UPDATES:START -->
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
