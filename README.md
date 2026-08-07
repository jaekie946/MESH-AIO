<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.24.0:START -->
## v2.24.0

### 한국어

#### 지원 챔피언

- 올라프
- 르블랑
- 블라디미르
- 시비르
- 소라카
- 티모
- 트리스타나
- 미스 포츈
- 애쉬
- 트위치
- 카서스
- 이렐리아
- 갱플랭크
- 코르키
- 케이틀린
- 블리츠크랭크
- 말파이트
- 엘리스
- 오리아나
- 베인
- 카시오페아
- 이즈리얼
- 모데카이저
- 아칼리
- 가렌
- 말자하
- 탈론
- 리븐
- 코그모
- 제라스
- 아리
- 렝가
- 바루스
- 빅토르
- 드레이븐
- 카직스
- 신드라
- 카이사
- 야스오
- 탈리야
- 진
- 제리
- 징크스
- 루시안
- 제드
- 키아나
- 사미라
- 쓰레쉬
- 일라오이
- 칼리스타
- 자야
- 아펠리오스
- 파이크
- 요네
- 멜
- 유나라
- 로크
- 오로라
- 밀리오
- 자헨
- 흐웨이

#### 핵심 및 메뉴

- v2.24.0은 Riot 16.15.1/클라이언트 16.15 기준 173챔피언을 수작업 전용 28개, 생성 전용 33개, 공용 112개로 실행합니다.
- NG-AIO 10개는 모두 전용입니다. 기존 이즈리얼·칼리스타·로크 상태 머신은 보존하고, 일라오이·이렐리아·카서스·멜·블라디미르·야스오·제드는 현재 Hanbot API와 공식 데이터로 상태 로직을 이식했습니다.
- HGVip/CXJ/Q-Aio는 라이선스가 확인되지 않아 코드를 복사하지 않았습니다. 둘 이상 자료에서 독립적으로 확인된 26개 챔피언만 생성 전용으로 승격하고, 위험한 재시전·방어기·궁극기는 상태를 확인할 수 없으면 자동 시전을 거부합니다.
- 생성 전용 메뉴는 감사 출처와 기능 계약, 챔피언별 실동작 옵션을 표시하며 기존 Semi Q/W/E/R, Champion Actions, LMB 키 지정 기능을 그대로 사용합니다.
- 현재 스킬 슬롯 이름을 공식 raw 형태 1,004개(재시전 269·변신/강화 23·충전 23·평타 리셋 75)와 매 틱 대조하고, 동일 alias는 정확한 mScriptName을 우선해 각 시전 방식으로 분기합니다.
- Elise·Jayce·Nidalee 양방향 변신, Rek'Sai 잠복, Aphelios 무기 전환, Hwei 팔레트뿐 아니라 Sylas의 훔친 궁과 Viego 빙의 슬롯도 공식 전체 카탈로그에서 현재 이름으로 찾습니다.
- 공식 타게팅 계약이 불명확한 형태는 자동 시전을 막고 세미키만 허용하며, 궁극기와 변신 자동 사용은 기본 OFF로 두었습니다.
- 공식 평타 리셋 태그가 있는 형태는 평타 선딜을 보존한 뒤 첫 유효 백스윙에서 요청하고, 거부된 유효 요청만 1ms 스크립트 하한으로 재시도합니다.
- OP.GG 16.15 공개 페이지의 173챔피언 스킬 우선순위와 사용자 팁을 robots.txt 허용 확인 후 별도 보조 캐시에 저장했으며, 수치와 시전 형태는 Riot 원본만 기준으로 사용합니다.

#### Olaf

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 axe_pickup·q_magnet·low_hp_w 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### Vladimir

- NG-AIO+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 empowered_q·e_charge·e_release·pool_block·multi_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→R→W 순서를 유지합니다.

#### Sivir

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_return·w_reset·spellshield 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### MissFortune

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_swap·q_bounce·channel_r 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Ashe

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_weave·cone_w·global_r 계약을 연결했습니다. 공식 형태 6개와 전투 W→Q→E→R 순서를 유지합니다.

#### Twitch

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 poison·stealth_return·e_execute·r_line 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Karthus

- NG-AIO+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 isolated_q·aura_hysteresis·mana_reserve·passive_r·global_r 계약을 연결했습니다. 공식 형태 15개와 전투 E→Q→W→R 순서를 유지합니다.

#### Irelia

- NG-AIO+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_reset·marked_q·minion_gapclose·e_two_stage·w_block·multi_r 계약을 연결했습니다. 공식 형태 8개와 전투 E→R→Q→W 순서를 유지합니다.

#### Corki

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 missile_ammo·big_one·package_state 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Caitlyn

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 headshot·trap_cc·net_recoil·global_execute 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Blitzcrank

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 hook_collision·e_reset·interrupt_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Elise

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 stance·spiderlings·rappel_state 계약을 연결했습니다. 공식 형태 11개와 전투 Q→W→E→R 순서를 유지합니다.

#### Cassiopeia

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 poison_e·miasma_dash·facing_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Ezreal

- NG-AIO의 초반 패시브 유지 결정을 현재 API로 옮겨, 실시간 `ezrealpassivestacks` 종료와 Q 비행시간이 만나는 66ms 구간에만 미니언 Q를 사용하도록 추가했습니다. 옵션은 기본 OFF입니다.

#### Mordekaiser

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_ring·isolated_q·realm_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Varus

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_charge·blight·w_execute·chain_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Viktor

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 e_vector·w_cc·r_follow·hex_fragments 계약을 연결했습니다. 공식 형태 5개와 전투 E→Q→W→R 순서를 유지합니다.

#### Draven

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 axe_catch·axe_renewal·global_r 계약을 연결했습니다. 공식 형태 7개와 전투 Q→W→E→R 순서를 유지합니다.

#### Khazix

- HGVip+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 evolution·isolation·safe_e 계약을 연결했습니다. 공식 형태 10개와 전투 Q→W→E→R 순서를 유지합니다.

#### Kaisa

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 evolution·plasma·isolated_q·safe_r 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Yasuo

- NG-AIO+HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_stack·dash_marks·minion_dash·eq·eq_flash·windwall·knockup_r 계약을 연결했습니다. 공식 형태 13개와 전투 Q→E→W→R 순서를 유지합니다.

#### Taliyah

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 worked_ground·w_vector·e_dash·channel_r 계약을 연결했습니다. 공식 형태 9개와 전투 Q→E→W→R 순서를 유지합니다.

#### Zeri

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_attack·charged_passive·wall_w·wall_e·r_effectiveness 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Lucian

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_weave·extended_q·r_magnet 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Zed

- NG-AIO+CXJ 교차 감사로 생성 전용 진입점에 승격하고 shadow_tracking·multi_origin_q·shadow_e·weq·death_mark·safe_swap 계약을 연결했습니다. 공식 형태 8개와 전투 R→W→E→Q 순서를 유지합니다.

#### Samira

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 style·melee_q·projectile_w·dash_reset·r_gate 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Thresh

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_recast·lantern_ally·e_direction 계약을 연결했습니다. 공식 형태 8개와 전투 Q→E→W→R 순서를 유지합니다.

#### Illaoi

- NG-AIO 교차 감사로 생성 전용 진입점에 승격하고 spirit_priority·w_attack_reset·heartsteel_wait·multi_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Xayah

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 feathers·e_root·r_reposition 계약을 연결했습니다. 공식 형태 4개와 전투 E→W→Q→R 순서를 유지합니다.

#### Aphelios

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 weapon_state·mark_range·weapon_swap 계약을 연결했습니다. 공식 형태 11개와 전투 Q→E→W→R 순서를 유지합니다.

#### Yone

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_stack·spirit_return·safe_r 계약을 연결했습니다. 공식 형태 6개와 전투 Q→E→W→R 순서를 유지합니다.

#### Mel

- NG-AIO+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 multi_q·reserve_w·reflect_lethal·e_setup·r_reserve 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→R→W 순서를 유지합니다.

#### Milio

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 ally_shield·interrupt_q·cleanse_r 계약을 연결했습니다. 공식 형태 5개와 전투 E→W→Q→R 순서를 유지합니다.

#### Zaahen

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 recast_state·resource·execute 계약을 연결했습니다. 공식 형태 6개와 전투 Q→E→W→R 순서를 유지합니다.

### English

#### Supported Champions

- Olaf
- LeBlanc
- Vladimir
- Sivir
- Soraka
- Teemo
- Tristana
- Miss Fortune
- Ashe
- Twitch
- Karthus
- Irelia
- Gangplank
- Corki
- Caitlyn
- Blitzcrank
- Malphite
- Elise
- Orianna
- Vayne
- Cassiopeia
- Ezreal
- Mordekaiser
- Akali
- Garen
- Malzahar
- Talon
- Riven
- Kog'Maw
- Xerath
- Ahri
- Rengar
- Varus
- Viktor
- Draven
- Kha'Zix
- Syndra
- Kai'Sa
- Yasuo
- Taliyah
- Jhin
- Zeri
- Jinx
- Lucian
- Zed
- Qiyana
- Samira
- Thresh
- Illaoi
- Kalista
- Xayah
- Aphelios
- Pyke
- Yone
- Mel
- Yunara
- Locke
- Aurora
- Milio
- Zaahen
- Hwei

#### Core & Menu

- v2.24.0 runs all 173 champions from Riot 16.15.1/client 16.15 as 28 hand-tuned, 33 generated-specialist, and 112 shared entries.
- All ten NG-AIO champions are dedicated. Existing Ezreal, Kalista, and Locke state machines remain intact; Illaoi, Irelia, Karthus, Mel, Vladimir, Yasuo, and Zed now use current-API specialist state logic.
- HGVip/CXJ/Q-Aio had no supplied reuse license, so no code was copied. Only 26 champions independently corroborated by at least two archives were promoted, with unsafe recasts, defensive spells, and ultimates failing closed when state is unknown.
- Specialist menus expose audit sources, feature contracts, and connected champion options while retaining Semi Q/W/E/R, Champion Actions, and LMB key assignment.
- Matches each live slot name against 1,004 official raw forms (recast 269, transform/upgrade 23, charge 23, attack reset 75) every tick, preferring an exact mScriptName when aliases overlap.
- Covers both directions of Elise, Jayce, and Nidalee transformations, Rek'Sai burrow, Aphelios weapon swaps, Hwei palettes, Sylas stolen ultimates, and Viego possession slots through the full official catalog.
- Forms with an ambiguous official targeting contract stay semi-manual only, while automatic ultimates and transformations remain disabled by default.
- Official attack-reset forms preserve the auto-attack windup, cast on the first valid backswing callback, and retry only valid rejected requests with a 1 ms script-local floor.
- Archived skill priorities and user-tip summaries for all 173 champions from OP.GG 16.15 after verifying robots.txt permission; Riot data remains the sole authority for numbers and cast forms.

#### Olaf

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with axe_pickup, q_magnet, low_hp_w; it retains 5 official forms and the Q→E→W→R combat order.

#### Vladimir

- Promoted to a dedicated specialist entry after NG-AIO+Q-Aio review, with empowered_q, e_charge, e_release, pool_block, multi_r; it retains 4 official forms and the Q→E→R→W combat order.

#### Sivir

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_return, w_reset, spellshield; it retains 4 official forms and the Q→W→E→R combat order.

#### MissFortune

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with passive_swap, q_bounce, channel_r; it retains 5 official forms and the Q→W→E→R combat order.

#### Ashe

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_weave, cone_w, global_r; it retains 6 official forms and the W→Q→E→R combat order.

#### Twitch

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with poison, stealth_return, e_execute, r_line; it retains 4 official forms and the E→Q→W→R combat order.

#### Karthus

- Promoted to a dedicated specialist entry after NG-AIO+CXJ+Q-Aio review, with isolated_q, aura_hysteresis, mana_reserve, passive_r, global_r; it retains 15 official forms and the E→Q→W→R combat order.

#### Irelia

- Promoted to a dedicated specialist entry after NG-AIO+CXJ review, with q_reset, marked_q, minion_gapclose, e_two_stage, w_block, multi_r; it retains 8 official forms and the E→R→Q→W combat order.

#### Corki

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with missile_ammo, big_one, package_state; it retains 4 official forms and the Q→E→W→R combat order.

#### Caitlyn

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with headshot, trap_cc, net_recoil, global_execute; it retains 5 official forms and the Q→W→E→R combat order.

#### Blitzcrank

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with hook_collision, e_reset, interrupt_r; it retains 4 official forms and the Q→E→W→R combat order.

#### Elise

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with stance, spiderlings, rappel_state; it retains 11 official forms and the Q→W→E→R combat order.

#### Cassiopeia

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with poison_e, miasma_dash, facing_r; it retains 4 official forms and the E→Q→W→R combat order.

#### Ezreal

- Ported NG-AIO's early passive refresh decision to the current API: minion Q is requested only in the 66 ms window where travel time lands before `ezrealpassivestacks` expires. The option defaults off.

#### Mordekaiser

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with passive_ring, isolated_q, realm_r; it retains 4 official forms and the Q→E→W→R combat order.

#### Varus

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_charge, blight, w_execute, chain_r; it retains 4 official forms and the Q→W→E→R combat order.

#### Viktor

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with e_vector, w_cc, r_follow, hex_fragments; it retains 5 official forms and the E→Q→W→R combat order.

#### Draven

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with axe_catch, axe_renewal, global_r; it retains 7 official forms and the Q→W→E→R combat order.

#### Khazix

- Promoted to a dedicated specialist entry after HGVip+Q-Aio review, with evolution, isolation, safe_e; it retains 10 official forms and the Q→W→E→R combat order.

#### Kaisa

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with evolution, plasma, isolated_q, safe_r; it retains 7 official forms and the Q→E→W→R combat order.

#### Yasuo

- Promoted to a dedicated specialist entry after NG-AIO+HGVip+CXJ review, with q_stack, dash_marks, minion_dash, eq, eq_flash, windwall, knockup_r; it retains 13 official forms and the Q→E→W→R combat order.

#### Taliyah

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with worked_ground, w_vector, e_dash, channel_r; it retains 9 official forms and the Q→E→W→R combat order.

#### Zeri

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_attack, charged_passive, wall_w, wall_e, r_effectiveness; it retains 4 official forms and the Q→E→W→R combat order.

#### Lucian

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with passive_weave, extended_q, r_magnet; it retains 4 official forms and the Q→E→W→R combat order.

#### Zed

- Promoted to a dedicated specialist entry after NG-AIO+CXJ review, with shadow_tracking, multi_origin_q, shadow_e, weq, death_mark, safe_swap; it retains 8 official forms and the R→W→E→Q combat order.

#### Samira

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with style, melee_q, projectile_w, dash_reset, r_gate; it retains 7 official forms and the Q→E→W→R combat order.

#### Thresh

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with q_recast, lantern_ally, e_direction; it retains 8 official forms and the Q→E→W→R combat order.

#### Illaoi

- Promoted to a dedicated specialist entry after NG-AIO review, with spirit_priority, w_attack_reset, heartsteel_wait, multi_r; it retains 4 official forms and the E→Q→W→R combat order.

#### Xayah

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with feathers, e_root, r_reposition; it retains 4 official forms and the E→W→Q→R combat order.

#### Aphelios

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with weapon_state, mark_range, weapon_swap; it retains 11 official forms and the Q→E→W→R combat order.

#### Yone

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_stack, spirit_return, safe_r; it retains 6 official forms and the Q→E→W→R combat order.

#### Mel

- Promoted to a dedicated specialist entry after NG-AIO+CXJ+Q-Aio review, with multi_q, reserve_w, reflect_lethal, e_setup, r_reserve; it retains 4 official forms and the E→Q→R→W combat order.

#### Milio

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with ally_shield, interrupt_q, cleanse_r; it retains 5 official forms and the E→W→Q→R combat order.

#### Zaahen

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with recast_state, resource, execute; it retains 6 official forms and the Q→E→W→R combat order.

### 简体中文

#### 支持英雄

- 狂战士
- 诡术妖姬
- 猩红收割者
- 战争女神
- 众星之子
- 迅捷斥候
- 麦林炮手
- 赏金猎人
- 寒冰射手
- 瘟疫之源
- 死亡颂唱者
- 刀锋舞者
- 海洋之灾
- 英勇投弹手
- 皮城女警
- 蒸汽机器人
- 熔岩巨兽
- 蜘蛛女皇
- 发条魔灵
- 暗夜猎手
- 魔蛇之拥
- 探险家
- 铁铠冥魂
- 离群之刺
- 德玛西亚之力
- 虚空先知
- 刀锋之影
- 放逐之刃
- 深渊巨口
- 远古巫灵
- 九尾妖狐
- 傲之追猎者
- 惩戒之箭
- 奥术先驱
- 荣耀行刑官
- 虚空掠夺者
- 暗黑元首
- 虚空之女
- 疾风剑豪
- 岩雀
- 戏命师
- 祖安花火
- 暴走萝莉
- 圣枪游侠
- 影流之主
- 元素女皇
- 沙漠玫瑰
- 魂锁典狱长
- 海兽祭司
- 复仇之矛
- 逆羽
- 残月之肃
- 血港鬼影
- 封魔剑魂
- 流光镜影
- 不破之誓
- 灰烬驱魔人
- 双界灵兔
- 明烛
- 不落魔锋
- 异画师

#### 核心与菜单

- v2.24.0 依据 Riot 16.15.1/客户端 16.15 支持全部 173 位英雄：28 个手工专属、33 个生成专属、112 个共用入口。
- NG-AIO 的 10 位英雄全部使用专属入口；保留伊泽瑞尔、卡莉丝塔、洛克的现有状态机，并为俄洛伊、艾瑞莉娅、卡尔萨斯、梅尔、弗拉基米尔、亚索、劫加入当前 API 状态逻辑。
- HGVip/CXJ/Q-Aio 未附带可复用许可证，因此没有复制代码；仅将至少两个资料独立确认的 26 位英雄升级为生成专属，未知状态下会拒绝危险的再施法、防御技能与终极技能。
- 专属菜单显示审计来源、功能契约和已连接的英雄选项，同时保留 Semi Q/W/E/R、Champion Actions 与 LMB 按键分配。
- 每个 tick 将当前技能槽名称与 1,004 个官方 raw 形态（再施法 269、变身/强化 23、蓄力 23、普攻重置 75）匹配；别名重叠时优先精确 mScriptName。
- 通过完整官方目录覆盖伊莉丝、杰斯、奈德丽双向变身、雷克塞遁地、厄斐琉斯换枪、慧的画板、塞拉斯偷取终极技能和佛耶戈附身后的技能槽。
- 官方目标类型不明确的形态只允许半自动按键，自动使用终极技能和自动变身默认关闭。
- 带官方普攻重置标签的形态会保留普攻前摇，在第一个有效后摇回调施法，并仅对有效但被拒绝的请求按 1 毫秒脚本下限重试。
- 在确认 robots.txt 允许后，离线保存 OP.GG 16.15 的 173 位英雄技能优先级和用户技巧摘要；技能数值与施法形态仍只以 Riot 原始数据为准。

#### Olaf

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 axe_pickup、q_magnet、low_hp_w，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### Vladimir

- 经 NG-AIO+Q-Aio 交叉审计后升级为专属入口，加入 empowered_q、e_charge、e_release、pool_block、multi_r，并保留 4 个官方形态与 Q→E→R→W 战斗顺序。

#### Sivir

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_return、w_reset、spellshield，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### MissFortune

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_swap、q_bounce、channel_r，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Ashe

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_weave、cone_w、global_r，并保留 6 个官方形态与 W→Q→E→R 战斗顺序。

#### Twitch

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 poison、stealth_return、e_execute、r_line，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Karthus

- 经 NG-AIO+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 isolated_q、aura_hysteresis、mana_reserve、passive_r、global_r，并保留 15 个官方形态与 E→Q→W→R 战斗顺序。

#### Irelia

- 经 NG-AIO+CXJ 交叉审计后升级为专属入口，加入 q_reset、marked_q、minion_gapclose、e_two_stage、w_block、multi_r，并保留 8 个官方形态与 E→R→Q→W 战斗顺序。

#### Corki

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 missile_ammo、big_one、package_state，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Caitlyn

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 headshot、trap_cc、net_recoil、global_execute，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Blitzcrank

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 hook_collision、e_reset、interrupt_r，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Elise

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 stance、spiderlings、rappel_state，并保留 11 个官方形态与 Q→W→E→R 战斗顺序。

#### Cassiopeia

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 poison_e、miasma_dash、facing_r，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Ezreal

- 将 NG-AIO 的前期被动续层判断迁移到当前 API：只有当 Q 飞行时间能在 `ezrealpassivestacks` 结束前命中的 66 毫秒窗口内，才会对小兵施放 Q；该选项默认关闭。

#### Mordekaiser

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_ring、isolated_q、realm_r，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Varus

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_charge、blight、w_execute、chain_r，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Viktor

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 e_vector、w_cc、r_follow、hex_fragments，并保留 5 个官方形态与 E→Q→W→R 战斗顺序。

#### Draven

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 axe_catch、axe_renewal、global_r，并保留 7 个官方形态与 Q→W→E→R 战斗顺序。

#### Khazix

- 经 HGVip+Q-Aio 交叉审计后升级为专属入口，加入 evolution、isolation、safe_e，并保留 10 个官方形态与 Q→W→E→R 战斗顺序。

#### Kaisa

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 evolution、plasma、isolated_q、safe_r，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Yasuo

- 经 NG-AIO+HGVip+CXJ 交叉审计后升级为专属入口，加入 q_stack、dash_marks、minion_dash、eq、eq_flash、windwall、knockup_r，并保留 13 个官方形态与 Q→E→W→R 战斗顺序。

#### Taliyah

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 worked_ground、w_vector、e_dash、channel_r，并保留 9 个官方形态与 Q→E→W→R 战斗顺序。

#### Zeri

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_attack、charged_passive、wall_w、wall_e、r_effectiveness，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Lucian

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_weave、extended_q、r_magnet，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Zed

- 经 NG-AIO+CXJ 交叉审计后升级为专属入口，加入 shadow_tracking、multi_origin_q、shadow_e、weq、death_mark、safe_swap，并保留 8 个官方形态与 R→W→E→Q 战斗顺序。

#### Samira

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 style、melee_q、projectile_w、dash_reset、r_gate，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Thresh

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 q_recast、lantern_ally、e_direction，并保留 8 个官方形态与 Q→E→W→R 战斗顺序。

#### Illaoi

- 经 NG-AIO 交叉审计后升级为专属入口，加入 spirit_priority、w_attack_reset、heartsteel_wait、multi_r，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Xayah

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 feathers、e_root、r_reposition，并保留 4 个官方形态与 E→W→Q→R 战斗顺序。

#### Aphelios

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 weapon_state、mark_range、weapon_swap，并保留 11 个官方形态与 Q→E→W→R 战斗顺序。

#### Yone

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_stack、spirit_return、safe_r，并保留 6 个官方形态与 Q→E→W→R 战斗顺序。

#### Mel

- 经 NG-AIO+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 multi_q、reserve_w、reflect_lethal、e_setup、r_reserve，并保留 4 个官方形态与 E→Q→R→W 战斗顺序。

#### Milio

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 ally_shield、interrupt_q、cleanse_r，并保留 5 个官方形态与 E→W→Q→R 战斗顺序。

#### Zaahen

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 recast_state、resource、execute，并保留 6 个官方形态与 Q→E→W→R 战斗顺序。
<!-- MESH-AIO:RELEASE:v2.24.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
