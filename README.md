<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.2.1:START -->
## v3.2.1

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

- v3.2.1은 MESH AIO, MGoD Orb, `[MESH]Evade`를 각각 단독으로 쓸 수 있게 유지하면서 함께 로드했을 때만 공개 Evade API로 주문 소유권을 양보합니다. 어느 구성요소도 다른 둘을 필수로 로드하지 않습니다.
- 현대 173명과 League Classic 60명 전부의 시작 순서를 감사했습니다. 시작 때 Evade가 없으면 핸들이 영구 nil이던 현대 69명과 Classic 20명은 0.5초 간격으로만 재탐색하고, 발견 즉시 임시 callback을 제거합니다. 이미 늦은 로드를 지원하던 144개 모듈은 그대로 유지했습니다.
- Evade 활성 중에도 별도 공격·이동·시전을 낼 수 있던 콜백 16곳을 Evade-first로 닫았습니다. 일반 tick뿐 아니라 pre-attack, after-attack, spell, castspell, issue-order 경로가 같은 소유권 규칙을 따릅니다.
- Evade v1의 targeted collection은 아직 완전 준비 상태가 아니므로 Ezreal, Irelia, Samira, Sivir, Vladimir의 보조 방어는 `targeted_ready=true`일 때만 사용합니다. Sivir는 `is_cc`와 `isHardCC` 양쪽 명칭을 인식합니다.
- Evade가 설치되지 않은 사용자는 기존 AIO 동작을 그대로 사용합니다. unresolved 상태의 공용 resolver는 매 tick 시간 비교만 하고 실제 module 조회는 0.5초마다 제한해 프레임 비용을 억제합니다.
- Lua·173 AIO·60 Classic·메뉴·팜·공식 데이터·위빙 계약의 정적 검사는 통과했지만, 임의 로드 순서와 실제 회피 시작 틱의 주문 양보, targeted readiness 전환은 F12에서 별도로 확인해야 합니다.

#### Akshan

- Evade 활성 중 pre-attack이 두 번째 평타 상태를 바꾸지 않도록 했습니다.

#### Briar

- 포탑 spell callback의 자동 Q보다 Evade 소유권과 pending 정리를 먼저 처리합니다.

#### Camille

- pre-attack 자동 Q가 Evade 틱에 실행되지 않습니다.

#### Ezreal

- targeted Evade 데이터가 완전 준비됐다고 명시된 경우에만 해당 보조 방어를 사용합니다.

#### Hecarim

- Evade 활성 중 사용자 공격 명령을 차단하거나 공격 pause를 걸지 않도록 issue-order 순서를 교정했습니다.

#### Illaoi

- 영혼 끌기 반응 R보다 Evade 소유권을 먼저 확인합니다.

#### Irelia

- pre-attack E와 targeted 보조 판정을 모두 Evade 활성·readiness 계약 뒤로 옮겼습니다.

#### JarvanIV

- pre-attack E가 Evade 틱에는 실행되지 않습니다.

#### Jhin

- 치명타 취소용 pause와 이동보다 Evade를 먼저 확인하고 pending 상태를 안전하게 정리합니다.

#### Malphite

- W pre-attack/after-attack 두 경로를 모두 Evade-first로 닫고 after-attack 스트림도 종료합니다.

#### RekSai

- pre-attack Q가 Evade 틱에는 실행되지 않습니다.

#### Samira

- Evade 활성 중 pre-attack 타깃을 오브워커에 다시 주입하지 않으며 targeted 보조는 readiness를 확인합니다.

#### Sivir

- targeted 보조는 readiness를 확인하고 하드 CC 데이터는 `is_cc`와 `isHardCC`를 모두 지원합니다.

#### Teemo

- after-attack 이모트/Q보다 Evade를 먼저 확인하고 스트림을 즉시 닫습니다.

#### Thresh

- spell callback의 자동 랜턴보다 Evade 소유권을 먼저 확인합니다.

#### TwistedFate

- 평타 callback의 자동 Q보다 Evade를 먼저 확인하고 카드 reset 상태를 정리합니다.

#### Vladimir

- targeted Evade collection이 준비된 경우에만 해당 보조 방어를 사용합니다.

#### Warwick

- castspell callback에서 Q release보다 Evade 소유권을 먼저 확인합니다.

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

- v3.2.1 keeps MESH AIO, MGoD Orb, and `[MESH]Evade` independently usable. When combined, AIO yields order ownership only through the public Evade facade; none of the three hard-loads either companion.
- Startup order was audited across all 173 modern and 60 League Classic modules. The 69 modern and 20 Classic modules whose Evade handle could remain permanently nil now retry only every 0.5 seconds and remove the temporary callback immediately after adoption. The existing 144 lazy paths remain unchanged.
- Sixteen action callbacks that could still attack, move, or cast during Evade are now Evade-first, including pre-attack, after-attack, spell, castspell, and issue-order paths.
- Evade v1 does not yet claim a complete targeted collection. Ezreal, Irelia, Samira, Sivir, and Vladimir therefore consume those defenses only when `targeted_ready=true`; Sivir accepts both `is_cc` and `isHardCC` aliases.
- Users without Evade retain the existing AIO behavior. While unresolved, the shared resolver performs only a time check each tick and limits the actual module lookup to once every 0.5 seconds.
- Static Lua, 173-AIO, 60-Classic, menu, farm, official-data, and weave checks pass. Arbitrary live load order, first-threat order yielding, and targeted-readiness transitions remain separate F12 checks.

#### Akshan

- The pre-attack callback no longer mutates second-shot state while Evade is active.

#### Briar

- Evade ownership and pending cleanup now run before the turret-spell callback can cast Q.

#### Camille

- The automatic pre-attack Q no longer fires on an Evade-owned tick.

#### Ezreal

- Targeted Evade defenses are used only when the facade explicitly reports that collection ready.

#### Hecarim

- Issue-order now checks Evade before suppressing a user attack or applying an attack pause.

#### Illaoi

- Evade ownership is checked before the spirit-grab reactive R.

#### Irelia

- Both pre-attack E and targeted defenses now sit behind Evade-active and readiness contracts.

#### JarvanIV

- The pre-attack E no longer fires during Evade.

#### Jhin

- Crit-cancel pause and movement check Evade first and safely discard pending state.

#### Malphite

- Both W pre-attack and after-attack paths are Evade-first and close the after-attack stream.

#### RekSai

- The pre-attack Q no longer fires during Evade.

#### Samira

- Pre-attack no longer injects an orbwalker target during Evade, and targeted defenses require readiness.

#### Sivir

- Targeted defenses require readiness and hard-CC metadata accepts both `is_cc` and `isHardCC`.

#### Teemo

- After-attack emote/Q checks Evade first and closes the stream immediately.

#### Thresh

- Spell-callback lantern automation now checks Evade ownership first.

#### TwistedFate

- Attack-callback Q checks Evade first and clears the card-reset state.

#### Vladimir

- Targeted Evade defenses run only after the collection reports ready.

#### Warwick

- The castspell callback checks Evade ownership before releasing Q.

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

- v3.2.1 保持 MESH AIO、MGoD Orb 与 `[MESH]Evade` 均可独立使用；共同加载时，AIO 只通过公开 Evade facade 让出指令所有权，三者互不硬加载。
- 已审计 173 个现代英雄与 60 个 League Classic 模块的加载顺序。原本可能永久保留空 Evade 句柄的 69 个现代模块和 20 个 Classic 模块，现在最多每 0.5 秒重查一次，接入后立即移除临时 callback；原有 144 条延迟加载路径保持不变。
- 16 个原本可能在 Evade 期间继续攻击、移动或施法的回调已改为 Evade-first，覆盖 pre-attack、after-attack、spell、castspell 与 issue-order。
- Evade v1 尚未声明完整 targeted collection，因此 Ezreal、Irelia、Samira、Sivir、Vladimir 仅在 `targeted_ready=true` 时使用该防御；Sivir 同时识别 `is_cc` 与 `isHardCC`。
- 未安装 Evade 的用户保持原有 AIO 行为。未解析时，共用 resolver 每 tick 只做时间比较，实际 module 查询限制为每 0.5 秒一次。
- 静态 Lua、173 AIO、60 Classic、菜单、农兵、官方数据与 weave 检查均已通过；真实任意加载顺序、首个威胁 tick 的指令让权和 targeted readiness 变化仍需 F12 验证。

#### Akshan

- Evade 生效时，pre-attack 不再修改第二次普攻状态。

#### Briar

- 炮塔 spell callback 自动施放 Q 前，先处理 Evade 所有权与 pending 清理。

#### Camille

- Evade 所有的 tick 中不再自动触发 pre-attack Q。

#### Ezreal

- 仅在 facade 明确报告 targeted collection 已就绪时使用该防御。

#### Hecarim

- issue-order 会先检查 Evade，再决定是否拦截用户攻击或添加攻击暂停。

#### Illaoi

- 灵魂拉取后的反应 R 之前先检查 Evade 所有权。

#### Irelia

- pre-attack E 与 targeted 防御均受 Evade active 和 readiness 契约保护。

#### JarvanIV

- Evade 期间不再触发 pre-attack E。

#### Jhin

- 暴击取消的暂停与移动先检查 Evade，并安全清除 pending 状态。

#### Malphite

- W 的 pre-attack 与 after-attack 两条路径均改为 Evade-first，并关闭 after-attack 流。

#### RekSai

- Evade 期间不再触发 pre-attack Q。

#### Samira

- Evade 期间 pre-attack 不再注入目标，targeted 防御也要求 readiness。

#### Sivir

- targeted 防御要求 readiness，硬控数据同时支持 `is_cc` 与 `isHardCC`。

#### Teemo

- after-attack 的表情/Q 先检查 Evade，并立即关闭该流。

#### Thresh

- spell callback 的自动灯笼现在先检查 Evade 所有权。

#### TwistedFate

- 普攻 callback 的自动 Q 先检查 Evade，并清理卡牌 reset 状态。

#### Vladimir

- 仅在 targeted Evade collection 报告就绪后使用该防御。

#### Warwick

- castspell callback 会在释放 Q 前先检查 Evade 所有权。
<!-- MESH-AIO:RELEASE:v3.2.1:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
