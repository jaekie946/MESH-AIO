<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.4.12:START -->
## v3.4.12

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

- 982개 Lua 전체를 프레임 비용 관점에서 재감사했습니다. 화면 그리기 콜백 안에서 매 프레임 문자열을 만들거나 타겟 선택·피해 계산을 반복하던 9개 모듈을 찾았고, 전부 0.05~0.15초 스냅샷 캐시 또는 1회 생성 재사용으로 바꿨습니다. 조준·시전·판단 로직은 바꾸지 않았습니다.
- 이 감사로 프레임마다 쌓이던 임시 문자열/테이블 쓰레기가 줄어 잦은 GC 멈춤에 의한 미세 프레임 드랍이 감소합니다. 표시 내용은 동일하며 갱신 주기만 사람 눈에 구분되지 않는 스냅샷 간격으로 제한됩니다.
- 회귀 검사기가 이제 드로우 캐시 호출 인벤토리 54곳을 고정해, 이후 작업에서 캐시 없이 화면 콜백에 계산을 되돌리면 CI가 실패합니다.

#### Karthus

- League Classic 전용 모듈의 '죽음 무시' 남은 시간 표시가 매 프레임 문자열을 만들지 않고 0.1초 스냅샷을 재사용합니다.
- Farm/Auto R 키 상태 줄은 네 가지 조합 문자열을 한 번만 만들어 재사용합니다. 표시 내용은 같습니다.

#### Katarina

- League Classic 전용 모듈의 Farm/Tower E 키 상태 줄이 조합별 문자열을 한 번만 만들어 재사용합니다.

#### MonkeyKing

- League Classic 전용 모듈의 Farm/Tower E 키 상태 줄이 조합별 문자열을 한 번만 만들어 재사용합니다.

#### Rammus

- 현대 모듈의 Q/W/자동 R 상태 줄이 여덟 가지 조합 문자열을 한 번만 만들어 재사용합니다.
- League Classic 모듈의 파워볼 남은 시간 표시가 0.05초 스냅샷을 재사용해 매 프레임 포맷을 없앴습니다.

#### Rumble

- 피해 표시가 켜져 있을 때 매 프레임 수행하던 타겟 선택과 콤보 피해 계산·문자열 포맷을 0.15초 스냅샷으로 옮겼습니다. 표시 위치는 매 프레임 실제 대상 위치를 따라갑니다.

#### Swain

- E 회수 대상의 속박 남은 시간 표시가 0.1초 스냅샷을 재사용해 매 프레임 문자열 생성을 없앴습니다.

#### Veigar

- League Classic 전용 모듈의 콤보 피해 표시가 매 프레임 수행하던 타겟 선택·감옥 콤보 피해 계산·문자열 포맷을 0.15초 스냅샷으로 옮겼습니다. 실제 시전 판단은 바뀌지 않습니다.

#### Warwick

- League Classic 전용 모듈의 처치 가능(LETHAL) 판정이 매 프레임 Q+R 피해 합산을 하지 않고 0.15초 스냅샷을 사용합니다.
- W 지속시간 표시도 0.1초 스냅샷을 재사용해 매 프레임 포맷을 없앴습니다.

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

- All 982 Lua files were re-audited for per-frame cost. Nine modules built strings or ran target selection and damage math inside the draw callback every frame; all of them now use 0.05-0.15 s snapshot caches or build-once reuse. Aiming, casting, and decision logic are unchanged.
- This removes the per-frame garbage that caused frequent GC pauses and micro frame drops. Displayed content is identical; only the refresh cadence is capped at snapshot intervals indistinguishable to the eye.
- The regression checker now pins the 54 draw-cache call sites, so any future change that moves computation back into a draw callback without a cache fails CI.

#### Karthus

- The League Classic module's Death Defied countdown reuses a 0.1 s snapshot instead of formatting a new string every frame.
- The Farm/Auto R key status line builds its four combination strings once and reuses them. The displayed content is unchanged.

#### Katarina

- The League Classic module's Farm/Tower E key status line builds each combination string once and reuses it.

#### MonkeyKing

- The League Classic module's Farm/Tower E key status line builds each combination string once and reuses it.

#### Rammus

- The modern module's Q/W/Auto R status line builds its eight combination strings once and reuses them.
- The League Classic module's Powerball countdown reuses a 0.05 s snapshot, removing the per-frame format call.

#### Rumble

- With the damage overlay enabled, the per-frame target selection, combo damage math, and string formatting moved to a 0.15 s snapshot. The overlay position still follows the target's live position every frame.

#### Swain

- The root-remaining countdown on the E pull target reuses a 0.1 s snapshot, removing the per-frame string build.

#### Veigar

- The League Classic module's combo damage overlay moved its per-frame target selection, caged-combo damage math, and string formatting to a 0.15 s snapshot. Actual cast decisions are unchanged.

#### Warwick

- The League Classic module's LETHAL verdict uses a 0.15 s snapshot instead of summing Q+R damage every frame.
- The W duration display also reuses a 0.1 s snapshot, removing the per-frame format call.

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

- 对全部982个Lua文件重新进行了每帧开销审计。共发现9个模块在绘制回调中每帧构建字符串或执行目标选择与伤害计算，现已全部改为0.05~0.15秒快照缓存或一次生成后复用。瞄准、施法与判断逻辑均未改变。
- 此项审计消除了每帧产生的临时字符串/表垃圾，减少了由频繁GC暂停引起的细微掉帧。显示内容不变，仅刷新节奏被限制在肉眼无法分辨的快照间隔。
- 回归检查器现在固定54处绘制缓存调用点，之后若有改动把计算移回未缓存的绘制回调，CI将直接失败。

#### Karthus

- 英雄联盟经典模式模块的“死亡不灭”倒计时改为复用0.1秒快照，不再每帧生成新字符串。
- Farm/自动R按键状态行的四种组合字符串只生成一次并复用，显示内容不变。

#### Katarina

- 英雄联盟经典模式模块的 Farm/塔下E 按键状态行改为每种组合只生成一次字符串并复用。

#### MonkeyKing

- 英雄联盟经典模式模块的 Farm/塔下E 按键状态行改为每种组合只生成一次字符串并复用。

#### Rammus

- 现代模块的 Q/W/自动R 状态行的八种组合字符串只生成一次并复用。
- 英雄联盟经典模式模块的滚球倒计时改为复用0.05秒快照，去除了每帧格式化。

#### Rumble

- 开启伤害显示时，原本每帧执行的目标选择、连招伤害计算与字符串格式化改为0.15秒快照。显示位置仍然每帧跟随目标实际位置。

#### Swain

- E 拉回目标的束缚剩余时间显示改为复用0.1秒快照，不再每帧生成字符串。

#### Veigar

- 英雄联盟经典模式模块的连招伤害显示把每帧的目标选择、牢笼连招伤害计算与字符串格式化改为0.15秒快照。实际施法判断不变。

#### Warwick

- 英雄联盟经典模式模块的可击杀(LETHAL)判定改为0.15秒快照，不再每帧累加Q+R伤害。
- W 持续时间显示同样复用0.1秒快照，去除了每帧格式化。
<!-- MESH-AIO:RELEASE:v3.4.12:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

- [v3.4.10](https://github.com/jaekie946/MESH-AIO/releases/tag/v3.4.10)
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
