<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.22.0:START -->
## v2.22.0

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

- 버전: v2.22.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준 173챔피언 지원(전용 28, 공용 145)을 유지합니다.
- 공용 엔진에 Evade 우선권, 실제 live spell 피해 기반 처치 확정, 돌진 도착시간 안티갭, 주 대상을 보존하는 다중 적중 조준, 이동기 착지 검증과 아군 체력 임계값을 추가했습니다.
- 공용 Hotkeys에 Semi Q/W/E/R, `J` Auto Q, `X1MB` 수동 이동기/벽넘기, 자동 시전 일시정지를 정리했습니다. Last Hit 중에는 Auto Q가 작동하지 않고, 일시정지는 자동 주문만 막아 기본 오브워커 이동과 공격은 유지합니다.
- 공용 메뉴와 전용 28개 메뉴에 dropdown + `Set LMB` 버튼을 추가했습니다. 이미 구현된 수동 동작을 골라 왼쪽 마우스에 배정하며, 존재하지 않는 keybind를 선택지에 넣으면 정적 검사가 실패합니다.
- FXT 173개 챔피언 파일은 라이선스 미확인 읽기 전용 행동 자료로만 전수 감사했습니다. 파일·함수·상수·구형 API는 배포물에 복사하지 않았습니다.

#### Annie

- E를 적 대상 주문으로 오분류하던 생성 프로필을 아군/자기 보호 주문으로 바로잡아 공용 콤보가 적에게 시전하려는 경로를 차단했습니다.

#### Jayce

- 완전한 Q→E 상태 연계 없이 Acceleration Gate만 자동 시전하지 않도록 fail-closed 처리했습니다. 수동 Semi E는 그대로 사용할 수 있습니다.

#### Jhin

- Evade가 활성인 틱에는 치명타 재시도와 Semi/채널 로직보다 먼저 반환하도록 전용 pre-tick 안전 순서를 보강했고, 기존 수동 키를 LMB로 배정할 수 있게 했습니다.

#### Malphite

- Evade 활성 중에는 Flee·Semi·자동 시전이 주문을 내지 않도록 전용 모듈을 공용 틱 소유권 표준에 맞추고, Semi 키 LMB 배정 버튼을 추가했습니다.

#### Pyke

- Evade가 Q 차징·E 이동·점멸 연계보다 먼저 틱을 소유하도록 보강했으며, Semi Q/R과 Delivery/E-Flash 키를 메뉴에서 LMB로 재지정할 수 있습니다.

#### Soraka

- Evade가 활성인 동안 Force E, Flee, 자동 치유·반응 주문이 실행되지 않도록 했고, Force E와 Flee 키를 LMB 선택기에 연결했습니다.

#### Teemo

- Evade 중 Semi/Flee/함정 로직이 이동·시전 주문을 내지 않도록 안전 게이트를 앞당기고, Semi Q/R·일시정지·Flee 키의 LMB 배정을 지원합니다.

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

- Version: v2.22.0. Support remains at 173 champions (28 dedicated and 145 shared) on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- The shared engine gains Evade ownership, exact live-spell damage kill confirmation, arrival-timed anti-gapclose, primary-preserving multi-hit aim, mobility landing validation, and ally-health thresholds.
- Shared Hotkeys now organize Semi Q/W/E/R, `J` Auto Q, `X1MB` manual mobility/wall hop, and a pause-automatic-casts action. Auto Q stays out of Last Hit, while pause suppresses script automation without stopping native orbwalker movement or attacks.
- The shared menu and all 28 dedicated menus gain a dropdown plus `Set LMB` button. It binds the left mouse button to an existing manual action, and static validation rejects any selector entry without a declared keybind.
- All 173 FXT champion files were audited only as unlicensed, read-only behavioural references. No file, function, constant, or legacy API was copied into the package.

#### Annie

- The generated profile now classifies E as an ally/self protection spell instead of an enemy spell, preventing the shared combo engine from trying to cast it on opponents.

#### Jayce

- Acceleration Gate now fails closed for automation until a complete Q-to-E state sequence exists. Manual Semi E remains available.

#### Jhin

- The dedicated pre-tick now yields to active Evade before critical-retry, Semi, or channel logic, and its existing manual actions can be assigned to LMB.

#### Malphite

- The dedicated module now emits no Flee, Semi, or automatic spell orders while Evade is active, and its Semi actions are available in the LMB selector.

#### Pyke

- Evade now owns the tick before Q charging, E movement, or Flash sequences; Semi Q/R and Delivery/E-Flash actions can be rebound to LMB from the menu.

#### Soraka

- Force E, Flee, automatic healing, and reactive casts now yield while Evade is active, and Force E/Flee are connected to the LMB selector.

#### Teemo

- The safety gate now prevents Semi, Flee, and trap logic from issuing orders during active Evade, while Semi Q/R, pause, and Flee can be assigned to LMB.

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

- 版本：v2.22.0。基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端数据，继续支持 173 位英雄（28 个专属模块、145 个共用模块）。
- 共用引擎新增 Evade 行动优先权、实时技能伤害斩杀确认、按突进到达时间触发的反突进、保留主目标的多目标瞄准、位移落点验证与队友生命阈值。
- 共用快捷键现在包含 Semi Q/W/E/R、`J` 自动 Q、`X1MB` 手动位移/翻墙，以及暂停自动施法。补刀模式会阻止自动 Q，暂停只阻止脚本自动订单，不会停止原生走砍移动和普攻。
- 共用菜单和全部 28 个专属菜单新增下拉框与 `Set LMB` 按钮，可把已有手动动作绑定到鼠标左键；选择器若引用未声明的 keybind，静态检查会直接失败。
- FXT 的 173 个英雄文件仅作为无许可证的只读行为参考进行审查，未把文件、函数、常量或旧 API 复制进发布包。

#### Annie

- 生成配置已把 E 修正为队友/自身保护技能，不再误判成对敌技能，避免共用连招尝试向敌人施放。

#### Jayce

- 在完整 Q→E 状态连招实现前，加速之门的自动路径现在默认关闭；手动 Semi E 仍可正常使用。

#### Jhin

- 专属 pre-tick 会在暴击重试、Semi 或大招引导逻辑前先让出给活动中的 Evade，现有手动动作也可绑定到 LMB。

#### Malphite

- Evade 活动时专属模块不再发出逃跑、Semi 或自动技能订单，并在 LMB 选择器中提供现有 Semi 动作。

#### Pyke

- Evade 现在优先于 Q 蓄力、E 位移和闪现连招；Semi Q/R 与 Delivery/E-Flash 动作可在菜单中改绑到 LMB。

#### Soraka

- Evade 活动时 Force E、逃跑、自动治疗与反应施法都会让出，并把 Force E 和逃跑键接入 LMB 选择器。

#### Teemo

- 安全门会阻止 Semi、逃跑和蘑菇逻辑在 Evade 活动时发出订单，同时支持把 Semi Q/R、暂停与逃跑动作绑定到 LMB。
<!-- MESH-AIO:RELEASE:v2.22.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
