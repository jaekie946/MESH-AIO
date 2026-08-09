<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.1.2:START -->
## v3.1.2

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

- v3.1.2는 현대 173명과 League Classic 60명 전부의 팜 동작 설정을 하나의 `Farm` 패널에 Q/W/E/R/Other로 모았습니다. 기존 옵션 ID·키·저장값·main getter는 유지하므로 저장 설정을 지울 필요가 없습니다.
- 중복 Clear/Last Hit 패널은 Farm으로 합치고, FXT/CXJ/CNo1 같은 참고 구현 패널은 숨긴 뒤 내부 옵션을 일반 Q/W/E/R/Hotkeys/Drawings/Additional behavior에 배치했습니다. 메뉴 구성은 로드 직후 한 번만 실행되고 callback이 제거됩니다.
- 234개 메뉴 루트와 13,215개 전체 문구는 Hanbot 본체가 중국어면 CP936/GBK 간체 중국어, 그 외에는 영어로 표시됩니다. 스크립트 언어 선택지는 없고, 한글 카탈로그는 미래 글꼴 지원용 dormant 상태로 남습니다.
- 챔피언 아래 공용 HUD는 기본 `Farm: ON/OFF` 한 줄만 유지합니다. General Debug를 켠 동안에만 1초마다 모드·맵·orb 키·현재 대상·windup·lock·Q/W/E/R live 상태를 `[mesh-debug]`로 기록하고, 끄면 공용 tick callback 자체가 없습니다.
- 일반 협곡의 `gameMode=CLASSIC`과 League Classic을 분리했습니다. JADE는 `Jade_*` 런타임 이름만 사용하고, 칼바람은 현대 챔피언 모듈과 ARAM 피해 보정을 유지합니다.
- 차징·채널형 스킬을 전수 감사해 이미 시작된 상태가 시작 키를 놓았다는 이유로 멈추지 않게 했습니다. 정적 검사와 캐시는 프레임 드랍 회귀를 막지만, 실제 서버 승인과 FPS는 F12/연습 도구에서 계속 확인해야 합니다.

#### Ezreal

- W는 이제 Q 준비 여부나 Q 예측 성공과 무관하게 자체 준비·마나·예측 조건만으로 사용합니다. W 시전이 승인된 경우에만 다음 Q가 비행 완료를 기다렸다가 표식 대상을 우선합니다.

#### Gangplank

- Farm이 켜진 상태에서 Harass를 누르면 챔피언 견제를 먼저 시도하고, 승인된 견제 시전이 없을 때 Lane Clear와 같은 예측 막타 Q로 미니언을 처치합니다.

#### Irelia

- 이미 승인된 W 충전은 Evade 뒤에서 전역적으로 유지되며 live W2 확인을 기다린 다음 안전하게 release합니다. 시작 모드가 바뀌어도 충전이 고아 상태로 남지 않습니다.

#### Jhin

- 정확한 재장전 버프 또는 공식 패시브 타이머를 확인하면 Combo/Harass에서 유효한 Q를 먼저 사용합니다. 중복 참고 구현 메뉴도 일반 스킬 메뉴로 평탄화했습니다.

#### Kalista

- Rend 표식의 서버 `endTime`을 `game.time`과 비교하도록 고쳐 잘못된 만료·리셋 판단을 제거했습니다. Harass 2단 점프 Q는 완료된 공격의 살아 있는 챔피언 대상이 확인될 때만 열려 허공 Q를 사용하지 않으며, E 판단 로그는 스택·잔여시간·피해·HP·거부 사유를 남깁니다.

#### Xerath

- R은 여전히 Space로만 시작하지만, 채널이 이미 활성화된 뒤에는 Combo를 누르고 있어도 준비되는 즉시 다음 탄을 계속 발사합니다. 자동 처치탄과 공식 탄 간격은 그대로 유지합니다.

#### Zeri

- 타워 Q는 Farm 토글과 실제 Lane Clear가 모두 활성이고, 오브워커가 그 타워를 현재 공격/클리어 대상으로 잡았을 때만 사용합니다. Combo는 타워 Q를 열지 않고 주변 타워를 임의 탐색하지 않습니다.

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

- v3.1.2 gathers every farm behavior control for all 173 modern and 60 League Classic champions into one Farm panel grouped by Q/W/E/R/Other. Existing option IDs, keys, saved values, and main getters remain authoritative, so saves do not need to be deleted.
- Duplicate Clear/Last Hit panels are consolidated into Farm. FXT/CXJ/CNo1 reference-family panels are hidden and their controls are placed in the normal spell, hotkey, drawing, Farm, or Additional behavior sections. Finalization runs once after load and removes its callback.
- All 234 menu roots and 13,215 whole strings follow Hanbot itself: CP936/GBK Simplified Chinese on a Chinese client and English otherwise. There is no script-side selector; the Korean catalogue remains dormant for a future font update.
- The shared under-champion HUD still defaults to one `Farm: ON/OFF` line. Only while General Debug is enabled, a one-Hz `[mesh-debug]` trace records mode/map, orb keys and target, windup/lock state, and live Q/W/E/R forms; its tick callback is absent when disabled.
- Ordinary Rift `gameMode=CLASSIC` is separated from League Classic. Only a `Jade_*` runtime champion selects JADE, while Howling Abyss keeps modern champion modules and ARAM damage balance.
- Charge and channel transports were audited so an accepted state no longer stalls merely because the start key changed. Static gates and caches prevent known frame-drop regressions, while real server acceptance and FPS remain Practice Tool/F12 checks.

#### Ezreal

- W now uses only its own readiness, mana, and prediction gates instead of depending on Q readiness or a successful Q prediction. Only an accepted W flight delays the next Q and gives the marked target priority.

#### Gangplank

- With Farm enabled, holding Harass tries champion harassment first and then uses the same predicted-lethal minion Q last hit as Lane Clear when no harassment cast is accepted.

#### Irelia

- An accepted W charge is maintained globally after Evade, waits for live W2 acknowledgement, and then releases safely even if the mode that started it has changed.

#### Jhin

- A confirmed reload buff or official passive timer now lets Combo/Harass use a valid Q before ordinary attack-windup protection. Duplicate reference-family controls are flattened into the normal spell menus.

#### Kalista

- Rend marker server endTime is now compared with game.time, removing false expiry/reset decisions. Harass double-hop Q requires a live champion from the completed attack and cannot fire at empty space; detailed E logs include stacks, remaining time, damage, HP, and rejection reason.

#### Xerath

- R still starts only from Space, but once its channel is active, held Combo also fires each newly ready follow-up pulse. Automatic lethal shots and the official shot interval remain intact.

#### Zeri

- Turret Q requires both Farm and the real Lane Clear mode, and the turret must be the orbwalker's current attack/clear target. Combo never opens turret Q, and nearby turrets are not scanned into invented targets.

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

- v3.1.2 将全部 173 个现代英雄与 60 个 League Classic 英雄的清线功能集中到一个 Farm 菜单，并按 Q/W/E/R/Other 分组。原有选项 ID、按键、存档值与 main getter 保持不变，无需删除存档。
- 重复的 Clear/Last Hit 菜单会合并到 Farm；FXT、CXJ、CNo1 等参考实现面板会隐藏，内部选项移到普通技能、按键、绘制、Farm 或 Additional behavior。整理只在加载后运行一次，并立即移除 callback。
- 234 个菜单根与 13,215 条完整文本继续跟随 Hanbot 主程序：中文客户端使用 CP936/GBK 简体中文，其他客户端使用 English。脚本内没有语言选择器，韩文目录仅为未来字体支持保留。
- 英雄下方默认仍只显示一行 `Farm: ON/OFF`。只有开启 General Debug 时，才会每秒输出一次 `[mesh-debug]`，记录模式、地图、orb 按键与目标、windup/lock 以及 Q/W/E/R 实时形态；关闭后没有公共 tick callback。
- 普通峡谷的 `gameMode=CLASSIC` 与 League Classic 已明确分离。只有 `Jade_*` 运行时英雄会进入 JADE，嚎哭深渊继续使用现代英雄模块与 ARAM 伤害平衡。
- 已审计蓄力与引导技能，已接受的状态不会因为起始按键改变而停住。静态检查与缓存会阻止已知掉帧回归，真实服务器接受与 FPS 仍需在训练模式/F12 验证。

#### Ezreal

- W 现在只检查自身的准备、法力与预测，不再依赖 Q 是否可用或 Q 预测是否成功。只有 W 施放被接受后，下一次 Q 才等待飞行并优先攻击带标记目标。

#### Gangplank

- Farm 开启时按住 Harass 会先尝试攻击英雄；若没有英雄技能被接受，则使用与 Lane Clear 相同的预测致死 Q 补刀小兵。

#### Irelia

- 已接受的 W 蓄力会在 Evade 之后全局维护，等待实时 W2 确认后安全释放，即使起始模式已经改变也不会留下孤立蓄力。

#### Jhin

- 确认装弹 buff 或官方被动计时后，Combo/Harass 会在普通攻击 windup 保护前使用有效 Q。重复的参考实现控制也已整理到普通技能菜单。

#### Kalista

- Rend 标记的服务器 endTime 现在与 game.time 比较，修复错误过期与重置判断。Harass 双跳 Q 必须来自已完成攻击的存活英雄目标，不会再向空地施放；E 详细日志会记录层数、剩余时间、伤害、生命值与拒绝原因。

#### Xerath

- R 仍只能由 Space 开始，但引导已经激活后，按住 Combo 也会在每发准备好时继续发射。自动致死炮与官方发射间隔保持不变。

#### Zeri

- 防御塔 Q 必须同时开启 Farm 与真实 Lane Clear，而且防御塔必须是 orbwalker 当前攻击/清线目标。Combo 不会开启防御塔 Q，也不会扫描附近防御塔制造目标。
<!-- MESH-AIO:RELEASE:v3.1.2:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
