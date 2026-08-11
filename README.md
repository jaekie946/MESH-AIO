<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.2.0:START -->
## v3.2.0

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

- v3.2.0은 로드 직후 화면 상단에 현재 MESH AIO 버전을, 화면 중앙에 `MESH TG : Click`을 최대 12초 동안 표시합니다. `Click`에서 마우스를 놓으면 공식 Hanbot 클립보드 API로 텔레그램 초대 링크를 복사합니다.
- 상점·Tab·가까운 적 챔피언·적 라인 미니언이 있으면 오버레이를 숨기고 클릭 상태를 즉시 폐기합니다. 12초가 끝나면 draw callback 자체를 제거해 정상 플레이 중 프레임 비용을 남기지 않습니다.
- MGoD Orb와 함께 로드하면 MESH가 같은 텔레그램 표시를 소유하는 12초 마감 시각을 공용 orb 계층에 게시합니다. 갱신된 MGoD는 그동안 중복 링크를 숨겨 두 스크립트가 한 줄씩만 표시됩니다.
- 모든 메뉴는 Hanbot 본체의 영어/중국어 설정을 계속 따릅니다. 평탄화된 keybind는 지원되지 않는 `set("value")`/`set("visible")`를 호출하지 않고 새 키를 런타임 권위로 쓰므로 로드 치명 오류를 막습니다. 기존에 직접 바꾼 키는 새 패널에서 한 번 재지정해야 할 수 있습니다.
- 팜 helper 입력의 `damage(unit)`를 전수 검사하고 after-attack 스트림을 사용한 뒤 즉시 닫도록 보강했습니다. 고정 문자열·상태·피해 계산은 로드 또는 저빈도 캐시에만 두어 정상 플레이의 draw/tick 비용도 줄였습니다.
- Lua·메뉴·공식 계약의 정적 검사는 통과했지만, 두 샤드의 실제 로드 순서·키 저장 복원·클릭 복사·12초 callback 해제·백스윙 타이밍은 F12에서 별도로 확인해야 합니다.

#### Jhin

- W 팜 helper에 실제 W 피해 함수를 제공해 라인 정리 중 `orb2/main` nil 비교가 나지 않도록 했습니다.

#### Jinx

- W 팜 helper의 피해 입력 누락을 고쳤고, Q/W 범위는 보이는 Drawings 토글과 준비 상태만 따릅니다. 숨김 출처 옵션이 W OFF를 다시 켜거나 상세 HUD가 기본 표시되는 문제도 제거했습니다.

#### TwistedFate

- Q 팜 helper에 실제 Q 피해 함수를 연결해 라인 정리 대상 비교가 항상 숫자로 계산되도록 했습니다.

#### Lux

- 평타 뒤 표적 기록을 마치거나 Evade가 활성화되면 after-attack 스트림을 즉시 닫아 불필요한 반복 callback을 막았습니다.

#### JarvanIV

- League Classic Jarvan IV의 실제 백스윙 표식 뒤 after-attack 스트림을 닫고, Evade 틱에서는 기록과 동작을 모두 중단합니다.

#### Malphite

- League Classic Malphite의 백스윙 표식은 한 번만 갱신하고 스트림을 즉시 닫아 W 위빙 감시가 상시 반복되지 않게 했습니다.

#### MasterYi

- League Classic Master Yi의 백스윙 표식과 Evade 소유권을 보존하면서 after-attack 스트림을 매 공격마다 종료합니다.

#### MissFortune

- League Classic Miss Fortune의 백스윙 표식 뒤 스트림을 즉시 닫아 다음 실제 평타 전까지 같은 callback이 반복되지 않게 했습니다.

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

- v3.2.0 shows the current MESH AIO version at the top of the screen and `MESH TG : Click` in the middle for up to 12 seconds after load. Releasing the mouse over `Click` copies the Telegram invite through Hanbot's documented clipboard API.
- The overlay hides in the shop, while Tab is held, or near enemy champions and lane minions, clearing any pending click immediately. Its draw callback removes itself after 12 seconds, leaving no normal-play frame cost.
- When MGoD Orb is loaded beside MESH, MESH publishes the shared 12-second promotion deadline through the orb layer. The updated MGoD hides its duplicate link during that window, so only one Telegram line is shown.
- Menus still follow Hanbot's English/Chinese setting. Flattened keybinds no longer call unsupported `set("value")` or `set("visible")`; the new visible key is the runtime authority, preventing the fatal load error. A previously customised key may need to be rebound once in the new panel.
- Farm-helper `damage(unit)` inputs are exhaustively checked and after-attack streams now close immediately after use. Fixed text, status, and damage work stays in load-time or low-frequency caches to reduce normal draw/tick cost.
- Static Lua, menu, and official-contract checks pass, while actual dual-shard load order, saved-key restore, clipboard copy, callback removal, and backswing timing remain separate F12 checks.

#### Jhin

- Supplies Jhin W's real damage function to the farm helper, preventing the `orb2/main` nil comparison during lane clear.

#### Jinx

- Fixes the missing W farm damage input. Q/W ranges now obey only the visible Drawings toggles and readiness, so a hidden source switch cannot re-enable W and optional status rows stay opt-in.

#### TwistedFate

- Connects Twisted Fate Q's real damage to the farm helper so every clear-target comparison remains numeric.

#### Lux

- Closes the after-attack stream after recording the target, and immediately closes it without acting on an Evade tick.

#### JarvanIV

- League Classic Jarvan IV now closes the after-attack stream after a real backswing marker and performs no marker work during Evade.

#### Malphite

- League Classic Malphite records one backswing and closes the stream, avoiding continuous monitoring between real W-weave attacks.

#### MasterYi

- League Classic Master Yi preserves its backswing marker and Evade ownership while closing each after-attack stream.

#### MissFortune

- League Classic Miss Fortune closes the stream after its backswing marker so the callback does not repeat before the next real attack.

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

- v3.2.0 在加载后最多 12 秒内，于屏幕顶部显示当前 MESH AIO 版本，并在屏幕中部显示 `MESH TG : Click`。在 `Click` 上松开鼠标时，会通过 Hanbot 官方剪贴板 API 复制 Telegram 邀请链接。
- 商店打开、按住 Tab、附近有敌方英雄或敌方兵线单位时，覆盖层会隐藏并立即清除待处理点击。12 秒后 draw callback 会自行移除，不给正常游戏留下帧开销。
- 与 MGoD Orb 同时加载时，MESH 会通过共用 orb 层发布 12 秒宣传截止时间。更新后的 MGoD 在该窗口内隐藏重复链接，因此只显示一条 Telegram 信息。
- 菜单继续跟随 Hanbot 本体的英文/中文设置。扁平化 keybind 不再调用不支持的 `set("value")` 或 `set("visible")`，而由新的可见按键作为运行时权威，从而避免致命加载错误；旧版自定义按键可能需要在新面板中重新绑定一次。
- 已全量检查农兵 helper 的 `damage(unit)` 输入，并在使用后立即关闭 after-attack 流。固定文本、状态和伤害计算仅放在加载阶段或低频缓存中，降低正常 draw/tick 开销。
- 静态 Lua、菜单与官方契约检查均已通过；双 shard 加载顺序、按键存档恢复、剪贴板复制、callback 移除和后摇时机仍需 F12 单独确认。

#### Jhin

- 为烬 W 农兵 helper 提供真实伤害函数，避免清线时出现 `orb2/main` 空值比较。

#### Jinx

- 修复金克丝 W 农兵伤害输入缺失。Q/W 范围现在只服从可见 Drawings 开关和技能就绪状态，隐藏来源开关不会重新开启 W，可选状态行也保持手动启用。

#### TwistedFate

- 将崔斯特 Q 的真实伤害连接到农兵 helper，使清线目标比较始终使用数值。

#### Lux

- 拉克丝记录平A目标后立即关闭 after-attack 流，并在 Evade 生效时直接关闭且不执行动作。

#### JarvanIV

- League Classic 嘉文四世在真实后摇标记后关闭 after-attack 流，Evade 期间不记录也不执行。

#### Malphite

- League Classic 墨菲特只记录一次后摇并关闭流，避免在真实 W 穿插攻击之间持续监控。

#### MasterYi

- League Classic 易保留后摇标记与 Evade 所有权，同时在每次攻击后关闭流。

#### MissFortune

- League Classic 厄运小姐在后摇标记后关闭流，避免下次真实攻击前重复 callback。
<!-- MESH-AIO:RELEASE:v3.2.0:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
