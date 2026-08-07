<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.23.0:START -->
## v2.23.0

### 한국어

#### 지원 챔피언

공식 16.15 데이터 기준 173챔피언 전체를 지원합니다. 아래는 세부 상태 머신을
직접 제작한 전용 모듈 28개이며, 나머지 145챔피언은 각자의 행동 계약을 공용
엔진에서 실행합니다.

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

- 버전 v2.23.0에서 173개 `profile.lua` 전부에 Combo/Harass/Farm/Flee/Reactive/Weave 순서, 실행 동작, 상태·자원 특성 계약을 추가했습니다. 공식 목록과 173/173 일치하지 않으면 빌드가 실패합니다.
- 현재 계약은 실행 동작 440개와 상태·정책 특성 275개입니다. 공용 145챔피언은 하나의 전역 Q/W/E/R 순서 대신 자기 계약을 실제로 읽고, 전용 28챔피언은 기존 실측 상태 머신을 유지합니다.
- 각 공용 챔피언은 필요한 수동·강제·커서·아군·처형·자동·일시정지·스킬→점멸·점멸→스킬·벽 동작만 `Champion Actions`에 표시합니다. 새 키는 기본 미지정이며 dropdown + `Set LMB`로 배정합니다.
- 공식 `mClientData.mTargeterDefinitions`의 Line/Cone/Aoe/Range 사거리·반경·폭을 일반식으로 읽어 누락되거나 잘못 생성되던 판정을 복구했습니다. 글로벌 R과 이동속도 기반 동적 사거리도 공식 계약으로 고정했습니다.
- FXT 173파일은 라이선스 미확인 읽기 전용 행동 자료로만 감사했습니다. 파일·함수·상수·수치·구형 API는 복사하지 않았고 Riot 고정 데이터와 현재 Hanbot API로 독립 구현했습니다.
- 새 다단계·점멸 동작은 정적 검사와 Lua 5.1 검사를 통과했지만 라이브 서버 타이밍은 F12 확인 대상입니다. 버프·스택·무기·소환물처럼 live 상태가 필요한 기능은 추측 시전하지 않고 안전하게 닫힙니다.

#### Aatrox

- Q의 공식 850/400 판정과 E 300/50 판정을 nested targeter에서 복구하고, 수동 W·Q→점멸·Q 단계 상태 계약을 프로필에 추가했습니다.

#### Aphelios

- 무기 상태 특성을 보존하면서 수동 Q/R, 강제 R, 자동 W 일시정지 동작을 독립 키로 노출했습니다.

#### Jayce

- 자세 상태와 정확한 live form을 기준으로 수동 Q/EQ, 커서 EQ, E→점멸, 강제 E, 자동 R 일시정지 계약을 추가했습니다.

#### Seraphine

- R의 공식 1300/160 판정을 복구하고 수동 E/R, E·R→점멸, 패시브 일시정지, 이중 시전·에코 상태를 기록했습니다.

#### Sett

- W 공식 805/210 판정을 복구하고 수동 W/E/EW/R, W→점멸, 점멸→E/R, 강제 R과 W 조준 보정 계약을 추가했습니다.

#### Sion

- Q의 공식 750/180 판정을 복구하고 W·E→점멸, Q 충전, R 조향 상태를 공용 계약에 반영했습니다.

#### TwistedFate

- Q의 공식 1400/40 판정을 복구하고 수동 Q/W, 카드 색 선택, 카드 평타 위빙·공격 일시정지 상태를 분리했습니다.

#### Warwick

- R 사거리를 이동속도 x2.5, 최대 2500으로 계산하고 수동 R, Q→점멸, 점멸→E, 강제 Q와 Q 홀드 상태를 추가했습니다.

#### Yasuo

- 커서 E, 자동 R, Q→점멸, EQ→점멸, E 모드, Q 스택과 대상별 돌진 표식 계약을 추가했습니다.

#### Zeri

- Q 평타 상태를 보존하면서 수동 W, 자동 Q, 강제 Q→Q, 커서 방향 벽 E를 추가했습니다. 지형 확인이 필요한 W/E는 자동 조준으로 추측하지 않습니다.

### English

#### Supported Champions

All 173 champions are supported on the official 16.15 data. The following 28
use hand-tuned state machines; the other 145 execute their own behaviour
contracts through the shared engine.

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

- Version v2.23.0 gives all 173 `profile.lua` files independent Combo, Harass, Farm, Flee, Reactive, and Weave orders plus executable actions and state/resource traits. Generation fails unless the catalog matches the official roster 173/173.
- The catalog contains 440 executable actions and 275 state/policy traits. The 145 shared champions consume their own contracts instead of one global Q/W/E/R order, while the 28 dedicated champions retain their measured state machines.
- Each shared champion exposes only its relevant manual, force, cursor, ally, execute, auto, pause, spell-to-Flash, Flash-to-spell, and wall actions under `Champion Actions`. New bindings default to unassigned and support dropdown + `Set LMB` mapping.
- General extraction of official Line/Cone/Aoe/Range geometry from `mClientData.mTargeterDefinitions` restores missing or incorrect targeting. Global ultimates and movement-speed-scaled ranges are also pinned as official contracts.
- The 173 FXT files were used only as unlicensed, read-only behavioural references. No file, function, constant, numeric value, or legacy API was copied; Riot-pinned data and the current Hanbot API drive the independent implementation.
- New multi-step and Flash actions pass static and Lua 5.1 validation, but their live server timing remains an F12 test item. Buff-, stack-, weapon-, and summon-dependent logic fails closed instead of guessing live state.

#### Aatrox

- Restored official 850/400 Q and 300/50 E geometry from nested targeters, then added Manual W, Q-to-Flash, and Q-stage contracts.

#### Aphelios

- Preserved weapon-state traits while exposing Manual Q/R, Force R, and Pause Automatic W as independent actions.

#### Jayce

- Added stance-aware Manual Q/EQ, Cursor EQ, E-to-Flash, Force E, and Pause Automatic R contracts against exact live forms.

#### Seraphine

- Restored official 1300/160 R geometry and recorded Manual E/R, E/R-to-Flash, passive pause, double-cast, and Echo behaviour.

#### Sett

- Restored official 805/210 W geometry and added Manual W/E/EW/R, W-to-Flash, Flash-to-E/R, Force R, and W-adjustment contracts.

#### Sion

- Restored official 750/180 Q geometry and added W/E-to-Flash, Q-charge, and R-steering contracts.

#### TwistedFate

- Restored official 1400/40 Q geometry and separated Manual Q/W, card selection, card-attack weaving, and attack-pause state.

#### Warwick

- R now uses movement speed x2.5 up to 2500, with Manual R, Q-to-Flash, Flash-to-E, Force Q, and Q-hold contracts.

#### Yasuo

- Added Cursor E, Auto R, Q-to-Flash, EQ-to-Flash, E mode, Q stacks, and per-target dash-mark contracts.

#### Zeri

- Preserved Q-as-attack state while adding Manual W, Auto Q, Force Q-to-Q, and cursor-directed wall E. Terrain-dependent W/E stays fail-closed for automatic aim.

### 简体中文

#### 支持英雄

基于官方 16.15 数据支持全部 173 位英雄。以下 28 位使用手工状态机；其余 145 位
通过共用引擎执行各自的行为契约。

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

- v2.23.0 为全部 173 个 `profile.lua` 加入独立的 Combo、Harass、Farm、Flee、Reactive、Weave 顺序，以及执行动作和状态/资源特性；契约目录若未与官方名单 173/173 完全一致，生成会失败。
- 当前目录包含 440 个可执行动作和 275 个状态/策略特性。145 个共用英雄读取自己的契约，不再使用单一全局 Q/W/E/R 顺序；28 个专属英雄保留实测状态机。
- 每位共用英雄只在 `Champion Actions` 中显示自己需要的手动、强制、鼠标方向、队友、斩杀、自动、暂停、技能→闪现、闪现→技能和翻墙动作。新按键默认未绑定，可通过下拉框与 `Set LMB` 分配。
- 现在会从官方 `mClientData.mTargeterDefinitions` 统一提取 Line/Cone/Aoe/Range 的距离、半径和宽度，修复缺失或错误的目标几何；全图大招和移速动态距离也固定为官方契约。
- FXT 的 173 个文件仅作为无许可证的只读行为参考。没有复制文件、函数、常量、数值或旧 API；独立实现只使用锁定的 Riot 数据和当前 Hanbot API。
- 新增多段与闪现动作已通过静态及 Lua 5.1 检查，但实时服务器时序仍需 F12 验证。依赖增益、层数、武器和召唤物的逻辑在状态不明时会安全拒绝。

#### Aatrox

- 从嵌套目标数据恢复 Q 的官方 850/400 与 E 的 300/50 几何，并加入手动 W、Q→闪现和 Q 阶段契约。

#### Aphelios

- 保留武器状态特性，同时把手动 Q/R、强制 R、暂停自动 W 作为独立动作开放。

#### Jayce

- 按精确实时形态加入姿态相关的手动 Q/EQ、鼠标 EQ、E→闪现、强制 E 和暂停自动 R 契约。

#### Seraphine

- 恢复 R 的官方 1300/160 几何，并记录手动 E/R、E/R→闪现、被动暂停、双重施法与回响行为。

#### Sett

- 恢复 W 的官方 805/210 几何，并加入手动 W/E/EW/R、W→闪现、闪现→E/R、强制 R 和 W 调整契约。

#### Sion

- 恢复 Q 的官方 750/180 几何，并加入 W/E→闪现、Q 蓄力与 R 转向契约。

#### TwistedFate

- 恢复 Q 的官方 1400/40 几何，并拆分手动 Q/W、选牌、卡牌普攻穿插与攻击暂停状态。

#### Warwick

- R 现在按移速 x2.5 计算且最高 2500，并加入手动 R、Q→闪现、闪现→E、强制 Q 与 Q 长按契约。

#### Yasuo

- 加入鼠标 E、自动 R、Q→闪现、EQ→闪现、E 模式、Q 层数和目标冲刺标记契约。

#### Zeri

- 保留 Q 作为攻击的状态，同时加入手动 W、自动 Q、强制 Q→Q 与鼠标方向墙体 E；依赖地形的 W/E 不会自动猜测瞄准。
<!-- MESH-AIO:RELEASE:v2.23.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
