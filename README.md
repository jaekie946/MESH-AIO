<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.11.0:START -->
## v2.11.0

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

- 버전: v2.11.0. Riot Data Dragon 16.15.1과 패치 고정 16.15 클라이언트 원본 기준의 173챔피언(전용 22, 공용 151) 지원을 그대로 유지합니다.
- 갱플랭크 첫 인게임 실측(F12) 피드백을 반영한 수정 릴리즈입니다.

#### Orianna

- 프레임 드랍을 개선했습니다: 상태줄 문자열과 글자 폭을 매 프레임 새로 만들던 것을 값이 바뀔 때만 갱신하도록 캐시하고, 처치 가능 판정을 초당 5회로 제한했으며, 공 주변 W/R 원과 사거리 원의 그리기 세그먼트를 줄였습니다. 표시 내용은 동일합니다.

#### Gangplank

- 화약통 추적이 실제로 동작하도록 고쳤습니다. 실측 결과 통 오브젝트는 아군 팀이 아니라 중립 목록에 `gangplankbarrel`로 존재해, 팀 검사 때문에 추적기가 통을 하나도 인식하지 못했습니다. 이제 통을 정상 인식하므로 준비된 통 격발·사슬 연계가 작동합니다.
- 통 무한 설치를 막았습니다. 이미 대상 근처를 덮는 통이 있거나 진행 중인 설치가 있으면 새 통을 절대 추가하지 않고 격발을 기다립니다.
- E 시작 통에 두 가지 방식을 추가했습니다(기본: 내 쪽 설치). 내 옆에 안전하게 첫 통을 깔고 상대 쪽으로 연결 통을 이어 터트리는 방식과, 지금까지처럼 상대 위치에 바로 까는 방식 중 선택할 수 있습니다.
- 세미 R(Space)가 맨땅이 아니라 항상 적 챔피언에게 조준되도록 고쳤습니다. 마우스에 가장 가까운 적이 기준이며, 비슷한 거리면 더 많은 적을 덮는 지점을 고릅니다.
- Q 막타(약탈 골드·은화 스택)가 라인클리어뿐 아니라 하레스 모드와 라스트힛 모드에서도 동작합니다. 하레스 중에는 막타가 챔피언 견제 Q보다 우선하며, Q는 어느 모드에서든 처치가 확정된 미니언에게만 사용됩니다.
- Q 막타가 정글 몬스터에도 동작합니다(중립 목록을 스캔하지 않아 라인에서만 되던 문제 수정). 막타 우선순위는 처치 가능한 대포·슈퍼 미니언 최우선, 그 외에는 체력이 가장 낮은 미니언 순입니다. 자기 화약통은 막타 대상에서 제외됩니다.
- 트리플 배럴 옵션(기본 켜짐): 콤보에서 화약통을 최대 3개까지 연계해 사거리를 늘립니다.
- 자동 콤보의 사슬이 E-Q-E 방식으로 바뀌었습니다(사용자 교리): 미리 둘째 통을 까는 기존 E-E-Q는 적이 통을 부수거나 피하기 쉬워, 이제 준비된 통이 연결 거리 1~2개 안에 대상을 두면 즉시 Q로 격발하고 후속 통들은 Q·퓨즈가 날아가는 동안 실시간 대상 위치로 이어집니다(대상이 움직이면 자연스럽게 사선 연결).
- 시작 통 위치를 N 키로 실시간 전환할 수 있습니다(내 쪽 / 상대 쪽, 상태줄에 EnemySide로 표시). 메뉴 드롭다운은 기본값이고 토글이 뒤집습니다.
- 세미 통(X1MB)이 이제 안정적으로 격발합니다: 수동 키는 명시적 의도이므로 준비된 통이면 주변 적 여부와 무관하게 즉시 터뜨립니다.
- E-Q-E(G)의 간헐 동작 두 가지를 고쳤습니다: Q가 쿨다운이어도 첫 통을 미리 깔고(대기 중 Q가 돌아옴), Q 격발과 같은 틱에 나가는 두 번째 통이 내부 틱 가드에 먹혀 무작위로 빠지던 문제를 직접 시전으로 해결했습니다.
- E-Q-E(G)는 거리 적응형이 되었습니다: 대상이 E-Q-E 사거리면 두 통으로, 그보다 멀고 충전이 3개 있으면 자동으로 E-Q-E-E 세 통 체인으로 실행합니다. 첫 통은 항상 연결 거리의 정수 배만큼 대상 뒤에 깔려 마지막 통이 대상 정중앙에 떨어지고, 세 번째 통은 공식 0.5초 설치 간격에 맞춰 키를 떼도 자동으로 이어집니다.
- 전 챔피언 스탯 판독을 감사해 표준화했습니다: 총 AD·AP·보너스 AD를 문서화된 필드에서 우선 읽습니다. 수동 합성으로 아이템 스탯이 빠지던 모듈(아칼리·키아나·렝가·탈론·티모·갱플랭크)을 모두 수정해 피해 과소평가로 인한 막타·킬 판정 누락을 없앴고, 새 챔피언 제작 가이드에 표준으로 등재했습니다.
- 전 챔피언 드로우 성능 표준을 도입했습니다: 공용 캐시 모듈이 상태줄 문자열·글자 폭을 메모화하고, 원 그리기 세그먼트에 상한을 두었으며, 22개 전용 모듈과 공용 엔진(151챔피언) 전체에 일괄 적용했습니다. 매 프레임 문자열 생성이 유발하던 주기적 프레임 드랍이 사라집니다.
- 배포 페이지를 정리했습니다: 릴리즈 본문과 업데이트 히스토리의 지원 챔피언 173명 목록이 접힌 상태로 표시되고, 공개 README 첫 페이지는 최신 버전 전문만 보여주며 이전 버전들은 각 Release 링크 목록으로 압축됩니다.
- Q 피해 계산을 바로잡았습니다: 총 공격력을 표준 필드로 읽어 아이템 공격력이 빠지던 과소평가를 없앴고, 치명타 확률이 사실상 확정(87.5% 초과)일 때는 치명타 배수까지 반영합니다. 이제 Q가 충분히 처치 가능한 미니언·몬스터 막타를 놓치지 않습니다.
- 원거리 오프너 통은 사슬을 완성할 충전이 실제로 있을 때만 깝니다: 충전 1개로 먼 곳에 깔린 통이 영영 연계되지 못하던 낭비를 막았습니다(E-Q-E는 2개, E-Q-E-E는 3개 필요).
- 사슬 연계가 한 번 어긋난 뒤 조용히 영영 멈추던 문제를 고쳤습니다: 내부 연계 상태가 키를 떼거나 콜백이 누락되면 지워지지 않아 이후 모든 변환을 차단했습니다. 이제 6초 강제 만료와, 격발 후 0.15초 안에 콜백이 없으면 후속 통을 직접 이어가는 폴백이 있습니다.
- 격발 방식을 예측 리드에서 관측 기반으로 바꿨습니다(정확함 우선): Q는 통 체력이 실제로 1로 관측된 뒤에만 나가며, 슬라이더는 그 위에 추가 지연을 얹습니다. 미리 쏘다 통만 깎던 실수가 사라집니다.
- E-Q-E(G)가 기존 화약통을 활용합니다: Q 격발 사거리 안의 통이 대상까지의 연결 창에 맞으면 새 통을 깔지 않고 그 통을 앵커로 채택해 바로 격발 대기에 들어갑니다(세미 통 키와 동일한 원칙). 이미 대상을 덮는 통이면 격발만 하고 후속 통도 아낍니다.
- E-E-Q 폴백을 추가했습니다: 통이 아직 감소 중이거나 Q가 쿨다운이라 E-Q-E를 지금 칠 수 없으면 연장 통을 미리 깔아 두고, 준비되는 순간 사슬 전체를 격발합니다.
- 콤보 중 발생하던 치명적 스크립트 오류를 고쳤습니다(이 런타임에 없는 내장 함수 `next`를 처형 Q 판정에서 호출). 판정은 동작 그대로 안전한 방식으로 대체했습니다.
- 콤보 타겟 탐색이 Q/E 사거리(1000)로 잘려 있어, 발밑의 준비된 통으로 체인이 닿는 먼 적(최대 약 2400)에게 아무 것도 하지 않던 문제를 고쳤습니다. 이제 통 플레이의 실제 도달 거리까지 타겟을 잡습니다.
- 평타 격발 연계를 추가했습니다: 준비된 통이 평타 사거리 안이면 Q를 아끼고 평타로 격발하며, 격발 순간 후속 통이 퓨즈를 타고 이어집니다(평-E). 통이 평타 밖이면 기존처럼 Q 트리거(Q-E)를 씁니다.
- 콤보에서 챔피언 직접 Q는 이제 처형 전용입니다: Q 한 발로 죽는 적이거나 통 플레이가 아예 불가능할 때(통·충전 전무)만 나갑니다. 하레스 견제 Q는 그대로입니다.
- 화약통 설치 간격이 연결 거리 슬라이더의 경계값 그대로여서 실제로는 이어지지 않던 문제를 고쳤습니다: 모든 자동/세미 배치는 이제 슬라이더보다 60유닛 안쪽으로 깔려 경계 오차로 사슬이 끊기지 않습니다(기존 통 감지·표시는 슬라이더 값 그대로).
- Q 리드 격발이 너무 일찍 나가 통을 터뜨리지 못하고 체력만 깎던 버그를 고쳤습니다: 감소 틱 경계 정각에 도착하도록 쏘던 것을, 내장 150ms 안전 여유(+ 슬라이더 추가분)만큼 틱이 지난 뒤 도착하도록 바꿨습니다. 평타 격발은 관측 체력이 1일 때만 나갑니다.
- 자동 한타 R를 추가했습니다(기본 켜짐): 궁은 글로벌이므로 모든 적을 후보 중심으로 보고, 설정한 인원(기본 3명, 조절 가능)이 525 충격파 안에 확실히 들어오는 최적 지점에 자동 시전합니다. 명중 신뢰도 옵션을 켜면 0.5초 시전 동안 걸어 나갈 수 없는 적만 셉니다.
- 세미 통(X1MB)은 마우스 위치가 아니라 마우스 방향 최대 거리에 설치합니다: 기존 통이 있으면 그 통에서 연결 거리 최대로 연장하고, 없으면 Q가 직접 닿는 최대 거리에 깝니다(짧은 거리 낭비 수정).

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

- Version: v2.11.0. 173-champion support (22 hand-tuned, 151 shared-engine) stays on Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client data.
- A fix release from Gangplank's first in-game F12 feedback.

#### Orianna

- Improved frame drops: status-line strings and text widths are now cached and rebuilt only when a value changes, the killable check runs five times per second instead of every frame, and the W/R circles around the ball plus the range circles use fewer draw segments. What is shown is unchanged.

#### Gangplank

- Barrel tracking now actually works: the live keg object sits in the NEUTRAL list as `gangplankbarrel`, not on the ally team, so the team check made the tracker see zero barrels. With kegs recognized, ready-keg detonations and chain plays function.
- Stopped the infinite barrel placement: while a keg already covers the target or an opener is still in play, nothing new is placed - the play waits for the detonation.
- The opening barrel now has two modes (default: my side). Either a safe keg next to me chained toward the enemy and detonated, or the previous behavior of placing directly on the enemy.
- Semi R (Space) now always aims at an enemy champion instead of bare ground: the enemy nearest the mouse wins, with the denser cluster breaking near-ties.
- The Plunder Q last hit (gold and Silver Serpent stacks) now also runs in Harass and Last-Hit modes, not just lane clear. During harass the last hit outranks the champion poke, and Q is only ever spent on a minion it actually kills.
- The Q last hit now also works on jungle monsters (the neutral list was not scanned, so only lane worked). Priority: a killable cannon/super minion always first, then the lowest-health minion; our own kegs are excluded as targets.
- Triple barrel option (default on): Combo chains up to three kegs for range.
- The automatic combo chain now plays E-Q-E (user doctrine): the old pre-placed second keg (E-E-Q) was visible and got broken or dodged, so a ready keg within one or two links of the target is Q-detonated immediately and the follow-up kegs land while the Q and fuse are already in the air, aimed at the target's live position (naturally diagonal when they move).
- The opening barrel side flips in real time on N (my side / enemy side, shown as EnemySide in the status list). The menu dropdown is the default and the toggle inverts it.
- The semi barrel (X1MB) now detonates reliably: a held manual key is explicit intent, so any ready keg is blown regardless of nearby enemies.
- Two intermittent E-Q-E (G) issues are fixed: the first keg now drops even while Q is cooling (Q returns during the decay wait), and the second keg no longer randomly disappears when it left on the same tick as the Q - it is cast directly past the per-tick guard.
- E-Q-E (G) is now distance-adaptive: inside E-Q-E reach it plays two kegs, and beyond that - with three charges banked - it automatically runs the three-keg E-Q-E-E chain. The first keg always sits a whole number of links short of the target so the LAST keg lands exactly on them, and the third keg follows on the official 0.5-second between-barrels clock even if the key is released.
- Audited and standardized stat reads across every champion: total AD, AP, and bonus AD now read the documented fields first. Modules whose hand-composed math dropped item stats (Akali, Qiyana, Rengar, Talon, Teemo, Gangplank) are all fixed, removing missed last hits and kill checks from under-estimated damage, and the rule is recorded in the champion-building guide.
- Introduced a draw-performance standard for every champion: a shared cache module memoizes status-line strings and text widths, circle segment counts are capped, and the change is applied across all 22 dedicated modules and the shared engine covering the other 151 champions. The periodic frame drops caused by per-frame string building are gone.
- Cleaned up the distribution pages: the 173-champion support list is now collapsed in release notes and the update history, and the public README front page shows only the latest version in full with older versions compacted to a list of release links.
- Fixed the Q damage calculation: total attack damage now reads the standard field (item AD was being dropped), and a practically guaranteed crit (above 87.5%) applies the crit multiplier. Q no longer skips minions and monsters it can clearly execute.
- A far opener keg is only placed when the charges to finish the chain are actually banked: one banked charge used to strand a far keg that could never connect (E-Q-E needs two, E-Q-E-E needs three).
- Fixed chain plays silently stopping forever after one miss: the internal play state was never cleared when the key was released or a callback went missing, vetoing every later conversion. It now hard-expires after 6 seconds, and a 0.15-second fired-timeout places the follow-up keg directly when the callback never arrives.
- Detonation switched from predictive lead to observation (accuracy first): the Q only goes after the keg's health is actually SEEN at 1, with the slider adding delay on top. The early shots that merely shaved kegs are gone.
- E-Q-E (G) now uses existing kegs: a live keg inside Q-trigger reach whose distance to the target fits a links window is adopted as the anchor with no new placement at all (the same principle as the semi barrel key), and a keg already covering the target just detonates without spending follow-ups.
- Added the E-E-Q fallback: when E-Q-E cannot trigger right now - the keg is still decaying or Q is cooling - the extension keg is pre-placed and the whole chain detonates the moment it reads ready.
- Fixed a fatal script error during combo (the execute-Q check called the built-in `next`, which this runtime does not provide); the check now uses a safe equivalent with identical behavior.
- Fixed the combo target scan being capped at Q/E range (1000): a READY keg at your feet chains to enemies up to roughly 2400 away, but such enemies produced no action at all. The scan now covers the real keg-play reach.
- Added the basic-attack trigger chain: a ready keg inside attack range is detonated with an auto (saving the Q) and the follow-up kegs ride the fuse the moment the attack fires; kegs out of attack reach keep the Q trigger.
- Combo direct Q on champions is now execute-only: it fires when one Q kills, or when no keg play is possible at all (no kegs, no charges). The harass poke Q is unchanged.
- Fixed kegs being seated at exactly the link-distance boundary, where they failed to actually connect: every automatic and semi placement now undershoots the slider by 60 units so a boundary error can never break the chain (detection and drawing of existing kegs keep the raw value).
- Fixed the Q lead firing too early: aiming the arrival exactly at the decay-tick boundary made the shot land a few dozen milliseconds before the real tick, shaving the keg to 1 instead of detonating it. The arrival now trails the tick by a built-in 150 ms safety margin (plus the slider), and the basic-attack detonation only goes when the observed health already reads 1.
- Added the automatic teamfight R (default on): the barrage is global, so every enemy is a candidate zone center and it fires at the best spot reliably holding the configured head-count (default 3, adjustable). With the accuracy option on, only enemies that cannot walk out during the 0.5-second cast are counted.
- The semi barrel (X1MB) now places at maximum reach toward the mouse instead of at the mouse: a full link from the keg nearest the mouse when one exists, else the farthest point a direct Q can still trigger (short placements were wasted).

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

- 版本：v2.11.0。继续基于 Riot Data Dragon 16.15.1 与补丁锁定的 16.15 客户端原始数据支持 173 位英雄（22 个专属、151 个共用引擎）。
- 这是根据普朗克首次游戏内 F12 实测反馈的修复版本。

#### Orianna

- 改善了掉帧：状态栏字符串与文字宽度改为仅在数值变化时重建，可击杀判定改为每秒 5 次而非每帧，围绕球的 W/R 圆圈与射程圈使用更少的绘制段数。显示内容不变。

#### Gangplank

- 火药桶追踪现已真正生效：实测桶对象以 `gangplankbarrel` 存在于中立列表而非友方队伍，队伍检查导致追踪器一个桶都识别不到。桶被正确识别后，就绪桶引爆与桶链连招均可运作。
- 修复了无限放桶：当已有桶覆盖目标或开局桶仍在进行中时，不再放置新桶，而是等待引爆。
- 起手桶新增两种模式（默认：己方侧）。可以在自己身边安全放第一个桶并向敌方接链引爆，或沿用之前直接放在敌人位置的方式。
- 半手动 R（Space）现在始终瞄准敌方英雄而非空地：以离鼠标最近的敌人为准，距离接近时选择覆盖更多敌人的位置。
- 掠夺 Q 尾刀（金币与银蛇币层数）现在也在骚扰模式和尾刀模式下生效，而不仅是清线模式。骚扰时尾刀优先于对英雄的消耗 Q，且任何模式下 Q 只用于确定能击杀的小兵。
- Q 尾刀现在对野怪也生效（此前未扫描中立列表，只有兵线可用）。优先级：可击杀的炮车/超级兵永远优先，其余按血量最低的小兵；自己的火药桶不会被当作尾刀目标。
- 三桶选项（默认开启）：连招中最多连接三个火药桶来延伸距离。
- 自动连招的桶链改为 E-Q-E 方式（用户教义）：旧的预放第二桶（E-E-Q）容易被敌人打掉或躲开，现在只要就绪的桶在距目标一到两个连接距离内就立即用 Q 引爆，后续桶在 Q 与引信飞行期间按目标实时位置接上（目标移动时自然形成斜线连接）。
- 起手桶位置可用 N 键实时切换（己方侧 / 敌方侧，状态栏显示 EnemySide）。菜单下拉为默认值，切换键将其反转。
- 半自动放桶（X1MB）现在稳定引爆：按住手动键即明确意图，只要有就绪的桶就立刻引爆，无论附近有无敌人。
- 修复了 E-Q-E（G）的两个间歇性问题：Q 冷却中也会先放第一个桶（等待期间 Q 会转好）；与 Q 同一帧发出的第二个桶不再被内部帧保护随机吞掉，改为直接施放。
- E-Q-E（G）现在按距离自适应：目标在 E-Q-E 射程内时使用两个桶；更远且备有三层充能时，自动执行三桶的 E-Q-E-E 连锁。第一个桶始终放在距目标整数个连接距离之后，使最后一个桶正好落在目标身上；第三个桶按官方 0.5 秒放桶间隔自动接上，即使松开按键也会完成。
- 审计并标准化了所有英雄的属性读取：总攻击力、法强与额外攻击力现在优先读取文档化字段。手动合成漏算装备属性的模块（阿卡丽、奇亚娜、雷恩加尔、塔隆、提莫、普朗克）已全部修正，消除了因伤害低估导致的尾刀与击杀判定遗漏，并将该规则写入英雄制作指南。
- 为所有英雄引入绘制性能标准：共用缓存模块记忆化状态栏字符串与文字宽度，限制圆圈绘制段数，并统一应用于全部 22 个专属模块与覆盖其余 151 位英雄的共用引擎。由逐帧字符串构建引起的周期性掉帧不复存在。
- 清理了发布页面：支持英雄 173 人列表在发布说明与更新历史中默认折叠；公开 README 首页只完整展示最新版本，旧版本压缩为各 Release 链接列表。
- 修正了 Q 伤害计算：总攻击力改读标准字段（此前漏算装备攻击力），且暴击率接近必定（高于 87.5%）时计入暴击倍率。Q 不再错过明明能击杀的小兵与野怪。
- 只有当完成桶链所需的充能确实备好时才会放远距离起手桶：此前仅剩 1 层充能时放出的远桶永远无法连接（E-Q-E 需 2 层，E-Q-E-E 需 3 层）。
- 修复了桶链在一次失误后永久静默停摆的问题：内部连招状态在松开按键或回调丢失时不会清除，从而否决之后的所有转换。现在有 6 秒强制过期，且引爆后 0.15 秒内无回调时直接补放后续桶。
- 引爆方式从预测提前改为基于观测（准确优先）：Q 只在实际观测到桶血量为 1 之后才发出，滑条在此之上追加延迟。提前射击只削桶的失误不再发生。
- E-Q-E（G）现在会利用已有的火药桶：Q 触发距离内、且到目标距离符合连接窗口的桶会被直接采纳为锚点而不再新放桶（与半自动放桶键相同原则）；已覆盖目标的桶则直接引爆，不再消耗后续桶。
- 新增 E-E-Q 后备：当桶仍在衰减或 Q 在冷却而无法立即 E-Q-E 时，先把延伸桶放好，待桶就绪的瞬间引爆整条链。
- 修复了连招期间的致命脚本错误（处决 Q 判定调用了本运行时不存在的内置函数 `next`）；判定改用行为完全一致的安全写法。
- 修复了连招目标扫描被限制在 Q/E 射程（1000）的问题：脚下就绪的桶实际可连锁到约 2400 外的敌人，但此前对这些敌人毫无动作。现在扫描覆盖真实的桶链可达距离。
- 新增普攻引爆连锁：就绪的桶在普攻距离内时用普攻引爆（节省 Q），攻击出手的瞬间后续桶沿引信接上；桶在普攻距离外时仍用 Q 触发。
- 连招中对英雄的直接 Q 现在仅用于处决：只有一发 Q 能击杀、或完全无法进行桶连招（无桶无充能）时才施放。骚扰消耗 Q 不变。
- 修复了火药桶恰好放在连接距离滑条边界值上而实际无法连接的问题：所有自动/半自动放置现在比滑条值收进 60 单位，使边界误差不再断链（对已存在桶的检测与绘制仍使用原值）。
- 修复了 Q 提前引爆过早的问题：此前瞄准衰减刻度边界的精确时刻，导致弹丸比真实刻度早几十毫秒到达，只把桶削到 1 而没有引爆。现在到达时刻会滞后刻度一个内置 150 毫秒安全余量（加滑条附加值），普攻引爆只在观测血量已为 1 时进行。
- 新增自动团战 R（默认开启）：大招为全图施放，因此以每个敌人为候选中心，在可靠容纳设定人数（默认 3 人，可调）的最佳位置自动施放。开启命中可靠性选项时，只统计在 0.5 秒施法期间走不出范围的敌人。
- 半自动放桶（X1MB）改为朝鼠标方向的最大距离放置而非鼠标位置：已有桶时从离鼠标最近的桶延伸一个完整连接距离，否则放在 Q 能直接触发的最远处（修复近距离浪费）。
<!-- MESH-AIO:RELEASE:v2.11.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
