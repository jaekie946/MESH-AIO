<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.20.0:START -->
## v2.20.0

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

- 버전: v2.20.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언 지원과 전용 27/공용 146 구조를 유지합니다.
- 이번 릴리즈는 실전 로그로 확인된 전용 모듈 3종(칼리스타·아리·제라스)의 사용자 동작 수정과 표시 기능 추가가 중심입니다.
- 스킬-플래시 연계(로크 Q플 계열)의 콜백 순서 표준이 확정되었습니다: 플래시 예약을 시전 이전에 등록해야 동기 콜백에서도 연계가 발동합니다. 아리·제라스가 이 표준으로 정렬되었습니다.

#### Kalista

- Q 벽넘기 키가 X에서 프로젝트 표준 월점프 키 X1MB로 이동했습니다(콤보 계열 키와의 충돌 제거).
- Flee(Z) 도주 중 도주 경로에 넘을 수 있는 벽이 있으면 자동으로 Q 홉으로 넘어갑니다. 벽 착지점 표시는 벽넘기 키뿐 아니라 Flee 중에도 그려집니다.
- E(파열) 예상 피해를 대상 위에 퍼센트로 표시하는 옵션이 추가되었습니다(Drawings > Rend damage percent, 기본 켜짐). 챔피언은 실드 포함 체력 대비, 정글 몬스터도 전부 표시하며 처치 가능(100% 이상)이면 빨간색으로 바뀝니다. 처치 가능 원 표시도 정글 몬스터(바론/드래곤 E 스틸 판단)까지 확장되었습니다.

#### Ahri

- E-플래시(A)가 원거리 대상에게 E만 발사하고 플래시가 따라붙지 않던 문제를 수정했습니다. 플래시 예약이 시전 이후에 등록되어 동기 콜백이 빈손으로 돌던 순서 버그로, 이제 E 윈드업 중 플래시가 정상 연계됩니다.
- R 진입(콤보 옵션)이 켜져 있어도 발동하지 않던 문제를 수정했습니다. 충전 수 판독이 실패하면 "마지막 대시 보존" 기본 옵션이 모든 진입을 차단했는데, 공식 15초 3회 재시전 창을 자체 추적해 첫 R가 준비된 상태를 3충전으로 올바르게 인식합니다.
- 도주 W(Use in Flee)가 적 근접(900) 조건 없이, 옵션이 켜져 있고 Z를 누르면 준비 즉시 시전됩니다(감쇠 이속을 도주 시작부터 활용).

#### Xerath

- E-플래시(G)에 아리와 동일한 콜백 순서 버그가 잠복해 있어 같은 방식으로 수정했습니다. 윈드업 중 플래시 연계가 코드 경로상 복구되었습니다.

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

- Version: v2.20.0. 173-champion support stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data, with the 27 dedicated / 146 shared-engine split unchanged.
- This release focuses on user-visible behavior fixes and new displays for three dedicated modules (Kalista, Ahri, Xerath), all confirmed from live game logs.
- The spell-into-Flash callback ordering standard (the Locke Q-Flash family) is now settled: the Flash reservation must be registered BEFORE the cast so a synchronous callback still fires the link. Ahri and Xerath are aligned to it.

#### Kalista

- The Q wall-hop key moved from X to the project-standard wall-jump key X1MB (removes the collision with combo-family keys).
- While fleeing (Z), a hoppable wall on the escape path now triggers the Q hop automatically; the wall landing marker draws during Flee as well as on the wall key.
- New display: Rend (E) damage as a percent over each target (Drawings > Rend damage percent, default on). Champions are measured against health plus shields, jungle monsters are all covered, and the text turns red once lethal (100%+). The killable circle also extends to jungle monsters (Baron/Dragon E steals at a glance).

#### Ahri

- Fixed E-Flash (A) firing only the E at faraway targets with no Flash following: the Flash reservation was registered after the cast, so a synchronous callback found nothing pending. The Flash now links during the E wind-up.
- Fixed R engage never firing with the combo option on: when the charge count could not be read, the default "never spend the final dash" option blocked every engage. The official 15-second three-recast window is now self-tracked, so a fresh R correctly reads as three charges.
- Flee W (Use in Flee) now casts the moment W is ready while Z is held with the option on - the enemy-within-900 gate is gone, so the decaying haste starts with the escape.

#### Xerath

- E-Flash (G) carried the same latent callback-ordering bug as Ahri and received the same fix; the Flash link during the E wind-up is restored on the code path.

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

- 版本：v2.20.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄，专属 27 / 共用引擎 146 的结构不变。
- 本次更新聚焦三个专属模块（复仇之矛、九尾妖狐、远古巫灵）经实战日志确认的用户可见行为修复与新显示功能。
- 技能接闪现（洛克 Q 闪系列）的回调顺序标准已确定：闪现预约必须在施放之前登记，同步回调才能触发衔接。九尾妖狐与远古巫灵已按此标准对齐。

#### Kalista

- Q 翻墙键从 X 移至项目标准跳墙键 X1MB（消除与连招系键位的冲突）。
- Flee（Z）逃跑时，逃跑路径上有可翻越的墙会自动用 Q 跳跃翻越；墙体落点标记在 Flee 期间与翻墙键期间都会绘制。
- 新增显示：在目标上方以百分比显示 E（撕裂）预计伤害（Drawings > Rend damage percent，默认开启）。英雄按含护盾生命计算，野怪全部覆盖，可击杀（100% 以上）时文字变红；可击杀圆圈也扩展到野怪（男爵/巨龙 E 抢夺一目了然）。

#### Ahri

- 修复 E 闪（A）对远处目标只发 E、闪现不跟随的问题：闪现预约登记在施放之后，同步回调扑空。现在 E 前摇期间闪现正常衔接。
- 修复开启连招选项后 R 仍不进场的问题：充能数读取失败时，默认的"保留最后一段位移"选项会拦截所有进场。现改为自行跟踪官方 15 秒三段重施窗口，新 R 就绪时正确识别为三充能。
- 逃跑 W（Use in Flee）不再要求 900 范围内有敌人——选项开启且按住 Z 时，W 就绪即刻施放（衰减加速从逃跑开始就生效）。

#### Xerath

- E 闪（G）潜伏着与九尾妖狐相同的回调顺序问题，已用同样方式修复；E 前摇期间的闪现衔接在代码路径上恢复。
<!-- MESH-AIO:RELEASE:v2.20.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
