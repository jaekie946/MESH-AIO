<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.25.0:START -->
## v2.25.0

### 한국어

#### 지원 챔피언

- 애니
- 올라프
- 트위스티드 페이트
- 신 짜오
- 르블랑
- 블라디미르
- 케일
- 알리스타
- 사이온
- 시비르
- 소라카
- 티모
- 트리스타나
- 미스 포츈
- 애쉬
- 잭스
- 모르가나
- 트위치
- 카서스
- 초가스
- 아무무
- 문도 박사
- 카사딘
- 이렐리아
- 갱플랭크
- 코르키
- 트런들
- 스웨인
- 케이틀린
- 블리츠크랭크
- 말파이트
- 카타리나
- 녹턴
- 엘리스
- 오리아나
- 브랜드
- 리 신
- 베인
- 럼블
- 카시오페아
- 나서스
- 뽀삐
- 판테온
- 이즈리얼
- 모데카이저
- 아칼리
- 케넨
- 가렌
- 레오나
- 말자하
- 탈론
- 리븐
- 코그모
- 럭스
- 제라스
- 쉬바나
- 아리
- 그레이브즈
- 렝가
- 바루스
- 노틸러스
- 빅토르
- 피오라
- 직스
- 룰루
- 드레이븐
- 카직스
- 다리우스
- 제이스
- 리산드라
- 다이애나
- 신드라
- 케인
- 조이
- 카이사
- 세라핀
- 자크
- 야스오
- 벨코즈
- 탈리야
- 브라움
- 진
- 킨드레드
- 제리
- 징크스
- 탐 켄치
- 세나
- 루시안
- 제드
- 키아나
- 바이
- 아트록스
- 나미
- 유미
- 사미라
- 쓰레쉬
- 일라오이
- 칼리스타
- 바드
- 자야
- 사일러스
- 니코
- 아펠리오스
- 렐
- 파이크
- 요네
- 암베사
- 멜
- 유나라
- 로크
- 릴리아
- 그웬
- 레나타 글라스크
- 오로라
- 닐라
- 스몰더
- 밀리오
- 자헨
- 흐웨이
- 나피리

#### 핵심 및 메뉴

- v2.25.0은 Riot 16.15.1/클라이언트 16.15 기준 현대 챔피언 173명을 수작업 전용 28개, 생성 전용 92개, 공용 53개로 실행하며 League Classic(JADE) 출시 명단 60명도 별도 구형 키트 프로필로 지원합니다.
- 사용자가 코드 활용을 허가한 NG-AIO/HGVip/CXJ/Q-Aio/FXT를 전수 비교해 해당 자료가 지원하는 현대 챔피언은 모두 전용 범주로 승격했습니다. 복원본 자체를 로드하지 않고 현재 Hanbot API와 Riot 원본에 맞춘 생성 프로필·상태 게이트로 이식합니다.
- 새 Source Guard는 자료에서 수동·방어용으로 분류된 재시전, 생존기, 궁극기를 실시간 형태를 확인할 수 없을 때 자동으로 추측 시전하지 않습니다.
- JADE는 런타임 챔피언 이름을 현대 기본 alias로 매핑하되 FXT의 59개 구형 스킬 형상을 적용합니다. FXT에 모듈이 없던 Rammus는 라이브 이름 확인 전까지 현대 프로필 안전 폴백을 사용합니다.
- 수작업 28개도 자료와 다시 비교했습니다. Tristana는 E 부착 대상을 평타 우선 대상으로 즉시 재지정하고, 현재 최대 DPS·안전 교리보다 불리한 구형 A-Q-A 또는 공격형 W 패턴은 채택하지 않았습니다.
- 생성 전용 메뉴는 감사 출처와 기능 계약, 챔피언별 실동작 옵션을 표시하며 기존 Semi Q/W/E/R, Champion Actions, LMB 키 지정 기능을 그대로 사용합니다.
- 현재 스킬 슬롯 이름을 공식 raw 형태 1,004개(재시전 269·변신/강화 23·충전 23·평타 리셋 75)와 매 틱 대조하고, 동일 alias는 정확한 mScriptName을 우선해 각 시전 방식으로 분기합니다.
- Elise·Jayce·Nidalee 양방향 변신, Rek'Sai 잠복, Aphelios 무기 전환, Hwei 팔레트뿐 아니라 Sylas의 훔친 궁과 Viego 빙의 슬롯도 공식 전체 카탈로그에서 현재 이름으로 찾습니다.
- 공식 타게팅 계약이 불명확한 형태는 자동 시전을 막고 세미키만 허용하며, 궁극기와 변신 자동 사용은 기본 OFF로 두었습니다.
- 공식 평타 리셋 태그가 있는 형태는 평타 선딜을 보존한 뒤 첫 유효 백스윙에서 요청하고, 거부된 유효 요청만 1ms 스크립트 하한으로 재시도합니다.
- OP.GG 16.15 공개 페이지의 173챔피언 스킬 우선순위와 사용자 팁을 robots.txt 허용 확인 후 별도 보조 캐시에 저장했으며, 수치와 시전 형태는 Riot 원본만 기준으로 사용합니다.

#### Annie

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 mode_farm·manual_q·manual_r·flash_after_w·flash_before_r·force_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Olaf

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 axe_pickup·q_magnet·low_hp_w·mode_q·magnet_q·state_axe 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### TwistedFate

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_card_gold·state_card_blue·state_card_red·state_attack_reset·state_card_attack_pause·state_card_attack_weave·manual_q·manual_w 계약을 연결했습니다. 공식 형태 8개와 전투 Q→W→E→R 순서를 유지합니다.

#### XinZhao

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_w_adjust·manual_w·flash_after_w·force_w·force_e 계약을 연결했습니다. 공식 형태 4개와 전투 W→E→Q→R 순서를 유지합니다.

#### Vladimir

- NG-AIO+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 empowered_q·e_charge·e_release·pool_block·multi_r·state_empowered_q·state_e_charge·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→R→W 순서를 유지합니다.

#### Kayle

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_auto_heal·ally_r 계약을 연결했습니다. 공식 형태 7개와 전투 E→Q→W→R 순서를 유지합니다.

#### Alistar

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_w·manual_wq·flash_after_q·flash_after_wq·flash_before_qw 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Sion

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_q_charge·state_r_steer·flash_after_w·flash_after_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Sivir

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_return·w_reset·spellshield·magnet_q·manual_q·auto_q·flash_after_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Tristana

- HGVip/CXJ/Q-Aio 비교에서 확인한 E 폭탄 대상 집중을 현재 오브워커 API로 이식했습니다. 폭탄 대상이 평타 사거리 안이면 그 틱의 공격 대상을 즉시 재지정하며, 대상이 사라지거나 사거리를 벗어나면 고착 없이 해제됩니다.

#### MissFortune

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_swap·q_bounce·channel_r·state_passive_logic·manual_w·manual_r·pause_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Ashe

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_weave·cone_w·global_r·cursor_e·manual_r 계약을 연결했습니다. 공식 형태 6개와 전투 W→Q→E→R 순서를 유지합니다.

#### Jax

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 block_e·safe_q·force_q 계약을 연결했습니다. 공식 형태 4개와 전투 W→E→Q→R 순서를 유지합니다.

#### Morgana

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Twitch

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 poison·stealth_return·e_execute·r_line·state_stealth_return·state_poison·manual_w·pause_e 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Karthus

- NG-AIO+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 isolated_q·aura_hysteresis·mana_reserve·passive_r·global_r·mode_first_strike·manual_w 계약을 연결했습니다. 공식 형태 15개와 전투 E→Q→W→R 순서를 유지합니다.

#### Chogath

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 farm_e·manual_q·flash_after_w 계약을 연결했습니다. 공식 형태 6개와 전투 E→Q→W→R 순서를 유지합니다.

#### Amumu

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 farm_no_q·manual_q·flash_after_q 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### DrMundo

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_q·auto_q 계약을 연결했습니다. 공식 형태 6개와 전투 Q→E→W→R 순서를 유지합니다.

#### Kassadin

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 safe_mobility·farm_q·manual_q·auto_q·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 E→W→Q→R 순서를 유지합니다.

#### Irelia

- NG-AIO+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_reset·marked_q·minion_gapclose·e_two_stage·w_block·multi_r·safe_farm_turret·state_q_reset·manual_r·flash_after_r·force_q 계약을 연결했습니다. 공식 형태 8개와 전투 E→R→Q→W 순서를 유지합니다.

#### Corki

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 missile_ammo·big_one·package_state·manual_q·manual_r·auto_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Trundle

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_e_push·state_e_pull·manual_e·manual_r 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Swain

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 magnet_e·state_soul_fragment·manual_w·manual_e·flash_after_q 계약을 연결했습니다. 공식 형태 6개와 전투 Q→W→E→R 순서를 유지합니다.

#### Caitlyn

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 headshot·trap_cc·net_recoil·global_execute·state_reverse_e·manual_q·manual_w·manual_e·flash_after_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Blitzcrank

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 hook_collision·e_reset·interrupt_r·manual_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Katarina

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 safe_farm_turret·state_daggers·auto_q·pause_e 계약을 연결했습니다. 공식 형태 8개와 전투 Q→E→W→R 순서를 유지합니다.

#### Nocturne

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 safe_r·manual_q·manual_e·manual_r 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### Elise

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 stance·spiderlings·rappel_state·state_spider_e_stage·manual_e·flash_after_e·force_e·pause_r 계약을 연결했습니다. 공식 형태 11개와 전투 Q→W→E→R 순서를 유지합니다.

#### Brand

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 baseline 계약을 연결했습니다. 공식 형태 4개와 전투 W→Q→E→R 순서를 유지합니다.

#### LeeSin

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_insec·state_insec_anchor·state_r_line·wall_w·flash_after_w·flash_after_e·execute_r·flash_after_r 계약을 연결했습니다. 공식 형태 7개와 전투 Q→W→E→R 순서를 유지합니다.

#### Rumble

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_heat·state_danger_zone·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Cassiopeia

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 poison_e·miasma_dash·facing_r·manual_r·flash_after_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Nasus

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_q_stack·manual_w·manual_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Poppy

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 magnet_passive·state_wall_stun·force_e·flash_after_q·manual_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Pantheon

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 block_e·magnet_e·mode_q·mode_e·flash_after_q·force_w 계약을 연결했습니다. 공식 형태 7개와 전투 Q→W→E→R 순서를 유지합니다.

#### Ezreal

- NG-AIO의 초반 패시브 유지 결정을 현재 API로 옮겨, 실시간 `ezrealpassivestacks` 종료와 Q 비행시간이 만나는 66ms 구간에만 미니언 Q를 사용하도록 추가했습니다. 옵션은 기본 OFF입니다.

#### Mordekaiser

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_ring·isolated_q·realm_r·flash_after_q·force_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Kennen

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_mark·state_fast_farm·mode_farm·auto_q·auto_w 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Leona

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_e·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 W→E→Q→R 순서를 유지합니다.

#### Lux

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 mode_shield·manual_q·manual_r·flash_after_q 계약을 연결했습니다. 공식 형태 5개와 전투 E→Q→W→R 순서를 유지합니다.

#### Shyvana

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_dragon·manual_e·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 6개와 전투 Q→W→E→R 순서를 유지합니다.

#### Graves

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_q_wall·state_burst_combo·manual_w·manual_r·manual_er·flash_after_er 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### Varus

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_charge·blight·w_execute·chain_r·mode_q·mode_combat·state_blight·state_q_charge·manual_q·manual_r·flash_after_r·force_w 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Nautilus

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_q·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Viktor

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 e_vector·w_cc·r_follow·hex_fragments·state_e_vector·state_hex_fragments·manual_q·manual_w·manual_e·manual_r 계약을 연결했습니다. 공식 형태 5개와 전투 E→Q→W→R 순서를 유지합니다.

#### Fiora

- HGVip 교차 감사로 생성 전용 진입점에 승격하고 block_w·state_vitals·state_four_vitals·state_passive_follow·manual_w 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Ziggs

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_w_push·state_w_pull·manual_r·manual_w 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Lulu

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 mode_support·manual_we·manual_w·ally_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→W→Q→R 순서를 유지합니다.

#### Draven

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 axe_catch·axe_renewal·global_r·magnet_q·pause_magnet·state_q_renewal·safe_turret·manual_e·manual_r·flash_after_e 계약을 연결했습니다. 공식 형태 7개와 전투 Q→W→E→R 순서를 유지합니다.

#### Khazix

- HGVip+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 evolution·isolation·safe_e·state_evolution·state_isolation·force_e·pause_e 계약을 연결했습니다. 공식 형태 10개와 전투 Q→W→E→R 순서를 유지합니다.

#### Darius

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 magnet_q·manual_e·flash_after_q·pause_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### Jayce

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_stance·manual_q·manual_eq·cursor_eq·flash_after_e·force_e·pause_r 계약을 연결했습니다. 공식 형태 8개와 전투 Q→W→E→R 순서를 유지합니다.

#### Lissandra

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 auto_w·manual_r·flash_after_q 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Diana

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_qe·flash_after_r·force_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Kayn

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 safe_q·state_form·force_r 계약을 연결했습니다. 공식 형태 6개와 전투 Q→W→E→R 순서를 유지합니다.

#### Zoe

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_sleep·state_spell_shards 계약을 연결했습니다. 공식 형태 16개와 전투 Q→E→W→R 순서를 유지합니다.

#### Kaisa

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 evolution·plasma·isolated_q·safe_r·state_evolution·state_taunt·manual_w·force_e 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Seraphine

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 pause_passive·mode_double_cast·state_echo·manual_e·manual_r·flash_after_e·flash_after_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Zac

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_e_charge·state_passive·manual_e·cursor_e·auto_e 계약을 연결했습니다. 공식 형태 5개와 전투 E→W→Q→R 순서를 유지합니다.

#### Yasuo

- NG-AIO+HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_stack·dash_marks·minion_dash·eq·eq_flash·windwall·knockup_r·mode_e·state_q_stack·state_dash_marks·cursor_e·auto_r·flash_after_q·flash_after_eq 계약을 연결했습니다. 공식 형태 13개와 전투 Q→E→W→R 순서를 유지합니다.

#### Velkoz

- HGVip 교차 감사로 생성 전용 진입점에 승격하고 state_research·manual_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Taliyah

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 worked_ground·w_vector·e_dash·channel_r·magnet_q·state_w_push·state_w_pull·state_w_self_pull·manual_w·manual_r 계약을 연결했습니다. 공식 형태 9개와 전투 Q→E→W→R 순서를 유지합니다.

#### Braum

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_q·manual_r·flash_after_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Kindred

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_marks 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Zeri

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_attack·charged_passive·wall_w·wall_e·r_effectiveness·state_q_attack·state_r_effectiveness·manual_w·auto_q·force_qq 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### TahmKench

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 farm_q·state_acquired_taste·manual_q·manual_w·ally_r·force_r·auto_q 계약을 연결했습니다. 공식 형태 6개와 전투 Q→W→E→R 순서를 유지합니다.

#### Senna

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_soul_pickup·state_ward_q·manual_q·manual_w·manual_r·ally_q 계약을 연결했습니다. 공식 형태 5개와 전투 Q→W→E→R 순서를 유지합니다.

#### Lucian

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 passive_weave·extended_q·r_magnet·magnet_r·farm_extended_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Zed

- NG-AIO+CXJ 교차 감사로 생성 전용 진입점에 승격하고 shadow_tracking·multi_origin_q·shadow_e·weq·death_mark·safe_swap·mode_combo·state_safe_flash_combo·state_shadows·manual_weq·force_r 계약을 연결했습니다. 공식 형태 8개와 전투 R→W→E→Q 순서를 유지합니다.

#### Vi

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_q_charge·manual_q·force_r·flash_after_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Aatrox

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_q_stage·manual_w·flash_after_q 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Nami

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 state_auto_heal·state_heal_only·manual_q·manual_r 계약을 연결했습니다. 공식 형태 4개와 전투 W→E→Q→R 순서를 유지합니다.

#### Yuumi

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 auto_full·state_attach 계약을 연결했습니다. 공식 형태 13개와 전투 Q→E→W→R 순서를 유지합니다.

#### Samira

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 style·melee_q·projectile_w·dash_reset·r_gate·safe_e·state_style·manual_q·manual_e·flash_after_q 계약을 연결했습니다. 공식 형태 7개와 전투 Q→E→W→R 순서를 유지합니다.

#### Thresh

- HGVip+CXJ 교차 감사로 생성 전용 진입점에 승격하고 q_recast·lantern_ally·e_direction·state_e_push·state_e_pull·manual_q·ally_w 계약을 연결했습니다. 공식 형태 8개와 전투 Q→E→W→R 순서를 유지합니다.

#### Illaoi

- NG-AIO 교차 감사로 생성 전용 진입점에 승격하고 spirit_priority·w_attack_reset·heartsteel_wait·multi_r·state_soul_spells·state_soul_attacks·manual_e·flash_after_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→W→R 순서를 유지합니다.

#### Bard

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 manual_r·flash_after_q·force_w 계약을 연결했습니다. 공식 형태 14개와 전투 Q→W→E→R 순서를 유지합니다.

#### Xayah

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 feathers·e_root·r_reposition·magnet_r·state_feathers·manual_r 계약을 연결했습니다. 공식 형태 4개와 전투 E→W→Q→R 순서를 유지합니다.

#### Sylas

- HGVip 교차 감사로 생성 전용 진입점에 승격하고 state_e2_offset·state_double_w_guard·state_e_feint·safe_turret·manual_r·flash_after_r 계약을 연결했습니다. 공식 형태 6개와 전투 W→E→Q→R 순서를 유지합니다.

#### Neeko

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_disguise·manual_e·flash_after_e·flash_after_r 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

#### Aphelios

- HGVip+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 weapon_state·mark_range·weapon_swap·state_weapon_control·manual_q·manual_r·force_r·pause_w 계약을 연결했습니다. 공식 형태 11개와 전투 Q→E→W→R 순서를 유지합니다.

#### Rell

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 state_mount·manual_w·manual_wr·flash_after_q·flash_after_w·flash_after_r 계약을 연결했습니다. 공식 형태 5개와 전투 W→E→Q→R 순서를 유지합니다.

#### Yone

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 q_stack·spirit_return·safe_r·state_q3_stack·state_e2_offset·state_r_cc_offset·manual_r·auto_q·flash_after_q·pause_e 계약을 연결했습니다. 공식 형태 6개와 전투 Q→E→W→R 순서를 유지합니다.

#### Ambessa

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 block_w·mode_combat·safe_turret·manual_r·flash_after_q 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Mel

- NG-AIO+CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 multi_q·reserve_w·reflect_lethal·e_setup·r_reserve·block_w·state_r_reserve·manual_q·manual_e·auto_q·flash_after_e 계약을 연결했습니다. 공식 형태 4개와 전투 E→Q→R→W 순서를 유지합니다.

#### Lillia

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 magnet_q·state_outer_ring·state_drag·safe_w·flash_after_q 계약을 연결했습니다. 공식 형태 7개와 전투 Q→W→E→R 순서를 유지합니다.

#### Gwen

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 manual_r 계약을 연결했습니다. 공식 형태 10개와 전투 Q→E→W→R 순서를 유지합니다.

#### Renata

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 mode_q_recast·manual_q·manual_r·manual_qr·force_w 계약을 연결했습니다. 공식 형태 5개와 전투 E→W→Q→R 순서를 유지합니다.

#### Nilah

- Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 mode_farm·flash_after_q·flash_after_e·flash_after_r·force_e·cursor_e 계약을 연결했습니다. 공식 형태 4개와 전투 Q→E→W→R 순서를 유지합니다.

#### Smolder

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 safe_e·state_stacks·manual_w·manual_r 계약을 연결했습니다. 공식 형태 4개와 전투 Q→W→E→R 순서를 유지합니다.

#### Milio

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 ally_shield·interrupt_q·cleanse_r·manual_q 계약을 연결했습니다. 공식 형태 5개와 전투 E→W→Q→R 순서를 유지합니다.

#### Zaahen

- CXJ+Q-Aio 교차 감사로 생성 전용 진입점에 승격하고 recast_state·resource·execute·mode_farm·state_r_aoe·state_taunt·manual_w·manual_r·flash_after_w·force_w·pause_e·pause_r 계약을 연결했습니다. 공식 형태 6개와 전투 Q→E→W→R 순서를 유지합니다.

#### Naafiri

- CXJ 교차 감사로 생성 전용 진입점에 승격하고 safe_w·auto_q·flash_after_q·force_r·force_w·pause_e 계약을 연결했습니다. 공식 형태 5개와 전투 Q→E→W→R 순서를 유지합니다.

### English

#### Supported Champions

- Annie
- Olaf
- Twisted Fate
- Xin Zhao
- LeBlanc
- Vladimir
- Kayle
- Alistar
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Miss Fortune
- Ashe
- Jax
- Morgana
- Twitch
- Karthus
- Cho'Gath
- Amumu
- Dr. Mundo
- Kassadin
- Irelia
- Gangplank
- Corki
- Trundle
- Swain
- Caitlyn
- Blitzcrank
- Malphite
- Katarina
- Nocturne
- Elise
- Orianna
- Brand
- Lee Sin
- Vayne
- Rumble
- Cassiopeia
- Nasus
- Poppy
- Pantheon
- Ezreal
- Mordekaiser
- Akali
- Kennen
- Garen
- Leona
- Malzahar
- Talon
- Riven
- Kog'Maw
- Lux
- Xerath
- Shyvana
- Ahri
- Graves
- Rengar
- Varus
- Nautilus
- Viktor
- Fiora
- Ziggs
- Lulu
- Draven
- Kha'Zix
- Darius
- Jayce
- Lissandra
- Diana
- Syndra
- Kayn
- Zoe
- Kai'Sa
- Seraphine
- Zac
- Yasuo
- Vel'Koz
- Taliyah
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- Tahm Kench
- Senna
- Lucian
- Zed
- Qiyana
- Vi
- Aatrox
- Nami
- Yuumi
- Samira
- Thresh
- Illaoi
- Kalista
- Bard
- Xayah
- Sylas
- Neeko
- Aphelios
- Rell
- Pyke
- Yone
- Ambessa
- Mel
- Yunara
- Locke
- Lillia
- Gwen
- Renata Glasc
- Aurora
- Nilah
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- v2.25.0 runs all 173 modern champions from Riot 16.15.1/client 16.15 as 28 hand-tuned, 92 generated-specialist, and 53 shared entries, plus the 60-champion League Classic (JADE) launch roster through separate old-kit profiles.
- Audited every user-authorized NG-AIO, HGVip, CXJ, Q-Aio, and FXT source and promoted every modern champion covered by those archives. Restored archives are not loaded directly; their useful logic is adapted to the current Hanbot API and Riot-backed generated profiles and state gates.
- The new Source Guard prevents guessed automatic casts of recasts, survival tools, and ultimates classified as manual or defensive when their live form cannot be confirmed.
- JADE maps each runtime champion name to its modern base alias while applying 59 old-kit geometry sets imported from FXT. Rammus, whose FXT module is absent, uses a safe modern-profile fallback until live names are verified.
- Re-audited all 28 hand-tuned modules instead of preserving them blindly. Tristana now immediately focuses the active E-bomb target; legacy A-Q-A and offensive-W patterns that conflict with current max-DPS or safety doctrine were rejected.
- Specialist menus expose audit sources, feature contracts, and connected champion options while retaining Semi Q/W/E/R, Champion Actions, and LMB key assignment.
- Matches each live slot name against 1,004 official raw forms (recast 269, transform/upgrade 23, charge 23, attack reset 75) every tick, preferring an exact mScriptName when aliases overlap.
- Covers both directions of Elise, Jayce, and Nidalee transformations, Rek'Sai burrow, Aphelios weapon swaps, Hwei palettes, Sylas stolen ultimates, and Viego possession slots through the full official catalog.
- Forms with an ambiguous official targeting contract stay semi-manual only, while automatic ultimates and transformations remain disabled by default.
- Official attack-reset forms preserve the auto-attack windup, cast on the first valid backswing callback, and retry only valid rejected requests with a 1 ms script-local floor.
- Archived skill priorities and user-tip summaries for all 173 champions from OP.GG 16.15 after verifying robots.txt permission; Riot data remains the sole authority for numbers and cast forms.

#### Annie

- Promoted to a dedicated specialist entry after CXJ review, with mode_farm, manual_q, manual_r, flash_after_w, flash_before_r, force_r; it retains 4 official forms and the Q→W→E→R combat order.

#### Olaf

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with axe_pickup, q_magnet, low_hp_w, mode_q, magnet_q, state_axe; it retains 5 official forms and the Q→E→W→R combat order.

#### TwistedFate

- Promoted to a dedicated specialist entry after Q-Aio review, with state_card_gold, state_card_blue, state_card_red, state_attack_reset, state_card_attack_pause, state_card_attack_weave, manual_q, manual_w; it retains 8 official forms and the Q→W→E→R combat order.

#### XinZhao

- Promoted to a dedicated specialist entry after Q-Aio review, with state_w_adjust, manual_w, flash_after_w, force_w, force_e; it retains 4 official forms and the W→E→Q→R combat order.

#### Vladimir

- Promoted to a dedicated specialist entry after NG-AIO+Q-Aio review, with empowered_q, e_charge, e_release, pool_block, multi_r, state_empowered_q, state_e_charge, manual_r, flash_after_e; it retains 4 official forms and the Q→E→R→W combat order.

#### Kayle

- Promoted to a dedicated specialist entry after Q-Aio review, with state_auto_heal, ally_r; it retains 7 official forms and the E→Q→W→R combat order.

#### Alistar

- Promoted to a dedicated specialist entry after CXJ review, with manual_w, manual_wq, flash_after_q, flash_after_wq, flash_before_qw; it retains 4 official forms and the Q→W→E→R combat order.

#### Sion

- Promoted to a dedicated specialist entry after CXJ review, with state_q_charge, state_r_steer, flash_after_w, flash_after_e; it retains 5 official forms and the Q→W→E→R combat order.

#### Sivir

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_return, w_reset, spellshield, magnet_q, manual_q, auto_q, flash_after_q; it retains 4 official forms and the Q→W→E→R combat order.

#### Tristana

- Ported E-bomb target focus found in the HGVip/CXJ/Q-Aio comparison to the current orbwalker API. The active bomb target is selected for that tick only while in attack range, so stale targets cannot lock movement.

#### MissFortune

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with passive_swap, q_bounce, channel_r, state_passive_logic, manual_w, manual_r, pause_e; it retains 5 official forms and the Q→W→E→R combat order.

#### Ashe

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_weave, cone_w, global_r, cursor_e, manual_r; it retains 6 official forms and the W→Q→E→R combat order.

#### Jax

- Promoted to a dedicated specialist entry after Q-Aio review, with block_e, safe_q, force_q; it retains 4 official forms and the W→E→Q→R combat order.

#### Morgana

- Promoted to a dedicated specialist entry after CXJ review, with manual_q; it retains 4 official forms and the Q→W→E→R combat order.

#### Twitch

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with poison, stealth_return, e_execute, r_line, state_stealth_return, state_poison, manual_w, pause_e; it retains 4 official forms and the E→Q→W→R combat order.

#### Karthus

- Promoted to a dedicated specialist entry after NG-AIO+CXJ+Q-Aio review, with isolated_q, aura_hysteresis, mana_reserve, passive_r, global_r, mode_first_strike, manual_w; it retains 15 official forms and the E→Q→W→R combat order.

#### Chogath

- Promoted to a dedicated specialist entry after CXJ review, with farm_e, manual_q, flash_after_w; it retains 6 official forms and the E→Q→W→R combat order.

#### Amumu

- Promoted to a dedicated specialist entry after CXJ review, with farm_no_q, manual_q, flash_after_q; it retains 4 official forms and the E→Q→W→R combat order.

#### DrMundo

- Promoted to a dedicated specialist entry after CXJ review, with manual_q, auto_q; it retains 6 official forms and the Q→E→W→R combat order.

#### Kassadin

- Promoted to a dedicated specialist entry after CXJ review, with safe_mobility, farm_q, manual_q, auto_q, flash_after_e; it retains 4 official forms and the E→W→Q→R combat order.

#### Irelia

- Promoted to a dedicated specialist entry after NG-AIO+CXJ review, with q_reset, marked_q, minion_gapclose, e_two_stage, w_block, multi_r, safe_farm_turret, state_q_reset, manual_r, flash_after_r, force_q; it retains 8 official forms and the E→R→Q→W combat order.

#### Corki

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with missile_ammo, big_one, package_state, manual_q, manual_r, auto_r; it retains 4 official forms and the Q→E→W→R combat order.

#### Trundle

- Promoted to a dedicated specialist entry after CXJ review, with state_e_push, state_e_pull, manual_e, manual_r; it retains 5 official forms and the Q→W→E→R combat order.

#### Swain

- Promoted to a dedicated specialist entry after CXJ review, with magnet_e, state_soul_fragment, manual_w, manual_e, flash_after_q; it retains 6 official forms and the Q→W→E→R combat order.

#### Caitlyn

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with headshot, trap_cc, net_recoil, global_execute, state_reverse_e, manual_q, manual_w, manual_e, flash_after_e; it retains 5 official forms and the Q→W→E→R combat order.

#### Blitzcrank

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with hook_collision, e_reset, interrupt_r, manual_q; it retains 4 official forms and the Q→E→W→R combat order.

#### Katarina

- Promoted to a dedicated specialist entry after CXJ review, with safe_farm_turret, state_daggers, auto_q, pause_e; it retains 8 official forms and the Q→E→W→R combat order.

#### Nocturne

- Promoted to a dedicated specialist entry after CXJ review, with safe_r, manual_q, manual_e, manual_r; it retains 5 official forms and the Q→E→W→R combat order.

#### Elise

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with stance, spiderlings, rappel_state, state_spider_e_stage, manual_e, flash_after_e, force_e, pause_r; it retains 11 official forms and the Q→W→E→R combat order.

#### Brand

- Promoted to a dedicated specialist entry after CXJ review, with baseline; it retains 4 official forms and the W→Q→E→R combat order.

#### LeeSin

- Promoted to a dedicated specialist entry after CXJ review, with state_insec, state_insec_anchor, state_r_line, wall_w, flash_after_w, flash_after_e, execute_r, flash_after_r; it retains 7 official forms and the Q→W→E→R combat order.

#### Rumble

- Promoted to a dedicated specialist entry after CXJ review, with state_heat, state_danger_zone, manual_r, flash_after_e; it retains 4 official forms and the Q→E→W→R combat order.

#### Cassiopeia

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with poison_e, miasma_dash, facing_r, manual_r, flash_after_r; it retains 4 official forms and the E→Q→W→R combat order.

#### Nasus

- Promoted to a dedicated specialist entry after CXJ review, with state_q_stack, manual_w, manual_e; it retains 4 official forms and the Q→W→E→R combat order.

#### Poppy

- Promoted to a dedicated specialist entry after CXJ review, with magnet_passive, state_wall_stun, force_e, flash_after_q, manual_r; it retains 4 official forms and the Q→E→W→R combat order.

#### Pantheon

- Promoted to a dedicated specialist entry after Q-Aio review, with block_e, magnet_e, mode_q, mode_e, flash_after_q, force_w; it retains 7 official forms and the Q→W→E→R combat order.

#### Ezreal

- Ported NG-AIO's early passive refresh decision to the current API: minion Q is requested only in the 66 ms window where travel time lands before `ezrealpassivestacks` expires. The option defaults off.

#### Mordekaiser

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with passive_ring, isolated_q, realm_r, flash_after_q, force_r; it retains 4 official forms and the Q→E→W→R combat order.

#### Kennen

- Promoted to a dedicated specialist entry after Q-Aio review, with state_mark, state_fast_farm, mode_farm, auto_q, auto_w; it retains 5 official forms and the Q→W→E→R combat order.

#### Leona

- Promoted to a dedicated specialist entry after CXJ review, with manual_e, manual_r, flash_after_e; it retains 4 official forms and the W→E→Q→R combat order.

#### Lux

- Promoted to a dedicated specialist entry after CXJ review, with mode_shield, manual_q, manual_r, flash_after_q; it retains 5 official forms and the E→Q→W→R combat order.

#### Shyvana

- Promoted to a dedicated specialist entry after CXJ review, with state_dragon, manual_e, manual_r, flash_after_e; it retains 6 official forms and the Q→W→E→R combat order.

#### Graves

- Promoted to a dedicated specialist entry after CXJ review, with state_q_wall, state_burst_combo, manual_w, manual_r, manual_er, flash_after_er; it retains 5 official forms and the Q→E→W→R combat order.

#### Varus

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_charge, blight, w_execute, chain_r, mode_q, mode_combat, state_blight, state_q_charge, manual_q, manual_r, flash_after_r, force_w; it retains 4 official forms and the Q→W→E→R combat order.

#### Nautilus

- Promoted to a dedicated specialist entry after CXJ review, with manual_q, manual_r, flash_after_e; it retains 4 official forms and the Q→W→E→R combat order.

#### Viktor

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with e_vector, w_cc, r_follow, hex_fragments, state_e_vector, state_hex_fragments, manual_q, manual_w, manual_e, manual_r; it retains 5 official forms and the E→Q→W→R combat order.

#### Fiora

- Promoted to a dedicated specialist entry after HGVip review, with block_w, state_vitals, state_four_vitals, state_passive_follow, manual_w; it retains 4 official forms and the Q→E→W→R combat order.

#### Ziggs

- Promoted to a dedicated specialist entry after Q-Aio review, with state_w_push, state_w_pull, manual_r, manual_w; it retains 7 official forms and the Q→E→W→R combat order.

#### Lulu

- Promoted to a dedicated specialist entry after Q-Aio review, with mode_support, manual_we, manual_w, ally_r; it retains 4 official forms and the E→W→Q→R combat order.

#### Draven

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with axe_catch, axe_renewal, global_r, magnet_q, pause_magnet, state_q_renewal, safe_turret, manual_e, manual_r, flash_after_e; it retains 7 official forms and the Q→W→E→R combat order.

#### Khazix

- Promoted to a dedicated specialist entry after HGVip+Q-Aio review, with evolution, isolation, safe_e, state_evolution, state_isolation, force_e, pause_e; it retains 10 official forms and the Q→W→E→R combat order.

#### Darius

- Promoted to a dedicated specialist entry after CXJ review, with magnet_q, manual_e, flash_after_q, pause_e; it retains 5 official forms and the Q→E→W→R combat order.

#### Jayce

- Promoted to a dedicated specialist entry after CXJ review, with state_stance, manual_q, manual_eq, cursor_eq, flash_after_e, force_e, pause_r; it retains 8 official forms and the Q→W→E→R combat order.

#### Lissandra

- Promoted to a dedicated specialist entry after CXJ review, with auto_w, manual_r, flash_after_q; it retains 5 official forms and the Q→W→E→R combat order.

#### Diana

- Promoted to a dedicated specialist entry after CXJ review, with manual_qe, flash_after_r, force_e; it retains 4 official forms and the Q→W→E→R combat order.

#### Kayn

- Promoted to a dedicated specialist entry after Q-Aio review, with safe_q, state_form, force_r; it retains 6 official forms and the Q→W→E→R combat order.

#### Zoe

- Promoted to a dedicated specialist entry after CXJ review, with state_sleep, state_spell_shards; it retains 16 official forms and the Q→E→W→R combat order.

#### Kaisa

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with evolution, plasma, isolated_q, safe_r, state_evolution, state_taunt, manual_w, force_e; it retains 7 official forms and the Q→E→W→R combat order.

#### Seraphine

- Promoted to a dedicated specialist entry after CXJ review, with pause_passive, mode_double_cast, state_echo, manual_e, manual_r, flash_after_e, flash_after_r; it retains 4 official forms and the Q→W→E→R combat order.

#### Zac

- Promoted to a dedicated specialist entry after CXJ review, with state_e_charge, state_passive, manual_e, cursor_e, auto_e; it retains 5 official forms and the E→W→Q→R combat order.

#### Yasuo

- Promoted to a dedicated specialist entry after NG-AIO+HGVip+CXJ review, with q_stack, dash_marks, minion_dash, eq, eq_flash, windwall, knockup_r, mode_e, state_q_stack, state_dash_marks, cursor_e, auto_r, flash_after_q, flash_after_eq; it retains 13 official forms and the Q→E→W→R combat order.

#### Velkoz

- Promoted to a dedicated specialist entry after HGVip review, with state_research, manual_e; it retains 5 official forms and the Q→W→E→R combat order.

#### Taliyah

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with worked_ground, w_vector, e_dash, channel_r, magnet_q, state_w_push, state_w_pull, state_w_self_pull, manual_w, manual_r; it retains 9 official forms and the Q→E→W→R combat order.

#### Braum

- Promoted to a dedicated specialist entry after CXJ review, with manual_q, manual_r, flash_after_q; it retains 4 official forms and the Q→E→W→R combat order.

#### Kindred

- Promoted to a dedicated specialist entry after Q-Aio review, with state_marks; it retains 5 official forms and the Q→W→E→R combat order.

#### Zeri

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_attack, charged_passive, wall_w, wall_e, r_effectiveness, state_q_attack, state_r_effectiveness, manual_w, auto_q, force_qq; it retains 4 official forms and the Q→E→W→R combat order.

#### TahmKench

- Promoted to a dedicated specialist entry after CXJ review, with farm_q, state_acquired_taste, manual_q, manual_w, ally_r, force_r, auto_q; it retains 6 official forms and the Q→W→E→R combat order.

#### Senna

- Promoted to a dedicated specialist entry after CXJ review, with state_soul_pickup, state_ward_q, manual_q, manual_w, manual_r, ally_q; it retains 5 official forms and the Q→W→E→R combat order.

#### Lucian

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with passive_weave, extended_q, r_magnet, magnet_r, farm_extended_q; it retains 4 official forms and the Q→E→W→R combat order.

#### Zed

- Promoted to a dedicated specialist entry after NG-AIO+CXJ review, with shadow_tracking, multi_origin_q, shadow_e, weq, death_mark, safe_swap, mode_combo, state_safe_flash_combo, state_shadows, manual_weq, force_r; it retains 8 official forms and the R→W→E→Q combat order.

#### Vi

- Promoted to a dedicated specialist entry after Q-Aio review, with state_q_charge, manual_q, force_r, flash_after_q; it retains 4 official forms and the Q→E→W→R combat order.

#### Aatrox

- Promoted to a dedicated specialist entry after CXJ review, with state_q_stage, manual_w, flash_after_q; it retains 7 official forms and the Q→E→W→R combat order.

#### Nami

- Promoted to a dedicated specialist entry after Q-Aio review, with state_auto_heal, state_heal_only, manual_q, manual_r; it retains 4 official forms and the W→E→Q→R combat order.

#### Yuumi

- Promoted to a dedicated specialist entry after CXJ review, with auto_full, state_attach; it retains 13 official forms and the Q→E→W→R combat order.

#### Samira

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with style, melee_q, projectile_w, dash_reset, r_gate, safe_e, state_style, manual_q, manual_e, flash_after_q; it retains 7 official forms and the Q→E→W→R combat order.

#### Thresh

- Promoted to a dedicated specialist entry after HGVip+CXJ review, with q_recast, lantern_ally, e_direction, state_e_push, state_e_pull, manual_q, ally_w; it retains 8 official forms and the Q→E→W→R combat order.

#### Illaoi

- Promoted to a dedicated specialist entry after NG-AIO review, with spirit_priority, w_attack_reset, heartsteel_wait, multi_r, state_soul_spells, state_soul_attacks, manual_e, flash_after_r; it retains 4 official forms and the E→Q→W→R combat order.

#### Bard

- Promoted to a dedicated specialist entry after CXJ review, with manual_r, flash_after_q, force_w; it retains 14 official forms and the Q→W→E→R combat order.

#### Xayah

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with feathers, e_root, r_reposition, magnet_r, state_feathers, manual_r; it retains 4 official forms and the E→W→Q→R combat order.

#### Sylas

- Promoted to a dedicated specialist entry after HGVip review, with state_e2_offset, state_double_w_guard, state_e_feint, safe_turret, manual_r, flash_after_r; it retains 6 official forms and the W→E→Q→R combat order.

#### Neeko

- Promoted to a dedicated specialist entry after CXJ review, with state_disguise, manual_e, flash_after_e, flash_after_r; it retains 5 official forms and the Q→E→W→R combat order.

#### Aphelios

- Promoted to a dedicated specialist entry after HGVip+CXJ+Q-Aio review, with weapon_state, mark_range, weapon_swap, state_weapon_control, manual_q, manual_r, force_r, pause_w; it retains 11 official forms and the Q→E→W→R combat order.

#### Rell

- Promoted to a dedicated specialist entry after CXJ review, with state_mount, manual_w, manual_wr, flash_after_q, flash_after_w, flash_after_r; it retains 5 official forms and the W→E→Q→R combat order.

#### Yone

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with q_stack, spirit_return, safe_r, state_q3_stack, state_e2_offset, state_r_cc_offset, manual_r, auto_q, flash_after_q, pause_e; it retains 6 official forms and the Q→E→W→R combat order.

#### Ambessa

- Promoted to a dedicated specialist entry after CXJ review, with block_w, mode_combat, safe_turret, manual_r, flash_after_q; it retains 4 official forms and the Q→E→W→R combat order.

#### Mel

- Promoted to a dedicated specialist entry after NG-AIO+CXJ+Q-Aio review, with multi_q, reserve_w, reflect_lethal, e_setup, r_reserve, block_w, state_r_reserve, manual_q, manual_e, auto_q, flash_after_e; it retains 4 official forms and the E→Q→R→W combat order.

#### Lillia

- Promoted to a dedicated specialist entry after CXJ review, with magnet_q, state_outer_ring, state_drag, safe_w, flash_after_q; it retains 7 official forms and the Q→W→E→R combat order.

#### Gwen

- Promoted to a dedicated specialist entry after Q-Aio review, with manual_r; it retains 10 official forms and the Q→E→W→R combat order.

#### Renata

- Promoted to a dedicated specialist entry after CXJ review, with mode_q_recast, manual_q, manual_r, manual_qr, force_w; it retains 5 official forms and the E→W→Q→R combat order.

#### Nilah

- Promoted to a dedicated specialist entry after Q-Aio review, with mode_farm, flash_after_q, flash_after_e, flash_after_r, force_e, cursor_e; it retains 4 official forms and the Q→E→W→R combat order.

#### Smolder

- Promoted to a dedicated specialist entry after CXJ review, with safe_e, state_stacks, manual_w, manual_r; it retains 4 official forms and the Q→W→E→R combat order.

#### Milio

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with ally_shield, interrupt_q, cleanse_r, manual_q; it retains 5 official forms and the E→W→Q→R combat order.

#### Zaahen

- Promoted to a dedicated specialist entry after CXJ+Q-Aio review, with recast_state, resource, execute, mode_farm, state_r_aoe, state_taunt, manual_w, manual_r, flash_after_w, force_w, pause_e, pause_r; it retains 6 official forms and the Q→E→W→R combat order.

#### Naafiri

- Promoted to a dedicated specialist entry after CXJ review, with safe_w, auto_q, flash_after_q, force_r, force_w, pause_e; it retains 5 official forms and the Q→E→W→R combat order.

### 简体中文

#### 支持英雄

- 黑暗之女
- 狂战士
- 卡牌大师
- 德邦总管
- 诡术妖姬
- 猩红收割者
- 正义天使
- 牛头酋长
- 亡灵战神
- 战争女神
- 众星之子
- 迅捷斥候
- 麦林炮手
- 赏金猎人
- 寒冰射手
- 武器大师
- 堕落天使
- 瘟疫之源
- 死亡颂唱者
- 虚空恐惧
- 殇之木乃伊
- 祖安狂人
- 虚空行者
- 刀锋舞者
- 海洋之灾
- 英勇投弹手
- 巨魔之王
- 诺克萨斯统领
- 皮城女警
- 蒸汽机器人
- 熔岩巨兽
- 不祥之刃
- 永恒梦魇
- 蜘蛛女皇
- 发条魔灵
- 复仇焰魂
- 盲僧
- 暗夜猎手
- 机械公敌
- 魔蛇之拥
- 沙漠死神
- 圣锤之毅
- 不屈之枪
- 探险家
- 铁铠冥魂
- 离群之刺
- 狂暴之心
- 德玛西亚之力
- 曙光女神
- 虚空先知
- 刀锋之影
- 放逐之刃
- 深渊巨口
- 光辉女郎
- 远古巫灵
- 龙血武姬
- 九尾妖狐
- 法外狂徒
- 傲之追猎者
- 惩戒之箭
- 深海泰坦
- 奥术先驱
- 无双剑姬
- 爆破鬼才
- 仙灵女巫
- 荣耀行刑官
- 虚空掠夺者
- 诺克萨斯之手
- 未来守护者
- 冰霜女巫
- 皎月女神
- 暗黑元首
- 影流之镰
- 暮光星灵
- 虚空之女
- 星籁歌姬
- 生化魔人
- 疾风剑豪
- 虚空之眼
- 岩雀
- 弗雷尔卓德之心
- 戏命师
- 永猎双子
- 祖安花火
- 暴走萝莉
- 河流之王
- 涤魂圣枪
- 圣枪游侠
- 影流之主
- 元素女皇
- 皮城执法官
- 暗裔剑魔
- 唤潮鲛姬
- 魔法猫咪
- 沙漠玫瑰
- 魂锁典狱长
- 海兽祭司
- 复仇之矛
- 星界游神
- 逆羽
- 解脱者
- 万花通灵
- 残月之肃
- 镕铁少女
- 血港鬼影
- 封魔剑魂
- 铁血狼母
- 流光镜影
- 不破之誓
- 灰烬驱魔人
- 含羞蓓蕾
- 灵罗娃娃
- 炼金男爵
- 双界灵兔
- 不羁之悦
- 炽炎雏龙
- 明烛
- 不落魔锋
- 异画师
- 百裂冥犬

#### 核心与菜单

- v2.25.0 依据 Riot 16.15.1/客户端 16.15 支持全部 173 位现代英雄：28 个手工专属、92 个生成专属、53 个共用入口，并通过独立旧版技能配置支持 League Classic（JADE）首发 60 位英雄。
- 全面审计用户授权使用的 NG-AIO、HGVip、CXJ、Q-Aio 与 FXT，并将这些资料覆盖的现代英雄全部升级为专属类别；不直接加载旧源码，而是按当前 Hanbot API 与 Riot 原始资料迁移有效逻辑。
- 新增 Source Guard：实时形态无法确认时，不会猜测自动施放被资料标记为手动或防御用途的再施法、生存技能与终极技能。
- JADE 将运行时英雄名映射到现代基础别名，同时应用 FXT 的 59 套旧版技能形状；FXT 缺少 Rammus 模块，因此在实测名称前使用安全的现代配置回退。
- 重新审计全部 28 个手工模块，而不是盲目保留。Tristana 现在会立即优先普攻已附着 E 炸弹的目标；与当前最高输出或安全策略冲突的旧 A-Q-A、进攻 W 方案未采用。
- 专属菜单显示审计来源、功能契约和已连接的英雄选项，同时保留 Semi Q/W/E/R、Champion Actions 与 LMB 按键分配。
- 每个 tick 将当前技能槽名称与 1,004 个官方 raw 形态（再施法 269、变身/强化 23、蓄力 23、普攻重置 75）匹配；别名重叠时优先精确 mScriptName。
- 通过完整官方目录覆盖伊莉丝、杰斯、奈德丽双向变身、雷克塞遁地、厄斐琉斯换枪、慧的画板、塞拉斯偷取终极技能和佛耶戈附身后的技能槽。
- 官方目标类型不明确的形态只允许半自动按键，自动使用终极技能和自动变身默认关闭。
- 带官方普攻重置标签的形态会保留普攻前摇，在第一个有效后摇回调施法，并仅对有效但被拒绝的请求按 1 毫秒脚本下限重试。
- 在确认 robots.txt 允许后，离线保存 OP.GG 16.15 的 173 位英雄技能优先级和用户技巧摘要；技能数值与施法形态仍只以 Riot 原始数据为准。

#### Annie

- 经 CXJ 交叉审计后升级为专属入口，加入 mode_farm、manual_q、manual_r、flash_after_w、flash_before_r、force_r，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Olaf

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 axe_pickup、q_magnet、low_hp_w、mode_q、magnet_q、state_axe，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### TwistedFate

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_card_gold、state_card_blue、state_card_red、state_attack_reset、state_card_attack_pause、state_card_attack_weave、manual_q、manual_w，并保留 8 个官方形态与 Q→W→E→R 战斗顺序。

#### XinZhao

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_w_adjust、manual_w、flash_after_w、force_w、force_e，并保留 4 个官方形态与 W→E→Q→R 战斗顺序。

#### Vladimir

- 经 NG-AIO+Q-Aio 交叉审计后升级为专属入口，加入 empowered_q、e_charge、e_release、pool_block、multi_r、state_empowered_q、state_e_charge、manual_r、flash_after_e，并保留 4 个官方形态与 Q→E→R→W 战斗顺序。

#### Kayle

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_auto_heal、ally_r，并保留 7 个官方形态与 E→Q→W→R 战斗顺序。

#### Alistar

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_w、manual_wq、flash_after_q、flash_after_wq、flash_before_qw，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Sion

- 经 CXJ 交叉审计后升级为专属入口，加入 state_q_charge、state_r_steer、flash_after_w、flash_after_e，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Sivir

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_return、w_reset、spellshield、magnet_q、manual_q、auto_q、flash_after_q，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Tristana

- 将 HGVip/CXJ/Q-Aio 对比中确认的 E 炸弹目标优先逻辑迁移到当前走砍 API；仅在目标处于普攻范围内时当 tick 重定向，目标失效或离开范围后不会残留锁定。

#### MissFortune

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_swap、q_bounce、channel_r、state_passive_logic、manual_w、manual_r、pause_e，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Ashe

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_weave、cone_w、global_r、cursor_e、manual_r，并保留 6 个官方形态与 W→Q→E→R 战斗顺序。

#### Jax

- 经 Q-Aio 交叉审计后升级为专属入口，加入 block_e、safe_q、force_q，并保留 4 个官方形态与 W→E→Q→R 战斗顺序。

#### Morgana

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_q，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Twitch

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 poison、stealth_return、e_execute、r_line、state_stealth_return、state_poison、manual_w、pause_e，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Karthus

- 经 NG-AIO+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 isolated_q、aura_hysteresis、mana_reserve、passive_r、global_r、mode_first_strike、manual_w，并保留 15 个官方形态与 E→Q→W→R 战斗顺序。

#### Chogath

- 经 CXJ 交叉审计后升级为专属入口，加入 farm_e、manual_q、flash_after_w，并保留 6 个官方形态与 E→Q→W→R 战斗顺序。

#### Amumu

- 经 CXJ 交叉审计后升级为专属入口，加入 farm_no_q、manual_q、flash_after_q，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### DrMundo

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_q、auto_q，并保留 6 个官方形态与 Q→E→W→R 战斗顺序。

#### Kassadin

- 经 CXJ 交叉审计后升级为专属入口，加入 safe_mobility、farm_q、manual_q、auto_q、flash_after_e，并保留 4 个官方形态与 E→W→Q→R 战斗顺序。

#### Irelia

- 经 NG-AIO+CXJ 交叉审计后升级为专属入口，加入 q_reset、marked_q、minion_gapclose、e_two_stage、w_block、multi_r、safe_farm_turret、state_q_reset、manual_r、flash_after_r、force_q，并保留 8 个官方形态与 E→R→Q→W 战斗顺序。

#### Corki

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 missile_ammo、big_one、package_state、manual_q、manual_r、auto_r，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Trundle

- 经 CXJ 交叉审计后升级为专属入口，加入 state_e_push、state_e_pull、manual_e、manual_r，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Swain

- 经 CXJ 交叉审计后升级为专属入口，加入 magnet_e、state_soul_fragment、manual_w、manual_e、flash_after_q，并保留 6 个官方形态与 Q→W→E→R 战斗顺序。

#### Caitlyn

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 headshot、trap_cc、net_recoil、global_execute、state_reverse_e、manual_q、manual_w、manual_e、flash_after_e，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Blitzcrank

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 hook_collision、e_reset、interrupt_r、manual_q，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Katarina

- 经 CXJ 交叉审计后升级为专属入口，加入 safe_farm_turret、state_daggers、auto_q、pause_e，并保留 8 个官方形态与 Q→E→W→R 战斗顺序。

#### Nocturne

- 经 CXJ 交叉审计后升级为专属入口，加入 safe_r、manual_q、manual_e、manual_r，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### Elise

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 stance、spiderlings、rappel_state、state_spider_e_stage、manual_e、flash_after_e、force_e、pause_r，并保留 11 个官方形态与 Q→W→E→R 战斗顺序。

#### Brand

- 经 CXJ 交叉审计后升级为专属入口，加入 baseline，并保留 4 个官方形态与 W→Q→E→R 战斗顺序。

#### LeeSin

- 经 CXJ 交叉审计后升级为专属入口，加入 state_insec、state_insec_anchor、state_r_line、wall_w、flash_after_w、flash_after_e、execute_r、flash_after_r，并保留 7 个官方形态与 Q→W→E→R 战斗顺序。

#### Rumble

- 经 CXJ 交叉审计后升级为专属入口，加入 state_heat、state_danger_zone、manual_r、flash_after_e，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Cassiopeia

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 poison_e、miasma_dash、facing_r、manual_r、flash_after_r，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Nasus

- 经 CXJ 交叉审计后升级为专属入口，加入 state_q_stack、manual_w、manual_e，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Poppy

- 经 CXJ 交叉审计后升级为专属入口，加入 magnet_passive、state_wall_stun、force_e、flash_after_q、manual_r，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Pantheon

- 经 Q-Aio 交叉审计后升级为专属入口，加入 block_e、magnet_e、mode_q、mode_e、flash_after_q、force_w，并保留 7 个官方形态与 Q→W→E→R 战斗顺序。

#### Ezreal

- 将 NG-AIO 的前期被动续层判断迁移到当前 API：只有当 Q 飞行时间能在 `ezrealpassivestacks` 结束前命中的 66 毫秒窗口内，才会对小兵施放 Q；该选项默认关闭。

#### Mordekaiser

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_ring、isolated_q、realm_r、flash_after_q、force_r，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Kennen

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_mark、state_fast_farm、mode_farm、auto_q、auto_w，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Leona

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_e、manual_r、flash_after_e，并保留 4 个官方形态与 W→E→Q→R 战斗顺序。

#### Lux

- 经 CXJ 交叉审计后升级为专属入口，加入 mode_shield、manual_q、manual_r、flash_after_q，并保留 5 个官方形态与 E→Q→W→R 战斗顺序。

#### Shyvana

- 经 CXJ 交叉审计后升级为专属入口，加入 state_dragon、manual_e、manual_r、flash_after_e，并保留 6 个官方形态与 Q→W→E→R 战斗顺序。

#### Graves

- 经 CXJ 交叉审计后升级为专属入口，加入 state_q_wall、state_burst_combo、manual_w、manual_r、manual_er、flash_after_er，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### Varus

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_charge、blight、w_execute、chain_r、mode_q、mode_combat、state_blight、state_q_charge、manual_q、manual_r、flash_after_r、force_w，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Nautilus

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_q、manual_r、flash_after_e，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Viktor

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 e_vector、w_cc、r_follow、hex_fragments、state_e_vector、state_hex_fragments、manual_q、manual_w、manual_e、manual_r，并保留 5 个官方形态与 E→Q→W→R 战斗顺序。

#### Fiora

- 经 HGVip 交叉审计后升级为专属入口，加入 block_w、state_vitals、state_four_vitals、state_passive_follow、manual_w，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Ziggs

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_w_push、state_w_pull、manual_r、manual_w，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Lulu

- 经 Q-Aio 交叉审计后升级为专属入口，加入 mode_support、manual_we、manual_w、ally_r，并保留 4 个官方形态与 E→W→Q→R 战斗顺序。

#### Draven

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 axe_catch、axe_renewal、global_r、magnet_q、pause_magnet、state_q_renewal、safe_turret、manual_e、manual_r、flash_after_e，并保留 7 个官方形态与 Q→W→E→R 战斗顺序。

#### Khazix

- 经 HGVip+Q-Aio 交叉审计后升级为专属入口，加入 evolution、isolation、safe_e、state_evolution、state_isolation、force_e、pause_e，并保留 10 个官方形态与 Q→W→E→R 战斗顺序。

#### Darius

- 经 CXJ 交叉审计后升级为专属入口，加入 magnet_q、manual_e、flash_after_q、pause_e，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### Jayce

- 经 CXJ 交叉审计后升级为专属入口，加入 state_stance、manual_q、manual_eq、cursor_eq、flash_after_e、force_e、pause_r，并保留 8 个官方形态与 Q→W→E→R 战斗顺序。

#### Lissandra

- 经 CXJ 交叉审计后升级为专属入口，加入 auto_w、manual_r、flash_after_q，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Diana

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_qe、flash_after_r、force_e，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Kayn

- 经 Q-Aio 交叉审计后升级为专属入口，加入 safe_q、state_form、force_r，并保留 6 个官方形态与 Q→W→E→R 战斗顺序。

#### Zoe

- 经 CXJ 交叉审计后升级为专属入口，加入 state_sleep、state_spell_shards，并保留 16 个官方形态与 Q→E→W→R 战斗顺序。

#### Kaisa

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 evolution、plasma、isolated_q、safe_r、state_evolution、state_taunt、manual_w、force_e，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Seraphine

- 经 CXJ 交叉审计后升级为专属入口，加入 pause_passive、mode_double_cast、state_echo、manual_e、manual_r、flash_after_e、flash_after_r，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Zac

- 经 CXJ 交叉审计后升级为专属入口，加入 state_e_charge、state_passive、manual_e、cursor_e、auto_e，并保留 5 个官方形态与 E→W→Q→R 战斗顺序。

#### Yasuo

- 经 NG-AIO+HGVip+CXJ 交叉审计后升级为专属入口，加入 q_stack、dash_marks、minion_dash、eq、eq_flash、windwall、knockup_r、mode_e、state_q_stack、state_dash_marks、cursor_e、auto_r、flash_after_q、flash_after_eq，并保留 13 个官方形态与 Q→E→W→R 战斗顺序。

#### Velkoz

- 经 HGVip 交叉审计后升级为专属入口，加入 state_research、manual_e，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Taliyah

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 worked_ground、w_vector、e_dash、channel_r、magnet_q、state_w_push、state_w_pull、state_w_self_pull、manual_w、manual_r，并保留 9 个官方形态与 Q→E→W→R 战斗顺序。

#### Braum

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_q、manual_r、flash_after_q，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Kindred

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_marks，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Zeri

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_attack、charged_passive、wall_w、wall_e、r_effectiveness、state_q_attack、state_r_effectiveness、manual_w、auto_q、force_qq，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### TahmKench

- 经 CXJ 交叉审计后升级为专属入口，加入 farm_q、state_acquired_taste、manual_q、manual_w、ally_r、force_r、auto_q，并保留 6 个官方形态与 Q→W→E→R 战斗顺序。

#### Senna

- 经 CXJ 交叉审计后升级为专属入口，加入 state_soul_pickup、state_ward_q、manual_q、manual_w、manual_r、ally_q，并保留 5 个官方形态与 Q→W→E→R 战斗顺序。

#### Lucian

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 passive_weave、extended_q、r_magnet、magnet_r、farm_extended_q，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Zed

- 经 NG-AIO+CXJ 交叉审计后升级为专属入口，加入 shadow_tracking、multi_origin_q、shadow_e、weq、death_mark、safe_swap、mode_combo、state_safe_flash_combo、state_shadows、manual_weq、force_r，并保留 8 个官方形态与 R→W→E→Q 战斗顺序。

#### Vi

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_q_charge、manual_q、force_r、flash_after_q，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Aatrox

- 经 CXJ 交叉审计后升级为专属入口，加入 state_q_stage、manual_w、flash_after_q，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Nami

- 经 Q-Aio 交叉审计后升级为专属入口，加入 state_auto_heal、state_heal_only、manual_q、manual_r，并保留 4 个官方形态与 W→E→Q→R 战斗顺序。

#### Yuumi

- 经 CXJ 交叉审计后升级为专属入口，加入 auto_full、state_attach，并保留 13 个官方形态与 Q→E→W→R 战斗顺序。

#### Samira

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 style、melee_q、projectile_w、dash_reset、r_gate、safe_e、state_style、manual_q、manual_e、flash_after_q，并保留 7 个官方形态与 Q→E→W→R 战斗顺序。

#### Thresh

- 经 HGVip+CXJ 交叉审计后升级为专属入口，加入 q_recast、lantern_ally、e_direction、state_e_push、state_e_pull、manual_q、ally_w，并保留 8 个官方形态与 Q→E→W→R 战斗顺序。

#### Illaoi

- 经 NG-AIO 交叉审计后升级为专属入口，加入 spirit_priority、w_attack_reset、heartsteel_wait、multi_r、state_soul_spells、state_soul_attacks、manual_e、flash_after_r，并保留 4 个官方形态与 E→Q→W→R 战斗顺序。

#### Bard

- 经 CXJ 交叉审计后升级为专属入口，加入 manual_r、flash_after_q、force_w，并保留 14 个官方形态与 Q→W→E→R 战斗顺序。

#### Xayah

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 feathers、e_root、r_reposition、magnet_r、state_feathers、manual_r，并保留 4 个官方形态与 E→W→Q→R 战斗顺序。

#### Sylas

- 经 HGVip 交叉审计后升级为专属入口，加入 state_e2_offset、state_double_w_guard、state_e_feint、safe_turret、manual_r、flash_after_r，并保留 6 个官方形态与 W→E→Q→R 战斗顺序。

#### Neeko

- 经 CXJ 交叉审计后升级为专属入口，加入 state_disguise、manual_e、flash_after_e、flash_after_r，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。

#### Aphelios

- 经 HGVip+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 weapon_state、mark_range、weapon_swap、state_weapon_control、manual_q、manual_r、force_r、pause_w，并保留 11 个官方形态与 Q→E→W→R 战斗顺序。

#### Rell

- 经 CXJ 交叉审计后升级为专属入口，加入 state_mount、manual_w、manual_wr、flash_after_q、flash_after_w、flash_after_r，并保留 5 个官方形态与 W→E→Q→R 战斗顺序。

#### Yone

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 q_stack、spirit_return、safe_r、state_q3_stack、state_e2_offset、state_r_cc_offset、manual_r、auto_q、flash_after_q、pause_e，并保留 6 个官方形态与 Q→E→W→R 战斗顺序。

#### Ambessa

- 经 CXJ 交叉审计后升级为专属入口，加入 block_w、mode_combat、safe_turret、manual_r、flash_after_q，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Mel

- 经 NG-AIO+CXJ+Q-Aio 交叉审计后升级为专属入口，加入 multi_q、reserve_w、reflect_lethal、e_setup、r_reserve、block_w、state_r_reserve、manual_q、manual_e、auto_q、flash_after_e，并保留 4 个官方形态与 E→Q→R→W 战斗顺序。

#### Lillia

- 经 CXJ 交叉审计后升级为专属入口，加入 magnet_q、state_outer_ring、state_drag、safe_w、flash_after_q，并保留 7 个官方形态与 Q→W→E→R 战斗顺序。

#### Gwen

- 经 Q-Aio 交叉审计后升级为专属入口，加入 manual_r，并保留 10 个官方形态与 Q→E→W→R 战斗顺序。

#### Renata

- 经 CXJ 交叉审计后升级为专属入口，加入 mode_q_recast、manual_q、manual_r、manual_qr、force_w，并保留 5 个官方形态与 E→W→Q→R 战斗顺序。

#### Nilah

- 经 Q-Aio 交叉审计后升级为专属入口，加入 mode_farm、flash_after_q、flash_after_e、flash_after_r、force_e、cursor_e，并保留 4 个官方形态与 Q→E→W→R 战斗顺序。

#### Smolder

- 经 CXJ 交叉审计后升级为专属入口，加入 safe_e、state_stacks、manual_w、manual_r，并保留 4 个官方形态与 Q→W→E→R 战斗顺序。

#### Milio

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 ally_shield、interrupt_q、cleanse_r、manual_q，并保留 5 个官方形态与 E→W→Q→R 战斗顺序。

#### Zaahen

- 经 CXJ+Q-Aio 交叉审计后升级为专属入口，加入 recast_state、resource、execute、mode_farm、state_r_aoe、state_taunt、manual_w、manual_r、flash_after_w、force_w、pause_e、pause_r，并保留 6 个官方形态与 Q→E→W→R 战斗顺序。

#### Naafiri

- 经 CXJ 交叉审计后升级为专属入口，加入 safe_w、auto_q、flash_after_q、force_r、force_w、pause_e，并保留 5 个官方形态与 Q→E→W→R 战斗顺序。
<!-- MESH-AIO:RELEASE:v2.25.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

- [v2.24.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.24.0)
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
