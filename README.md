<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

## 다운로드 / Download / 下载

- **[mesh.shard 최신 버전 바로 받기 / Direct download / 直接下载](https://github.com/jaekie946/MESH-AIO/releases/latest/download/mesh.shard)**
- [최신 릴리즈 페이지 / Latest release / 最新版本页面](https://github.com/jaekie946/MESH-AIO/releases/latest) — 릴리즈 목록 대신 이 링크를 쓰면 최신 1개만 표시됩니다. Shows only the newest release. 只显示最新一个版本。

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v3.1.1:START -->
## v3.1.1

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

- v3.1.1은 모든 현대 173명과 League Classic 60명의 메뉴를 Hanbot 본체 언어에 맞춥니다. Hanbot이 중국어면 간체 중국어, 그 외에는 영어로 자동 표시하며 스크립트 안에 별도 언어 선택지는 만들지 않습니다.
- 총 234개 메뉴 루트와 13,213개 정적 문구를 전체 문구 단위로 처리합니다. 기존 동작 옵션 ID·키·저장값은 유지하고 새 HUD/오버레이는 새 ID를 사용하며, 동적 아군·적군 목록도 같은 언어의 접두어를 사용합니다.
- 중국어 메뉴는 UTF-8 한자를 직접 넘기지 않고 Hanbot이 요구하는 CP936/GBK 바이트를 Lua 10진 이스케이프로 생성합니다. 한글 전체 카탈로그는 향후 Hanbot 글꼴 지원용으로 보존하지만, 현재 렌더러가 한글을 `?`로 표시하므로 런타임에서는 로드하지 않습니다.
- 메뉴에 보이던 FXT/CXJ/CNo1 같은 참고 구현 이름을 제거하고, 모든 라벨은 사용자가 켜는 기능만 설명하도록 정리했습니다.
- 챔피언 아래 공용 상태 HUD는 기본으로 두 번째 줄의 `Farm: ON/OFF` 하나만 표시합니다. 기존 다른 상태 옵션은 메뉴에 유지되고 `Show other status lines`를 켜면 다시 보이며, 탄환·스택 같은 실제 자원은 숨기지 않습니다.
- 번역·문자 폭을 캐시하고 대상별 스택/피해/남은 HP 계산을 0.15~0.2초 snapshot으로 제한해 매 프레임 문자열·피해 계산으로 생기던 프레임 드랍을 막았습니다.
- 번역 생성기와 전수 검사기가 누락·오염·stale 생성물, 언어 혼입, raw UTF-8 중국어, 스크립트 selector 재도입, 234개 루트의 공용 래퍼 우회를 릴리즈 전에 차단합니다. 전체 Lua 표면은 966개입니다.
- 한글 글꼴 미지원과 GBK 중국어 출력은 인게임 증거로 확인했지만, 새 MESH shard의 실제 중국어 클라이언트 메뉴 표본은 F12 확인 대상으로 남깁니다.

#### Kalista

- E 자동 리셋을 시전 직전에 다시 계산합니다. live Rend 스택과 표식 잔여시간을 확인하고 공식식/실시간 피해 중 낮은 값, 물리·전체 실드, 10 또는 2%의 오차 여유를 반영해 확실한 처치만 허용합니다. Combo를 누르는 동안 챔피언이 사거리 밖이면 레인 미니언·실제 정글 몬스터·적 타워를 계속 공격 대상으로 잡아 평타와 Martial Poise 이동을 유지하며 식물은 제외합니다. 표식 대상 위에는 0.15초 캐시로 `E xN | -피해 | HP 현재 > 이후`를 표시합니다.

#### Tristana

- 부착된 E 대상 위에 현재 스택, 지금 터질 E 단독 피해, 폭발 후 HP를 함께 표시합니다. 물리·전체 실드를 반영하며 R+E 콤보 피해로 E 표시를 잘못 빨갛게 만들지 않습니다. 새 오버레이 글자 크기 ID를 사용해 예전 저장값과 충돌하지 않고 0.15초 캐시로 프레임별 재계산을 피합니다.

#### LeeSin

- Q 선형 예측과 충돌 검사가 `radius`만 받아 `pred/linear`·`pred/collision`에서 종료되던 문제를 `width=60`으로 수정했습니다. Star Combo의 Flash 옵션도 재로드 시 충돌하지 않는 고유 ID로 바꿨습니다.

#### Fiora

- Q 이동 지점용 선형 예측에 필수 width를 넣어 같은 nil 예측 오류를 막았습니다.

#### Hecarim

- R 이동 경로 예측에 공식 265 폭을 명시했습니다.

#### KSante

- Q와 W 충전 경로의 선형 예측 입력을 각각 공식 폭 필드로 교정했습니다.

#### Lillia

- 장거리로 굴러가는 E의 선형 예측에 공식 80 폭을 명시했습니다.

#### Milio

- Q 선형 예측과 충돌 검사가 같은 width 입력을 사용하도록 교정했습니다.

#### Renekton

- E 돌진 조준의 선형 예측에 공식 50 폭을 명시했습니다.

#### TwistedFate

- Q Wild Cards의 선형 예측에 공식 40 폭을 명시했습니다.

#### Yone

- Q/Q3/W/R의 직선 예측 입력이 `radius`만 전달해 Hanbot `pred/linear`에서 `width` nil로 종료되던 문제를 수정했습니다. Riot 16.15의 Q 55, Q3 80, W 100, R 225 폭을 명시하고 같은 회귀를 막는 전용 계약 검사를 추가했습니다.

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

- v3.1.1 makes all 173 modern and 60 League Classic champion menus follow Hanbot's own language. A Chinese Hanbot client gets Simplified Chinese; every other client gets English, with no script-side language selector.
- All 234 menu roots and 13,213 static display strings are handled as whole strings. Existing behavior-option IDs, keys, and saved values stay intact; new HUD/overlay controls use new IDs, and dynamic ally/enemy lists use the active-language prefix.
- Chinese menu text is emitted as CP936/GBK bytes in Lua decimal escapes rather than raw UTF-8 Chinese. The complete Korean catalogue remains dormant for a future Hanbot font update, because the current renderer substitutes every Hangul glyph with `?`.
- Reference implementation names such as FXT, CXJ, and CNo1 were removed from visible menus; every label now describes only the feature the user controls.
- The shared under-champion HUD shows only `Farm: ON/OFF` on the second row by default. Existing status options remain available behind `Show other status lines`, while true resources such as ammo and stacks remain visible under their own controls.
- Translation and text-width results are cached, while per-target stack, damage, and remaining-HP snapshots refresh every 0.15–0.2 seconds, avoiding per-frame string and damage work.
- Generation and exhaustive checks reject missing, contaminated, or stale translations, cross-language leakage, raw UTF-8 Chinese, a script-side selector, and any of the 234 roots bypassing the shared wrapper. The shard contains 966 Lua surfaces.
- In-game evidence established the missing Hangul glyphs and working GBK Chinese output; a Chinese-client sample of the new MESH shard still requires F12 verification.

#### Kalista

- Automatic Rend resets are recalculated immediately before cast. They require a live marker that survives the cast window and use the lower of Riot-formula and live damage, physical/all shields, plus a 10-damage or 2% safety margin. While Combo is held and the champion is out of reach, lane minions, real jungle monsters, or enemy turrets remain attack carriers so attacks and Martial Poise movement continue; plants are excluded. A 0.15-second cached line above marked targets shows `E xN | -damage | HP current > after`.

#### Tristana

- The attached E target now shows current stacks, current E-only detonation damage, and post-explosion HP together. Physical/all shields are included, and R+E combo damage no longer turns the E overlay lethal red. A new overlay-size ID avoids old-save collisions, and a 0.15-second cache prevents per-frame recalculation.

#### LeeSin

- Fixed Q linear prediction and collision inputs that passed only `radius` and terminated inside `pred/linear` or `pred/collision`; both now use `width=60`. Star Combo's Flash option also has a unique reload-safe ID.

#### Fiora

- Added the required width to Q movement-point linear prediction, preventing the same nil prediction failure.

#### Hecarim

- R path prediction now provides the official 265 width.

#### KSante

- Q and charged-W linear prediction inputs now provide their official width fields.

#### Lillia

- Long-range rolling E prediction now provides the official 80 width.

#### Milio

- Q linear prediction and collision now share the same width-bearing input.

#### Renekton

- E dash aiming now provides the official 50 width.

#### TwistedFate

- Wild Cards linear prediction now provides the official 40 width.

#### Yone

- Fixed Q/Q3/W/R linear prediction inputs that passed only `radius`, causing Hanbot `pred/linear` to terminate when `width` was nil. The Riot 16.15 widths—Q 55, Q3 80, W 100, and R 225—are explicit, with a dedicated regression contract.

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

- v3.1.1 让全部 173 个现代英雄与 60 个 League Classic 英雄菜单自动跟随 Hanbot 主程序语言。Hanbot 为中文时显示简体中文，其他语言显示 English，脚本内不再提供独立语言选择。
- 234 个菜单根与 13,213 条静态显示文本全部按完整句子处理。现有功能选项 ID、按键与保存值保持不变；新增 HUD/伤害显示使用新 ID，动态友军/敌军列表也使用当前语言的前缀。
- 中文菜单不直接传入 UTF-8 汉字，而是生成 Hanbot 所需的 CP936/GBK 字节与 Lua 十进制转义。完整韩文目录为未来字体支持保留，但当前渲染器会把所有韩文字形替换为 `?`，因此运行时不加载。
- 已从可见菜单中删除 FXT、CXJ、CNo1 等参考实现名称；所有标签只说明用户实际控制的功能。
- 英雄下方的共享状态栏默认只在第二行显示 `Farm: ON/OFF`。其他原有状态选项仍保留，可通过 `Show other status lines` 重新开启；弹药、层数等真实资源不受此开关影响。
- 翻译与文字宽度使用缓存；每个目标的层数、伤害与剩余生命值只每 0.15–0.2 秒刷新一次，避免每帧创建字符串和重复伤害计算。
- 生成器与全量检查会阻止缺失、污染或过期翻译、跨语言混入、raw UTF-8 中文、脚本语言选择器回归，以及 234 个菜单根绕过共享包装器。当前共有 966 个 Lua 表面。
- 游戏内证据已确认 Hanbot 缺少韩文字形且 GBK 中文可正常显示；新 MESH shard 的中文客户端菜单样本仍需 F12 验证。

#### Kalista

- E 自动重置会在施放前立即重新计算：要求 Rend 标记能覆盖施法窗口，并取 Riot 公式与实时伤害中的较低值，同时计入物理/全护盾和 10 点或 2% 安全余量。按住 Combo 且英雄不在射程内时，会持续选择兵线单位、真实野怪或敌方防御塔作为攻击载体，让普攻与 Martial Poise 位移继续；植物会被排除。带标记目标上方以 0.15 秒缓存显示 `E xN | -伤害 | HP 当前 > 之后`。

#### Tristana

- E 附着目标上方现在同时显示当前层数、当前 E 单独爆炸伤害和爆炸后生命值。计算包含物理/全护盾，并且不会再用 R+E 连招伤害把 E 显示误判为红色可击杀。新的字体大小 ID 避免旧存档冲突，0.15 秒缓存避免逐帧重算。

#### LeeSin

- 修复 Q 直线预测与碰撞输入只传 `radius`，导致 `pred/linear` 或 `pred/collision` 终止的问题；现在统一使用 `width=60`。Star Combo 的 Flash 选项也改为重新加载时不会冲突的独立 ID。

#### Fiora

- Q 位移落点的直线预测补充必需的 width，避免同类 nil 预测错误。

#### Hecarim

- R 路径预测现在明确传入官方 265 宽度。

#### KSante

- Q 与蓄力 W 的直线预测输入现在都传入对应官方宽度。

#### Lillia

- 长距离滚动 E 的直线预测现在传入官方 80 宽度。

#### Milio

- Q 直线预测与碰撞检测现在共用带 width 的同一输入。

#### Renekton

- E 冲刺瞄准现在传入官方 50 宽度。

#### TwistedFate

- Q 万能牌直线预测现在传入官方 40 宽度。

#### Yone

- 修复 Q/Q3/W/R 直线预测仅传入 `radius`，导致 Hanbot `pred/linear` 因 `width` 为 nil 而终止的问题。现在明确使用 Riot 16.15 的宽度：Q 55、Q3 80、W 100、R 225，并加入专用回归契约。
<!-- MESH-AIO:RELEASE:v3.1.1:END -->

## 이전 버전 / Previous Versions / 历史版本

전체 변경 내역은 각 버전의 Release 페이지에 있습니다. Full notes live on each release page. 完整更新内容见各版本的 Release 页面。

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
