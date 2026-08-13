<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.4.10:START -->
## v3.4.10

### 한국어

#### 지원 챔피언

- 애니
- 올라프
- 갈리오
- 트위스티드 페이트
- 신 짜오
- 우르곳
- 르블랑
- 블라디미르
- 피들스틱
- 케일
- 마스터 이
- 알리스타
- 라이즈
- 사이온
- 시비르
- 소라카
- 티모
- 트리스타나
- 워윅
- 누누와 윌럼프
- 미스 포츈
- 애쉬
- 트린다미어
- 잭스
- 모르가나
- 질리언
- 신지드
- 이블린
- 트위치
- 카서스
- 초가스
- 아무무
- 람머스
- 애니비아
- 샤코
- 문도 박사
- 소나
- 카사딘
- 이렐리아
- 잔나
- 갱플랭크
- 코르키
- 카르마
- 타릭
- 베이가
- 트런들
- 스웨인
- 케이틀린
- 블리츠크랭크
- 말파이트
- 카타리나
- 녹턴
- 마오카이
- 레넥톤
- 자르반 4세
- 엘리스
- 오리아나
- 오공
- 브랜드
- 리 신
- 베인
- 럼블
- 카시오페아
- 스카너
- 하이머딩거
- 나서스
- 니달리
- 우디르
- 뽀삐
- 그라가스
- 판테온
- 이즈리얼
- 모데카이저
- 요릭
- 아칼리
- 케넨
- 가렌
- 레오나
- 말자하
- 탈론
- 리븐
- 코그모
- 쉔
- 럭스
- 제라스
- 쉬바나
- 아리
- 그레이브즈
- 피즈
- 볼리베어
- 렝가
- 바루스
- 노틸러스
- 빅토르
- 세주아니
- 피오라
- 직스
- 룰루
- 드레이븐
- 헤카림
- 카직스
- 다리우스
- 제이스
- 리산드라
- 다이애나
- 퀸
- 신드라
- 아우렐리온 솔
- 케인
- 조이
- 자이라
- 카이사
- 세라핀
- 나르
- 자크
- 야스오
- 벨코즈
- 탈리야
- 카밀
- 아크샨
- 벨베스
- 브라움
- 진
- 킨드레드
- 제리
- 징크스
- 탐 켄치
- 브라이어
- 비에고
- 세나
- 루시안
- 제드
- 클레드
- 에코
- 키아나
- 바이
- 아트록스
- 나미
- 아지르
- 유미
- 사미라
- 쓰레쉬
- 일라오이
- 렉사이
- 아이번
- 칼리스타
- 바드
- 라칸
- 자야
- 오른
- 사일러스
- 니코
- 아펠리오스
- 렐
- 파이크
- 벡스
- 요네
- 암베사
- 멜
- 유나라
- 로크
- 세트
- 릴리아
- 그웬
- 레나타 글라스크
- 오로라
- 닐라
- 크산테
- 스몰더
- 밀리오
- 자헨
- 흐웨이
- 나피리

#### 핵심 및 메뉴

- 현대 173명과 League Classic 63명의 Console Debug를 고정 메뉴 루트 `[MESH AIO] - Global Settings > AIO Console Debug` 하나로 통합했습니다. 한 번 설정하면 챔피언을 바꾸거나 스크립트를 다시 불러와도 같은 값이 유지됩니다.
- 로더가 실제 런타임 `charName`을 공식 alias 표로 정규화한 뒤 챔피언 폴더를 찾습니다. Fiddlesticks처럼 런타임 이름과 공식 키가 다른 챔피언이 전용 모듈 대신 공용 경로로 떨어지던 문제를 없앴고, 로드 성공·실패 경로를 콘솔에 남깁니다.
- 236챔피언의 원형 논타겟 자동 조준 146곳을 전수 점검해, 예측 지점이 실제 사거리 밖일 때 사거리 경계로 끌어당겨 쏘던 21개 경로를 실패 폐쇄했습니다. 이제 사거리 안에 들어온 예측 지점에만 시전합니다.
- 공식 데이터를 Data Dragon 16.16.1과 클라이언트 16.16.8049184로 재수집해 173챔피언·868아이템·참고자료 50종을 같은 패치로 맞췄습니다. 173개 스크립트 시트도 공식 캐시 전용 생성기로 16.16에서 다시 만들었습니다.
- 선택 설치형 `[MESH]Evade`가 실제 위험을 게시한 틱에는 수동키를 포함한 모든 자동 동작이 회피에 우선권을 넘깁니다. Evade를 나중에 켜도 0.5초 간격 재탐색으로 연결됩니다.

#### Brand

- W는 예측 중심점이 실제 사거리 안일 때만 시전합니다. 도망치는 적을 향해 사거리 끝으로 던져 빗나가던 자동 W가 사라졌습니다.
- E는 Q용 원거리 조준점과 분리해 675 사거리 안의 적을 다시 고릅니다. Q가 먼 대상을 노리는 동안 E가 사거리 밖으로 나가지 않습니다.

#### Fiddlesticks

- 런타임 이름이 공식 키와 달라 전용 모듈 대신 공용 경로로 로드되던 문제를 alias 표로 고쳤습니다. 이제 전용 상태기가 실제로 실행됩니다.
- League Classic 까마귀 폭풍은 보존된 시전 도착 지점에 실제로 도달한 뒤에만 채널 상태로 넘어갑니다.

#### Graves

- 평타 백스윙이 열린 직후의 E 대시를 Q/W 위빙보다 먼저 시도해 AA-E-AA 리셋을 놓치지 않습니다.
- Combo R을 자동 R 마스터 옵션에서 분리했습니다. 자동 R을 꺼도 Combo 중 R이 계속 나갑니다.

#### KogMaw

- 메뉴에 없던 숨은 자동 마스터 스위치를 제거했습니다. Combo·Harass·Auto R 옵션이 각각 직접 시전을 소유하므로 켠 항목이 그대로 동작합니다.
- 세미 R 입력은 여전히 자동 R보다 먼저 처리되어 수동 조준이 자동 판단에 밀리지 않습니다.

#### MasterYi

- E에 걸려 있던 숨은 패시브·Q·R·공격속도 조건을 제거했습니다. 메뉴에서 켠 조건대로만 E가 나갑니다.
- 평타 백스윙에서 W가 서버에 수락되면 즉시 평타를 리셋하고 후속 공격 명령을 보내 AA-W-AA를 실제로 완성합니다.

#### Mordekaiser

- Riot 16.16 원본에서 사라진 아레나 전용 R 능력치 탈취 0.08 오버라이드를 더 이상 쓰지 않습니다. 모든 모드에서 공식 수치 0.10으로 피해와 처치 표시를 계산합니다.

#### Viktor

- Debug를 켠 상태에서 같은 슬롯의 시전 로그를 250ms 단위로 묶고 억제된 횟수를 1초 상태 줄에 합쳐 콘솔 폭주를 없앴습니다. 시전 타이밍 자체는 바뀌지 않습니다.
- Evade가 소유한 틱과 일시정지 틱에서는 화면 표시에만 쓰는 피해 계산을 건너뛰고, 상태 표시줄 문자열과 테이블을 재사용해 프레임 비용을 줄였습니다.

#### Xayah

- `Farm (MMB)` 토글이 네이티브 키와 저장값 하나만 권위로 씁니다. 이전에는 내부 미러값이 남아 실제로는 꺼져 있는데 켜진 것처럼 동작하던 경우가 있었습니다.
- E는 깃털마다 귀환 도착 시각까지 현재선과 예측선을 모두 지나는 대상만 셉니다. 깃털이 많이 깔린 구간의 표시와 계산량도 함께 줄였습니다.

#### XinZhao

- 화면 표시 캐시의 만료 시간 계산 오류를 고쳐 사거리·표식 표시가 갱신되지 않고 멈추던 문제를 없앴습니다.

#### Zeri

- 파밍 Q가 같은 미니언에 대해 예측·충돌·지형 검사를 막타용과 푸시용으로 두 번 수행하던 경로를 한 번의 결과 재사용으로 줄였습니다. 대상 선택 결과는 같습니다.

### English

#### Supported Champions

- Annie
- Olaf
- Galio
- Twisted Fate
- Xin Zhao
- Urgot
- LeBlanc
- Vladimir
- Fiddlesticks
- Kayle
- Master Yi
- Alistar
- Ryze
- Sion
- Sivir
- Soraka
- Teemo
- Tristana
- Warwick
- Nunu & Willump
- Miss Fortune
- Ashe
- Tryndamere
- Jax
- Morgana
- Zilean
- Singed
- Evelynn
- Twitch
- Karthus
- Cho'Gath
- Amumu
- Rammus
- Anivia
- Shaco
- Dr. Mundo
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
- Jarvan IV
- Elise
- Orianna
- Wukong
- Brand
- Lee Sin
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
- Kog'Maw
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
- Kha'Zix
- Darius
- Jayce
- Lissandra
- Diana
- Quinn
- Syndra
- Aurelion Sol
- Kayn
- Zoe
- Zyra
- Kai'Sa
- Seraphine
- Gnar
- Zac
- Yasuo
- Vel'Koz
- Taliyah
- Camille
- Akshan
- Bel'Veth
- Braum
- Jhin
- Kindred
- Zeri
- Jinx
- Tahm Kench
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
- Rek'Sai
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
- Renata Glasc
- Aurora
- Nilah
- K'Sante
- Smolder
- Milio
- Zaahen
- Hwei
- Naafiri

#### Core & Menu

- Console Debug for all 173 modern and 63 League Classic champions now lives in one fixed menu root, `[MESH AIO] - Global Settings > AIO Console Debug`. Set it once and the value survives champion swaps and script reloads.
- The loader normalizes the live runtime `charName` through an official alias table before resolving the champion folder. Champions whose runtime name differs from their official key, such as Fiddlesticks, no longer fall back to the shared path, and both load success and failure are printed to the console.
- All 146 circular non-targeted auto-aim call sites across 236 champions were audited. The 21 paths that clamped an out-of-range prediction back onto the range boundary now fail closed, so these spells only fire when the predicted centre is genuinely inside range.
- Official data was recollected at Data Dragon 16.16.1 and client 16.16.8049184, aligning 173 champions, 868 items, and 50 reference sources on one patch. The 173 script sheets are regenerated at 16.16 from an official-cache-only generator.
- When the optional `[MESH]Evade` publishes real danger on a tick, every automatic action including manual hotkeys yields to the dodge. Enabling Evade later still connects through a 0.5 second rediscovery pass.

#### Brand

- W only fires when the predicted centre is genuinely inside range, removing the auto W that used to be thrown at the range edge toward a fleeing target and miss.
- E now picks its own target inside 675 range instead of reusing Q's long-range anchor, so E no longer fires out of range while Q is aiming at a distant enemy.

#### Fiddlesticks

- The alias table fixes the case where the live runtime name differed from the official key, which loaded the shared path instead of the dedicated module. The dedicated state machine now actually runs.
- League Classic Crowstorm only transitions into its channel state after it truly arrives at the preserved cast endpoint.

#### Graves

- The E dash is attempted ahead of Q/W weaving right after the attack backswing opens, so the AA-E-AA reset is no longer skipped.
- Combo R is separated from the automatic R master option, so R still fires during Combo while automatic R is off.

#### KogMaw

- The hidden automatic master switch that never appeared in the menu is gone. Combo, Harass, and Auto R each own their own casts, so whatever you enable is what runs.
- Semi R input is still processed ahead of automatic R, so manual aiming is never overridden by the automatic decision.

#### MasterYi

- The hidden passive, Q, R, and attack-speed gates on E are removed, so E fires exactly on the conditions you enabled in the menu.
- When W is accepted by the server during the attack backswing, the attack is reset immediately and a follow-up attack order is issued, which actually completes AA-W-AA.

#### Mordekaiser

- The Arena-only 0.08 R stat-steal override, which no longer exists in the Riot 16.16 source, is gone. Damage and kill indicators now use the official 0.10 value in every mode.

#### Viktor

- With Debug on, cast logs for the same slot are grouped into 250 ms buckets and the suppressed count is folded into the 1 Hz status line, which stops the console flood. Cast timing itself is unchanged.
- On ticks owned by Evade and on paused ticks, the draw-only damage computation is skipped and the status line strings and tables are reused, lowering per-frame cost.

#### Xayah

- The `Farm (MMB)` toggle now uses the native key and a single saved value as its only authority. Previously a stale internal mirror could keep the feature acting enabled while the visible toggle was off.
- E counts only the targets that cross both the current and predicted line up to each feather's own recall arrival time, and the draw and computation cost in dense feather situations is reduced.

#### XinZhao

- Fixed the draw cache expiry calculation so the range and mark overlays no longer freeze instead of refreshing.

#### Zeri

- Farm Q used to run prediction, collision, and wall checks twice on the same minion, once for the last hit and once for the push. It now reuses a single result, and the target selection outcome is unchanged.

### 简体中文

#### 支持英雄

- 黑暗之女
- 狂战士
- 正义巨像
- 卡牌大师
- 德邦总管
- 无畏战车
- 诡术妖姬
- 猩红收割者
- 远古恐惧
- 正义天使
- 无极剑圣
- 牛头酋长
- 符文法师
- 亡灵战神
- 战争女神
- 众星之子
- 迅捷斥候
- 麦林炮手
- 祖安怒兽
- 雪原双子
- 赏金猎人
- 寒冰射手
- 蛮族之王
- 武器大师
- 堕落天使
- 时光守护者
- 炼金术士
- 痛苦之拥
- 瘟疫之源
- 死亡颂唱者
- 虚空恐惧
- 殇之木乃伊
- 披甲龙龟
- 冰晶凤凰
- 恶魔小丑
- 祖安狂人
- 琴瑟仙女
- 虚空行者
- 刀锋舞者
- 风暴之怒
- 海洋之灾
- 英勇投弹手
- 天启者
- 瓦洛兰之盾
- 邪恶小法师
- 巨魔之王
- 诺克萨斯统领
- 皮城女警
- 蒸汽机器人
- 熔岩巨兽
- 不祥之刃
- 永恒梦魇
- 扭曲树精
- 荒漠屠夫
- 德玛西亚皇子
- 蜘蛛女皇
- 发条魔灵
- 齐天大圣
- 复仇焰魂
- 盲僧
- 暗夜猎手
- 机械公敌
- 魔蛇之拥
- 上古领主
- 大发明家
- 沙漠死神
- 狂野女猎手
- 兽灵行者
- 圣锤之毅
- 酒桶
- 不屈之枪
- 探险家
- 铁铠冥魂
- 牧魂人
- 离群之刺
- 狂暴之心
- 德玛西亚之力
- 曙光女神
- 虚空先知
- 刀锋之影
- 放逐之刃
- 深渊巨口
- 暮光之眼
- 光辉女郎
- 远古巫灵
- 龙血武姬
- 九尾妖狐
- 法外狂徒
- 潮汐海灵
- 不灭狂雷
- 傲之追猎者
- 惩戒之箭
- 深海泰坦
- 奥术先驱
- 北地之怒
- 无双剑姬
- 爆破鬼才
- 仙灵女巫
- 荣耀行刑官
- 战争之影
- 虚空掠夺者
- 诺克萨斯之手
- 未来守护者
- 冰霜女巫
- 皎月女神
- 德玛西亚之翼
- 暗黑元首
- 铸星龙王
- 影流之镰
- 暮光星灵
- 荆棘之兴
- 虚空之女
- 星籁歌姬
- 迷失之牙
- 生化魔人
- 疾风剑豪
- 虚空之眼
- 岩雀
- 青钢影
- 影哨
- 虚空女皇
- 弗雷尔卓德之心
- 戏命师
- 永猎双子
- 祖安花火
- 暴走萝莉
- 河流之王
- 狂厄蔷薇
- 破败之王
- 涤魂圣枪
- 圣枪游侠
- 影流之主
- 暴怒骑士
- 时间刺客
- 元素女皇
- 皮城执法官
- 暗裔剑魔
- 唤潮鲛姬
- 沙漠皇帝
- 魔法猫咪
- 沙漠玫瑰
- 魂锁典狱长
- 海兽祭司
- 虚空遁地兽
- 翠神
- 复仇之矛
- 星界游神
- 幻翎
- 逆羽
- 山隐之焰
- 解脱者
- 万花通灵
- 残月之肃
- 镕铁少女
- 血港鬼影
- 愁云使者
- 封魔剑魂
- 铁血狼母
- 流光镜影
- 不破之誓
- 灰烬驱魔人
- 腕豪
- 含羞蓓蕾
- 灵罗娃娃
- 炼金男爵
- 双界灵兔
- 不羁之悦
- 纳祖芒荣耀
- 炽炎雏龙
- 明烛
- 不落魔锋
- 异画师
- 百裂冥犬

#### 核心与菜单

- 现代173名与英雄联盟经典模式63名的控制台调试选项统一到固定菜单根 `[MESH AIO] - Global Settings > AIO Console Debug`。设置一次后，切换英雄或重新加载脚本都会保留该值。
- 加载器先通过官方别名表规范化实时运行名 `charName`，再解析英雄目录。像 Fiddlesticks 这类运行名与官方键不同的英雄不再退回到通用路径，并且加载成功与失败都会输出到控制台。
- 全面审计了236名英雄的146处圆形非指向自动瞄准调用。其中21条会把超出射程的预测点拉回射程边缘的路径现已失败关闭，只有预测中心确实处于射程内时才会释放。
- 官方数据按 Data Dragon 16.16.1 与客户端 16.16.8049184 重新采集，使173名英雄、868件装备与50项参考资料对齐到同一版本。173份脚本数据表也由仅使用官方缓存的生成器在16.16重新生成。
- 当可选安装的 `[MESH]Evade` 在某一帧发布真实危险时，包括手动热键在内的所有自动行为都会把优先权交给闪避。之后再启用 Evade 也会通过0.5秒的重新探测接上。

#### Brand

- W 仅在预测中心确实位于射程内时释放，不再朝逃跑目标沿射程边缘投掷并落空。
- E 不再沿用 Q 的远距离瞄准点，而是在675射程内重新选择目标，因此 Q 瞄准远处敌人时 E 不会超出射程。

#### Fiddlesticks

- 别名表修正了运行名与官方键不一致时加载通用路径而非专属模块的问题，专属状态机现在会真正运行。
- 英雄联盟经典模式的乌鸦风暴只有在真正到达所保留的施法落点后才会进入引导状态。

#### Graves

- 在普攻后摇刚开始时优先尝试 E 位移，而不是 Q/W 穿插，因此不会漏掉 AA-E-AA 重置。
- 连招 R 已从自动 R 主控选项中分离，关闭自动 R 后连招期间仍会释放 R。

#### KogMaw

- 移除了菜单中从未出现的隐藏自动主控开关。连招、骚扰与自动 R 各自拥有施法权，开启哪一项就执行哪一项。
- 半自动 R 输入仍优先于自动 R 处理，手动瞄准不会被自动判断覆盖。

#### MasterYi

- 移除了 E 上隐藏的被动、Q、R 与攻速判定条件，E 只按菜单中启用的条件释放。
- 普攻后摇期间 W 被服务器接受后立即重置普攻并发出后续攻击指令，从而真正完成 AA-W-AA。

#### Mordekaiser

- 不再使用 Riot 16.16 原始数据中已删除的竞技场专属 R 属性窃取0.08覆盖值。所有模式的伤害与击杀提示均按官方数值0.10计算。

#### Viktor

- 开启调试后，同一技能槽的施法日志按250毫秒合并，被抑制的次数并入每秒状态行，从而消除控制台刷屏。施法时机本身没有改变。
- 在由 Evade 拥有的帧和暂停帧上跳过仅用于绘制的伤害计算，并复用状态行的字符串与表，降低每帧开销。

#### Xayah

- `Farm (MMB)` 开关现在仅以原生按键与单一存档值为准。此前残留的内部镜像值可能导致显示为关闭时功能仍在运行。
- E 仅统计在各羽刃自身回收到达时间之前同时穿过当前线与预测线的目标，同时降低了羽刃密集时的绘制与计算开销。

#### XinZhao

- 修正了绘制缓存的过期时间计算，射程与标记显示不再停止刷新。

#### Zeri

- 清线 Q 此前会对同一小兵分别为补刀与推线各执行一次预测、碰撞与地形检测，现在改为复用同一结果，目标选择结果保持不变。
<!-- MESH-AIO:RELEASE:v3.4.10:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

- [v3.4.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.4.0)
- [v3.3.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.3.0)
- [v3.2.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.2.1)
- [v3.2.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.2.0)
- [v3.1.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.3)
- [v3.1.2](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.2)
- [v3.1.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.1.1)
- [v3.0.3](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.0.3)
- [v3.0.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.0.1)
- [v2.26.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.26.0)
- [v2.25.1](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.25.1)
- [v2.25.0](https://github.com/jaekie946/MESH-AIO/releases/tag/v2.25.0)
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
