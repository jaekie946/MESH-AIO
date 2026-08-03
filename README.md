<p align="center">
  <img src="./MESH-AIO.webp" alt="MESH-AIO" width="96">
</p>

# MESH-AIO Update History

<!-- MESH-AIO:UPDATES:START -->
<!-- MESH-AIO:RELEASE:v2.0.0:START -->
## v2.0.0

### 한국어

#### 지원 챔피언

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

#### 핵심 및 메뉴

- Riot 16.15.1 Data Dragon과 패치 고정 16.15 클라이언트 원본을 기준으로 173챔피언 전체를 인식하고, 기존 6개 전용 모듈을 제외한 167챔피언에 공용 AIO를 추가했습니다.
- 현재 스킬 슬롯 이름을 공식 raw 형태 1,002개(재시전 268·변신/강화 23·충전 23·평타 리셋 75)와 매 틱 대조하고, 동일 alias는 정확한 mScriptName을 우선해 각 시전 방식으로 분기합니다.
- Elise·Jayce·Nidalee 양방향 변신, Rek'Sai 잠복, Aphelios 무기 전환, Hwei 팔레트뿐 아니라 Sylas의 훔친 궁과 Viego 빙의 슬롯도 공식 전체 카탈로그에서 현재 이름으로 찾습니다.
- 공식 타게팅 계약이 불명확한 형태는 자동 시전을 막고 세미키만 허용하며, 궁극기와 변신 자동 사용은 기본 OFF로 두었습니다.
- 공식 평타 리셋 태그가 있는 형태는 평타 선딜을 보존한 뒤 첫 유효 백스윙에서 요청하고, 거부된 유효 요청만 1ms 스크립트 하한으로 재시도합니다.
- OP.GG 16.15 공개 페이지의 173챔피언 스킬 우선순위와 사용자 팁을 robots.txt 허용 확인 후 별도 보조 캐시에 저장했으며, 수치와 시전 형태는 Riot 원본만 기준으로 사용합니다.

#### Annie

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Olaf

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Galio

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### TwistedFate

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### XinZhao

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Urgot

- 공식 형태 6개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Leblanc

- 공식 형태 10개(재시전 8·변신/강화 5·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vladimir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fiddlesticks

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kayle

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MasterYi

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Alistar

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ryze

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sion

- 공식 형태 5개(재시전 3·변신/강화 0·충전 2·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sivir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Tristana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Warwick

- 공식 형태 5개(재시전 1·변신/강화 0·충전 2·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nunu

- 공식 형태 7개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MissFortune

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ashe

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Tryndamere

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jax

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Morgana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zilean

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Singed

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Evelynn

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Twitch

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Karthus

- 공식 형태 15개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Chogath

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Amumu

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rammus

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Anivia

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shaco

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### DrMundo

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sona

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kassadin

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Irelia

- 공식 형태 8개(재시전 5·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Janna

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gangplank

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Corki

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Karma

- 공식 형태 4개(재시전 0·변신/강화 1·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Taric

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Veigar

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Trundle

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Swain

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Caitlyn

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Blitzcrank

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Katarina

- 공식 형태 8개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nocturne

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Maokai

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Renekton

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### JarvanIV

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Elise

- 공식 형태 11개(재시전 5·변신/강화 2·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Orianna

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### MonkeyKing

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Brand

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### LeeSin

- 공식 형태 7개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vayne

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rumble

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Cassiopeia

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Skarner

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Heimerdinger

- 공식 형태 9개(재시전 1·변신/강화 1·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nasus

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nidalee

- 공식 형태 7개(재시전 1·변신/강화 1·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Udyr

- 공식 형태 4개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Poppy

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gragas

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Pantheon

- 공식 형태 7개(재시전 4·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ezreal

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Mordekaiser

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yorick

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Akali

- 공식 형태 10개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kennen

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Garen

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Leona

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Malzahar

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Talon

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Riven

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### KogMaw

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shen

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lux

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Xerath

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Shyvana

- 공식 형태 6개(재시전 0·변신/강화 1·충전 0·평타 리셋 3)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ahri

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Graves

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fizz

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Volibear

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rengar

- 공식 형태 8개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Varus

- 공식 형태 4개(재시전 1·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nautilus

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Viktor

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sejuani

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Fiora

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ziggs

- 공식 형태 7개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lulu

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Draven

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Hecarim

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Khazix

- 공식 형태 10개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Darius

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jayce

- 공식 형태 8개(재시전 3·변신/강화 2·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lissandra

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Diana

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Quinn

- 공식 형태 6개(재시전 2·변신/강화 3·충전 0·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Syndra

- 공식 형태 9개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### AurelionSol

- 공식 형태 6개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kayn

- 공식 형태 6개(재시전 3·변신/강화 3·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zoe

- 공식 형태 16개(재시전 8·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zyra

- 공식 형태 6개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kaisa

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Seraphine

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gnar

- 공식 형태 7개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zac

- 공식 형태 5개(재시전 2·변신/강화 0·충전 2·평타 리셋 2)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yasuo

- 공식 형태 13개(재시전 10·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Velkoz

- 공식 형태 5개(재시전 2·변신/강화 0·충전 1·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Taliyah

- 공식 형태 9개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Camille

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Akshan

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Belveth

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Braum

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kindred

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zeri

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Jinx

- 공식 형태 4개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### TahmKench

- 공식 형태 6개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Briar

- 공식 형태 5개(재시전 0·변신/강화 0·충전 1·평타 리셋 3)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Viego

- 공식 형태 4개(재시전 0·변신/강화 0·충전 1·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Senna

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lucian

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zed

- 공식 형태 8개(재시전 6·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kled

- 공식 형태 8개(재시전 3·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ekko

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Qiyana

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vi

- 공식 형태 4개(재시전 1·변신/강화 0·충전 1·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aatrox

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nami

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Azir

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yuumi

- 공식 형태 13개(재시전 10·변신/강화 0·충전 1·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Samira

- 공식 형태 7개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Thresh

- 공식 형태 8개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Illaoi

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### RekSai

- 공식 형태 10개(재시전 3·변신/강화 3·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ivern

- 공식 형태 6개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Kalista

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 E→Q→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Bard

- 공식 형태 14개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rakan

- 공식 형태 8개(재시전 5·변신/강화 0·충전 0·평타 리셋 0)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Xayah

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ornn

- 공식 형태 7개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 W→Q→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sylas

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 3)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Neeko

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aphelios

- 공식 형태 11개(재시전 5·변신/강화 1·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Rell

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 1)와 W→E→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Vex

- 공식 형태 6개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yone

- 공식 형태 6개(재시전 4·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Ambessa

- 공식 형태 4개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Mel

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Yunara

- 공식 형태 5개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Sett

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 2)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Lillia

- 공식 형태 7개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Gwen

- 공식 형태 10개(재시전 7·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Renata

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Aurora

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Nilah

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 1)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### KSante

- 공식 형태 13개(재시전 3·변신/강화 0·충전 2·평타 리셋 1)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Smolder

- 공식 형태 4개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→W→E→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Milio

- 공식 형태 5개(재시전 2·변신/강화 0·충전 0·평타 리셋 0)와 E→W→Q→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Zaahen

- 공식 형태 6개(재시전 3·변신/강화 0·충전 0·평타 리셋 2)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Hwei

- 공식 형태 14개(재시전 0·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

#### Naafiri

- 공식 형태 5개(재시전 1·변신/강화 0·충전 0·평타 리셋 0)와 Q→E→W→R 우선순위의 공용 콤보·하레스·팜·도주·세미키 로직을 추가했습니다.

### English

#### Supported Champions

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

#### Core & Menu

- Added full 173-champion recognition from Riot Data Dragon 16.15.1 and the patch-pinned 16.15 client export, preserving the six hand-tuned modules and adding the shared AIO baseline to the other 167 champions.
- Matches each live slot name against 1,002 official raw forms (recast 268, transform/upgrade 23, charge 23, attack reset 75) every tick, preferring an exact mScriptName when aliases overlap.
- Covers both directions of Elise, Jayce, and Nidalee transformations, Rek'Sai burrow, Aphelios weapon swaps, Hwei palettes, Sylas stolen ultimates, and Viego possession slots through the full official catalog.
- Forms with an ambiguous official targeting contract stay semi-manual only, while automatic ultimates and transformations remain disabled by default.
- Official attack-reset forms preserve the auto-attack windup, cast on the first valid backswing callback, and retry only valid rejected requests with a 1 ms script-local floor.
- Archived skill priorities and user-tip summaries for all 173 champions from OP.GG 16.15 after verifying robots.txt permission; Riot data remains the sole authority for numbers and cast forms.

#### Annie

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Olaf

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Galio

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### TwistedFate

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### XinZhao

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Urgot

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Leblanc

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 8, transform/upgrade 5, charge 0, attack reset 0) and W→Q→E→R priority.

#### Vladimir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Fiddlesticks

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Kayle

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### MasterYi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Alistar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ryze

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Sion

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 3, transform/upgrade 0, charge 2, attack reset 0) and Q→W→E→R priority.

#### Sivir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Tristana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Warwick

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 2, attack reset 0) and W→Q→E→R priority.

#### Nunu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### MissFortune

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ashe

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→Q→E→R priority.

#### Tryndamere

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Jax

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Morgana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Zilean

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Singed

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Evelynn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Twitch

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Karthus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 15 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Chogath

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### Amumu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Rammus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Anivia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Shaco

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### DrMundo

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Sona

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Kassadin

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Irelia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Janna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Gangplank

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Corki

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Karma

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 1, charge 0, attack reset 0) and Q→E→W→R priority.

#### Taric

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Veigar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Trundle

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Swain

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Caitlyn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Blitzcrank

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Katarina

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Nocturne

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Maokai

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Renekton

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### JarvanIV

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Elise

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 11 official forms (recast 5, transform/upgrade 2, charge 0, attack reset 1) and Q→W→E→R priority.

#### Orianna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### MonkeyKing

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Brand

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### LeeSin

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Vayne

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Rumble

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Cassiopeia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Skarner

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Heimerdinger

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 1, transform/upgrade 1, charge 0, attack reset 0) and Q→W→E→R priority.

#### Nasus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Nidalee

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 1, transform/upgrade 1, charge 0, attack reset 1) and Q→E→W→R priority.

#### Udyr

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Poppy

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Gragas

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Pantheon

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Ezreal

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Mordekaiser

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Yorick

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Akali

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kennen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Garen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### Leona

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Malzahar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Talon

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and W→Q→E→R priority.

#### Riven

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### KogMaw

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Shen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Lux

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Xerath

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Shyvana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 1, charge 0, attack reset 3) and Q→W→E→R priority.

#### Ahri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Graves

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Fizz

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Volibear

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and W→Q→E→R priority.

#### Rengar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Varus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Nautilus

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→W→E→R priority.

#### Viktor

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Sejuani

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Fiora

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Ziggs

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Lulu

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Draven

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Hecarim

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Khazix

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Darius

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Jayce

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 2, charge 0, attack reset 1) and Q→W→E→R priority.

#### Lissandra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Diana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Quinn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 3, charge 0, attack reset 1) and Q→W→E→R priority.

#### Syndra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### AurelionSol

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Kayn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 3, charge 1, attack reset 0) and Q→W→E→R priority.

#### Zoe

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 16 official forms (recast 8, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Zyra

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Kaisa

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Seraphine

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Gnar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Zac

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 2, attack reset 2) and E→W→Q→R priority.

#### Yasuo

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 10, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Velkoz

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 1, attack reset 0) and Q→W→E→R priority.

#### Taliyah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 9 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Camille

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Akshan

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Belveth

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Braum

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kindred

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→W→E→R priority.

#### Zeri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Jinx

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### TahmKench

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Briar

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 3) and W→Q→E→R priority.

#### Viego

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 1, attack reset 1) and Q→E→W→R priority.

#### Senna

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Lucian

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Zed

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 6, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Kled

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Ekko

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Qiyana

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Vi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 1, attack reset 1) and Q→E→W→R priority.

#### Aatrox

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Nami

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Azir

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Yuumi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 10, transform/upgrade 0, charge 1, attack reset 0) and Q→E→W→R priority.

#### Samira

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Thresh

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Illaoi

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→Q→W→R priority.

#### RekSai

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 3, transform/upgrade 3, charge 0, attack reset 2) and Q→E→W→R priority.

#### Ivern

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Kalista

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and E→Q→W→R priority.

#### Bard

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 14 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Rakan

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 8 official forms (recast 5, transform/upgrade 0, charge 0, attack reset 0) and W→E→Q→R priority.

#### Xayah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and E→W→Q→R priority.

#### Ornn

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and W→Q→E→R priority.

#### Sylas

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 3) and W→E→Q→R priority.

#### Neeko

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Aphelios

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 11 official forms (recast 5, transform/upgrade 1, charge 0, attack reset 0) and Q→E→W→R priority.

#### Rell

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 1) and W→E→Q→R priority.

#### Vex

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Yone

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 4, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Ambessa

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Mel

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Yunara

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Sett

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 2) and Q→W→E→R priority.

#### Lillia

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 7 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Gwen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 10 official forms (recast 7, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### Renata

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Aurora

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Nilah

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 1) and Q→E→W→R priority.

#### KSante

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 13 official forms (recast 3, transform/upgrade 0, charge 2, attack reset 1) and Q→W→E→R priority.

#### Smolder

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 4 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→W→E→R priority.

#### Milio

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 2, transform/upgrade 0, charge 0, attack reset 0) and E→W→Q→R priority.

#### Zaahen

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 6 official forms (recast 3, transform/upgrade 0, charge 0, attack reset 2) and Q→E→W→R priority.

#### Hwei

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 14 official forms (recast 0, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

#### Naafiri

- Added the shared Combo, Harass, Farm, Flee, and Semi-key baseline with 5 official forms (recast 1, transform/upgrade 0, charge 0, attack reset 0) and Q→E→W→R priority.

### 简体中文

#### 支持英雄

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

#### 核心与菜单

- 依据 Riot Data Dragon 16.15.1 和固定版本的 16.15 客户端原始数据支持全部 173 位英雄；保留 6 个手工专用模块，并为其余 167 位英雄加入通用 AIO 基线。
- 每个 tick 将当前技能槽名称与 1,002 个官方 raw 形态（再施法 268、变身/强化 23、蓄力 23、普攻重置 75）匹配；别名重叠时优先精确 mScriptName。
- 通过完整官方目录覆盖伊莉丝、杰斯、奈德丽双向变身、雷克塞遁地、厄斐琉斯换枪、慧的画板、塞拉斯偷取终极技能和佛耶戈附身后的技能槽。
- 官方目标类型不明确的形态只允许半自动按键，自动使用终极技能和自动变身默认关闭。
- 带官方普攻重置标签的形态会保留普攻前摇，在第一个有效后摇回调施法，并仅对有效但被拒绝的请求按 1 毫秒脚本下限重试。
- 在确认 robots.txt 允许后，离线保存 OP.GG 16.15 的 173 位英雄技能优先级和用户技巧摘要；技能数值与施法形态仍只以 Riot 原始数据为准。

#### Annie

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Olaf

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Galio

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### TwistedFate

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### XinZhao

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Urgot

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Leblanc

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 10 个官方形态（再施法 8、变身/强化 5、蓄力 0、普攻重置 0）。

#### Vladimir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 0）。

#### Fiddlesticks

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kayle

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### MasterYi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Alistar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ryze

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sion

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 3、变身/强化 0、蓄力 2、普攻重置 0）。

#### Sivir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Tristana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Warwick

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 2、普攻重置 0）。

#### Nunu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### MissFortune

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ashe

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Tryndamere

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Jax

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Morgana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zilean

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Singed

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Evelynn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Twitch

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Karthus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 15 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Chogath

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Amumu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Rammus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Anivia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Shaco

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### DrMundo

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Sona

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kassadin

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Irelia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 1、普攻重置 0）。

#### Janna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gangplank

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Corki

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Karma

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 1、蓄力 0、普攻重置 0）。

#### Taric

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Veigar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Trundle

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Swain

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Caitlyn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Blitzcrank

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Katarina

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Nocturne

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Maokai

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Renekton

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### JarvanIV

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Elise

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 11 个官方形态（再施法 5、变身/强化 2、蓄力 0、普攻重置 1）。

#### Orianna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### MonkeyKing

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Brand

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### LeeSin

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Vayne

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Rumble

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Cassiopeia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Skarner

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### Heimerdinger

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 9 个官方形态（再施法 1、变身/强化 1、蓄力 0、普攻重置 0）。

#### Nasus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Nidalee

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 1、变身/强化 1、蓄力 0、普攻重置 1）。

#### Udyr

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Poppy

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 0）。

#### Gragas

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Pantheon

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 1、普攻重置 0）。

#### Ezreal

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Mordekaiser

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yorick

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Akali

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kennen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Garen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Leona

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Malzahar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Talon

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Riven

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 1）。

#### KogMaw

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Shen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lux

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Xerath

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Shyvana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 0、变身/强化 1、蓄力 0、普攻重置 3）。

#### Ahri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Graves

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Fizz

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 1）。

#### Volibear

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Rengar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Varus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 1、普攻重置 0）。

#### Nautilus

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Viktor

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sejuani

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Fiora

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Ziggs

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lulu

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Draven

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Hecarim

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Khazix

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 10 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Darius

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Jayce

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 3、变身/强化 2、蓄力 0、普攻重置 1）。

#### Lissandra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Diana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Quinn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 2、变身/强化 3、蓄力 0、普攻重置 1）。

#### Syndra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 9 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### AurelionSol

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Kayn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 3、变身/强化 3、蓄力 1、普攻重置 0）。

#### Zoe

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 16 个官方形态（再施法 8、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zyra

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kaisa

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Seraphine

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gnar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zac

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 2、普攻重置 2）。

#### Yasuo

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 13 个官方形态（再施法 10、变身/强化 0、蓄力 0、普攻重置 0）。

#### Velkoz

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 1、普攻重置 0）。

#### Taliyah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 9 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Camille

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 2）。

#### Akshan

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Belveth

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Braum

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kindred

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Zeri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Jinx

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### TahmKench

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Briar

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 3）。

#### Viego

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 1、普攻重置 1）。

#### Senna

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Lucian

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Zed

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 6、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kled

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 8 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ekko

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Qiyana

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Vi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 1、普攻重置 1）。

#### Aatrox

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 1）。

#### Nami

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Azir

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yuumi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 13 个官方形态（再施法 10、变身/强化 0、蓄力 1、普攻重置 0）。

#### Samira

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 7 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Thresh

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Illaoi

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### RekSai

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 3、变身/强化 3、蓄力 0、普攻重置 2）。

#### Ivern

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 6 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Kalista

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→Q→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Bard

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 14 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Rakan

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 8 个官方形态（再施法 5、变身/强化 0、蓄力 0、普攻重置 0）。

#### Xayah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Ornn

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→Q→E→R 优先级处理 7 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Sylas

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 3）。

#### Neeko

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Aphelios

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 11 个官方形态（再施法 5、变身/强化 1、蓄力 0、普攻重置 0）。

#### Rell

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 W→E→Q→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 1）。

#### Vex

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 6 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yone

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 4、变身/强化 0、蓄力 0、普攻重置 0）。

#### Ambessa

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Mel

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Yunara

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### Sett

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 2）。

#### Lillia

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 7 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Gwen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 10 个官方形态（再施法 7、变身/强化 0、蓄力 0、普攻重置 1）。

#### Renata

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。

#### Aurora

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Nilah

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 1）。

#### KSante

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 13 个官方形态（再施法 3、变身/强化 0、蓄力 2、普攻重置 1）。

#### Smolder

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→W→E→R 优先级处理 4 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Milio

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 E→W→Q→R 优先级处理 5 个官方形态（再施法 2、变身/强化 0、蓄力 0、普攻重置 0）。

#### Zaahen

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 6 个官方形态（再施法 3、变身/强化 0、蓄力 0、普攻重置 2）。

#### Hwei

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 14 个官方形态（再施法 0、变身/强化 0、蓄力 0、普攻重置 0）。

#### Naafiri

- 新增通用连招、消耗、清线、逃跑和半自动按键逻辑，按 Q→E→W→R 优先级处理 5 个官方形态（再施法 1、变身/强化 0、蓄力 0、普攻重置 0）。
<!-- MESH-AIO:RELEASE:v2.0.0:END -->

<!-- MESH-AIO:RELEASE:v1.1.15:START -->
## v1.1.15

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 실제 평타 위빙 경로를 전수 점검해 평타 선딜은 보존하고, 선딜 종료가 확인된 첫 백스윙 콜백에서 스킬을 즉시 요청하도록 통일했습니다.
- 위빙 전용 fast-cast는 기존 90ms 공통 시전 제한만 우회하고, 서버 스킬 잠금·쿨다운·사거리·대상 안전·서버 pause는 그대로 유지합니다.
- 첫 요청이 잠금 등으로 거부되면 스크립트 내부 최소 1ms 간격으로 재시도합니다. 실제 요청 속도는 Hanbot 틱/콜백과 게임 서버 처리 주기의 제한을 받습니다.
- 새 챔피언의 평타 위빙도 같은 안전·속도 계약을 따르도록 전용 정적 검사와 CI 게이트를 추가했습니다.

#### Locke

- Combo/Harass AA→Q 위빙이 최근 다른 스킬 사용 때문에 90ms 동안 막히지 않고 첫 유효 백스윙 콜백에서 즉시 Q를 요청합니다.
- Q 요청이 일시적으로 거부될 때만 0.12초의 신선도 창 안에서 1ms 최소 간격으로 재시도하며, 옵션 OFF·도주·Evade·대상 소실 시 콜백 스트림을 즉시 닫습니다.

#### Teemo

- Combo/Harass와 정글 AA→Q→AA가 첫 유효 백스윙 콜백에서 즉시 Q를 요청하도록 변경했습니다.
- Q가 준비되지 않았거나 Farm/도주/대상 조건이 끝나면 재호출 스트림을 즉시 종료해 늦은 백스윙에서 Q가 낭비되는 상황을 막았습니다.

#### Malphite

- 실제 평타 리셋인 AA→W→AA가 백스윙 첫 콜백에서 즉시 W를 요청하고, 성공 직후 `orb.core.reset()`을 실행하도록 가속했습니다.
- E는 기존 계약대로 평타 위빙·캔슬·리셋에 포함하지 않았으며, W가 불가능한 상황에서는 after-attack 스트림을 즉시 닫습니다.

#### Pyke

- 기본 Q→평타→E 콤보의 E를 첫 유효 백스윙 콜백에서 즉시 요청하도록 가속했습니다.
- Q 대상·Combo 상태·E 준비·타워 안전 조건이 무효가 되면 재호출을 즉시 종료하고, 유효한 거부만 1ms 최소 간격으로 재시도합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Audited every real auto-attack weave path and standardized it to preserve the attack windup, then request the spell on the first callback that confirms the backswing has begun.
- The weave-only fast-cast path bypasses only the former 90 ms generic cast throttle; server spell lock, cooldown, range, target safety, and server pause remain enforced.
- A rejected first request is retried with a 1 ms script-local minimum interval. Actual issue speed remains bounded by Hanbot's tick/callback rate and the game server.
- Added a dedicated static contract test and CI gate so future champion weaves must keep the same speed and safety rules.

#### Locke

- Combo/Harass AA-to-Q weaving no longer waits behind the 90 ms generic throttle after another recent spell and requests Q on the first valid backswing callback.
- Only temporarily rejected Q requests retry inside the 0.12-second freshness window with a 1 ms floor; disabled weaving, escape/Evade modes, or a lost target close the callback stream immediately.

#### Teemo

- Combo/Harass and jungle AA-to-Q-to-AA now request Q on the first valid backswing callback.
- The re-invoke stream closes immediately when Q, Farm, escape, or target conditions are unavailable, preventing a late Q from being wasted near the end of recovery.

#### Malphite

- The real AA-to-W-to-AA reset now requests W on the first backswing callback and calls `orb.core.reset()` immediately after a successful cast.
- E remains excluded from weaving, animation-cancel, and reset logic, while an unusable W now closes the after-attack stream immediately.

#### Pyke

- Accelerated the E in the normal charged-Q-to-AA-to-E combo so it is requested on the first valid backswing callback.
- Invalid Q target, Combo state, E readiness, or turret safety closes the stream immediately; only valid transient rejections retry with the 1 ms local floor.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 全面检查了所有真正的普攻穿插路径：保留普攻前摇，并在确认进入后摇的第一个回调中立即请求技能。
- 穿插专用 fast-cast 只绕过原有 90 毫秒通用施法限制，服务器技能锁、冷却、距离、目标安全和服务器 pause 仍然保留。
- 首次请求被拒绝时，脚本内部以最低 1 毫秒间隔重试；实际请求速度仍受 Hanbot tick/回调频率和游戏服务器限制。
- 新增专用静态契约检查和 CI 门禁，今后新增英雄的普攻穿插也必须遵守相同的速度与安全规则。

#### Locke

- 连招/消耗的普攻接 Q 不再因近期其他技能触发的 90 毫秒通用限制而等待，会在第一个有效后摇回调中立即请求 Q。
- 只有暂时被拒绝的 Q 才会在 0.12 秒新鲜度窗口内以最低 1 毫秒间隔重试；关闭穿插、逃跑/Evade 或目标丢失时会立即关闭回调流。

#### Teemo

- 连招/消耗和打野的普攻→Q→普攻现在都会在第一个有效后摇回调中立即请求 Q。
- 当 Q、Farm、逃跑或目标条件不成立时立即结束重复回调，防止 Q 在后摇末段过晚释放。

#### Malphite

- 真正的普攻→W→普攻重置现在会在第一个后摇回调中立即请求 W，并在施法成功后立刻执行 `orb.core.reset()`。
- E 依旧不属于普攻穿插、动画取消或普攻重置；W 无法使用时会立即关闭 after-attack 回调流。

#### Pyke

- 加速了标准蓄力 Q→普攻→E 连招中的 E，使其在第一个有效后摇回调中立即请求。
- Q 目标、连招状态、E 准备状态或防御塔安全条件失效时立即停止回调；只有有效的临时拒绝才按最低 1 毫秒间隔重试。
<!-- MESH-AIO:RELEASE:v1.1.15:END -->

<!-- MESH-AIO:RELEASE:v1.1.14:START -->
## v1.1.14

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 진 W 자동 사용 조건을 CC 우선과 표식 폴백으로 분리하고, 실제 유효 사거리 안전 여유를 세부 조절할 수 있게 했습니다.
- W 드로우가 메뉴 최대치가 아닌 안전 여유를 반영한 실제 자동 시전 범위를 표시하도록 동기화했습니다.

#### Jhin

- 자동 W는 투사체 도착까지 유지되는 하드 CC 대상을 먼저 전수 검사합니다. 시전 가능한 CC 대상이 없을 때만 진 표식(`jhinespotteddebuff`)이 있는 적에게 즉시 폴백합니다.
- 기존 안전 계약을 유지해 자동·Combo·Harass·Killsteal W는 평타 사거리 안에서 사용하지 않으며, Semi W만 해당 제한을 우회합니다.
- 공식 3000 사거리 끝에서 발생하는 실패를 줄이도록 25~200유닛, 기본 75유닛의 `Edge safety buffer` 옵션을 추가했습니다.
- 최근 0.5초 안에 경로를 바꾸고 예측 이동량이 120유닛 이하인 잔무빙 대상은 과하게 앞을 예측하지 않고 현재 위치 정중앙에 W를 조준합니다. 돌진이나 확실한 장거리 이동에는 기존 선형 예측을 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Split Jhin's automatic W policy into hard-CC priority and a mark fallback, with a configurable effective-range safety margin.
- Synchronized the W drawing with the real automatic cast range after applying the edge buffer.

#### Jhin

- Automatic W first scans every target for hard CC that lasts through impact. It falls back immediately to an enemy carrying Jhin's mark (`jhinespotteddebuff`) only when no connectable CC target exists.
- Preserved the established safety rule: automatic, Combo, Harass, and Killsteal W remain blocked inside auto-attack range, while directly held Semi W may bypass it.
- Added an `Edge safety buffer` of 25-200 units, default 75, to prevent failures at the edge of the official 3000 range.
- A target that changed path within the last 0.5 seconds with no more than 120 units of predicted lead is aimed at its current center, preventing over-leading against short jitter movement. Dashes and committed long movement retain linear prediction.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 将烬的自动 W 逻辑拆分为硬控优先和标记后备，并加入可调节的实际施法距离安全边距。
- W 范围绘制现在会扣除边缘安全值，与自动施法的真实有效范围保持一致。

#### Jhin

- 自动 W 会先检查所有目标，优先选择硬控持续时间足以覆盖命中时刻的敌人。只有没有可命中的硬控目标时，才会立即改为攻击带有烬标记（`jhinespotteddebuff`）的敌人。
- 保留既有安全规则：自动、连招、消耗和斩杀 W 在普攻范围内仍被禁止，只有按住 Semi W 时可以绕过该限制。
- 新增 25~200 单位、默认 75 单位的 `Edge safety buffer`，减少在官方 3000 最大距离边缘施放失败的情况。
- 若目标在最近 0.5 秒内改变路径，且预测提前量不超过 120 单位，则 W 会瞄准目标当前位置中心，避免对小幅来回移动过度预判；冲刺和明确的长距离移动仍使用线性预测。
<!-- MESH-AIO:RELEASE:v1.1.14:END -->

<!-- MESH-AIO:RELEASE:v1.1.13:START -->
## v1.1.13

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 핵심 및 메뉴

- 신규 지원 챔피언 Pyke를 추가하고 실제 스킬 아이콘이 있는 세부 메뉴를 구성했습니다.
- 공식 Riot 16.15.1/16.15 Pyke 수치 21개와 챔피언 레벨별 처형 breakpoint를 자동 회귀 검사에 연결했습니다.

#### Pyke

- 기본 Combo를 차징 Q → 평타 → E로 구현했습니다. Harass는 차징 Q만 사용하고, 짧은 Q는 공식 400 사거리 안에서 Q 한 발로 처치 가능한 경우에만 사용합니다.
- W 접근 → E → Q 기습 콤보와 커서 방향으로 빠진 뒤 Q로 당기는 Delivery E → Q 전용 키를 추가했습니다.
- Q-Flash 키는 현재 차징 사거리와 점멸 400을 함께 계산하고, 직접 Q가 맞으면 점멸을 낭비하지 않습니다. 점멸 후 위치에서 예측·충돌을 다시 계산해 Q를 해제합니다.
- E-Flash 키는 공식 1초 그림자 회수 직전 기본 50ms에만 점멸합니다. 기존 E 선에는 안 맞고 원점→점멸 착지 선에는 맞는 대상만 선택하며 포탑 안전 옵션을 적용합니다.
- Flee는 E와 W가 모두 준비됐을 때 반드시 E를 먼저 사용한 뒤 W를 사용합니다.
- R은 공식 챔피언 레벨 처형 기준과 0.8 추가 공격력·1.5 물리 관통력 계수를 사용합니다. 보호 버프가 없는 처형 대상만 예측하며, Q 차징 중에도 Q를 중단하고 R을 매 틱 최우선 시도합니다.
- Farm MMB의 Q 막타·선택적 라인 클리어·정글 클리어와 실시간 Q 차징/E/R 범위, 처형 표시, Q+E 체력바 피해 표시를 추가했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### Core & Menu

- Added Pyke as a newly supported champion with detailed collapsible menus and live spell icons.
- Connected 21 official Riot 16.15.1/16.15 Pyke values and his champion-level execute breakpoints to the automatic regression gate.

#### Pyke

- Implemented the standard charged Q → auto attack → E Combo. Harass uses charged Q only, while tap Q is reserved for a target killable by one Q inside the official 400 range.
- Added the W approach → E → Q ambush and a dedicated Delivery E → Q key that dashes toward the cursor before pulling the stored target.
- Q-Flash combines live charge range with the 400 Flash range, avoids wasting Flash when Q already connects, then recalculates prediction and collision from the post-Flash position before release.
- E-Flash casts only during the final 50 ms by default before the official one-second shadow return. It requires a target missed by the original E line but crossed by the origin-to-Flash segment and respects turret safety.
- Flee always uses E first and W second when both abilities are ready.
- R uses the official champion-level execute base plus 0.8 bonus AD and 1.5 lethality. It skips protected targets and interrupts a charged Q to retry an executable R target every pre-tick.
- Added Farm MMB tap-Q last hit, optional lane clear and jungle clear, plus live Q-charge/E/R ranges, execute markers, and Q+E health-bar damage.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin
- Pyke

#### 核心与菜单

- 新增派克支持，并加入带实时技能图标的详细折叠菜单。
- 将 Riot 16.15.1/16.15 的 21 项派克官方数据及按英雄等级变化的斩杀 breakpoint 接入自动回归检查。

#### Pyke

- 实现标准蓄力 Q → 普攻 → E 连招。消耗模式仅使用蓄力 Q；短 Q 只会在官方 400 范围内且一发 Q 能击杀目标时使用。
- 新增 W 接近 → E → Q 突袭连招，以及向鼠标方向位移后拉回已记录目标的 Delivery E → Q 专用按键。
- Q-Flash 会同时计算实时蓄力距离与 400 闪现距离；Q 本身能够命中时不会浪费闪现，并在闪现后位置重新进行预测与碰撞检测再释放 Q。
- E-Flash 默认只在官方一秒影子返回前最后 50 毫秒使用。目标必须不会被原 E 线命中、但会被起点到闪现落点的线段命中，并遵守防御塔安全设置。
- 当 E 与 W 都可用时，逃跑模式始终先使用 E，再使用 W。
- R 使用官方按英雄等级计算的斩杀基础值，以及 0.8 额外攻击力和 1.5 穿甲系数。它会跳过受保护目标，并在 Q 蓄力期间中断 Q，每个 pre-tick 优先重试可斩杀目标。
- 新增 Farm MMB 的短 Q 补刀、可选清线与打野，并加入实时 Q 蓄力/E/R 范围、斩杀标记和 Q+E 血条伤害显示。
<!-- MESH-AIO:RELEASE:v1.1.13:END -->

<!-- MESH-AIO:RELEASE:v1.1.11:START -->
## v1.1.11

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 궁극기 조준과 치명타 재시도 안전 조건을 함께 개선했습니다.

#### Jhin

- R 채널 중 일반 한 발 피해로 처치 가능한 적을 먼저 찾습니다. 선형 예측과 챔피언·벽 충돌 계산을 통과해 실제로 맞힐 수 있을 때만 키 입력 없이 자동 발사하며 공식 1초 로컬 간격도 유지합니다.
- 처치 대상이 없으면 Semi R 또는 Combo 키를 누르는 동안에만 발사하며, 충돌 없이 맞힐 수 있는 적 중 마우스에 가장 가까운 대상을 선택합니다. 처치 가능 적이 있으면 수동 대상보다 항상 우선합니다.
- R 채널 최초 시작은 기존처럼 Semi R로만 수행하며 시작 방향도 마우스에 가장 가까운 적을 기준으로 합니다. 기존 전체 자동 조준 옵션은 `Auto-fire R on one-shot kill` 옵션으로 교체했습니다.
- 치명타 재시도 간격은 메뉴 설정 없이 1ms로 고정했습니다. `Anti-stuck timeout`은 100~500ms만 설정할 수 있고 기본값은 100ms이며, 제한에 도달하면 진행 중인 취소·재공격 상태도 즉시 종료합니다.
- 치명타 재시도 활성 기준을 30~100%로 확장하고 기본값을 30%로 낮췄습니다. 이전 저장값과 충돌하지 않도록 새 설정 키를 사용합니다.
- 일반 평타 한 발의 온힛 포함 실제 피해로 현재 체력과 공용·물리 보호막을 모두 제거할 수 있으면 치명타 재시도를 건너뛰고 그 평타로 바로 처치합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Improved both Jhin's Curtain Call targeting and critical-retry safety rules.

#### Jhin

- While Curtain Call is active, the script first searches for an enemy killable by one conservative regular shot. It auto-fires without a key only when linear prediction plus champion/wall collision confirms the shot can connect, while preserving the conservative local one-second gate.
- Without a killable target, shots fire only while Semi R or Combo is held and select the collision-free hittable enemy closest to the mouse. A killable target always takes priority over the manual target.
- Curtain Call still starts only from Semi R, now aimed toward the enemy closest to the mouse. The former full auto-aim option was replaced by `Auto-fire R on one-shot kill`.
- The critical-retry pulse is now fixed at 1 ms with no menu setting. `Anti-stuck timeout` is limited to 100-500 ms and defaults to 100 ms; reaching it immediately clears any active cancel/retry state.
- The critical-retry activation threshold now ranges from 30% to 100% and defaults to 30%. A new setting key prevents an older saved threshold from overriding it.
- If one ordinary auto attack's actual damage, including on-hit effects, can remove the target's current health and all/physical shields, that attack is allowed to land instead of being cancelled for a critical retry.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 同时改进烬的大招瞄准与暴击重试安全规则。

#### Jhin

- 大招引导期间，脚本会优先寻找能被一发保守普通大招子弹击杀的敌人。只有线性预测以及英雄、墙体碰撞检测确认能够命中时，才会无需按键自动发射，并保留保守的本地一秒间隔。
- 没有可击杀目标时，仅在按住 Semi R 或 Combo 键期间发射，并选择鼠标附近能够无碰撞命中的最近敌人。可击杀目标始终优先于手动目标。
- 大招仍然只能通过 Semi R 开始，现在会朝鼠标附近最近的敌人开启。原来的完整自动瞄准选项已替换为 `Auto-fire R on one-shot kill`。
- 暴击重试 pulse 现在固定为 1 毫秒，不再提供菜单设置。`Anti-stuck timeout` 只能设置为 100~500 毫秒，默认 100 毫秒；达到限制时会立即清除正在进行的取消与重试状态。
- 暴击重试启用阈值现已扩展为 30%~100%，默认值降至 30%。使用新的设置键，避免旧保存值覆盖新默认值。
- 如果一次普通攻击包含攻击特效后的实际伤害足以清空目标当前生命值以及通用、物理护盾，则不会为了暴击重试而取消这次攻击，而是直接完成击杀。
<!-- MESH-AIO:RELEASE:v1.1.11:END -->

<!-- MESH-AIO:RELEASE:v1.1.10:START -->
## v1.1.10

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 재시도 기본 간격을 1ms로 낮추고 고착 기본 시간을 300ms로 단축했습니다.

#### Jhin

- `Retry pulse` 기본값을 5ms에서 1ms로 낮췄습니다. 범위는 1~50ms를 유지하며 실제 속도는 게임 pre-tick 해상도 안에서 가장 빠르게 동작합니다.
- `Anti-stuck timeout` 최소값을 500ms에서 100ms로 낮추고 기본값을 3000ms에서 300ms로 변경했습니다. 현재 pending/confirmed 상태까지 즉시 종료하는 전체 hard limit라 100ms 설정이 실제로 120ms까지 늘어나지 않습니다.
- 기존 저장된 5ms/3000ms 값이 새 기본값을 덮지 않도록 두 슬라이더 모두 새 설정 키로 분리했습니다. 치명타 기준 최소·기본 60%와 Crit/보장 4타 보호는 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Reduced Jhin's default retry pulse to 1 ms and shortened the default anti-stuck duration to 300 ms.

#### Jhin

- Reduced the `Retry pulse` default from 5 ms to 1 ms. Its 1-50 ms range remains, with effective speed bounded only by the game's pre-tick resolution.
- Reduced the `Anti-stuck timeout` minimum from 500 ms to 100 ms and its default from 3000 ms to 300 ms. It is a hard whole-chain deadline that immediately clears pending/confirmed state, so a 100 ms setting cannot stretch to the separate 120 ms cancellation timeout.
- Both sliders use new setting keys so saved 5 ms/3000 ms values cannot override the new defaults. The 60% minimum/default threshold and random-crit/fourth-shot protection remain unchanged.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的默认重试 pulse 降至 1 毫秒，并将默认防卡死时间缩短至 300 毫秒。

#### Jhin

- 将 `Retry pulse` 默认值从 5 毫秒降至 1 毫秒，范围仍为 1~50 毫秒，实际速度仅受游戏 pre-tick 精度限制。
- 将 `Anti-stuck timeout` 最低值从 500 毫秒降至 100 毫秒，默认值从 3000 毫秒改为 300 毫秒。它是整个链的硬性截止时间，会立即清除 pending/confirmed 状态，因此 100 毫秒设置不会被单次取消的 120 毫秒超时延长。
- 两个滑块都改用新的设置键，防止旧的 5 毫秒/3000 毫秒保存值覆盖新默认值。最低/默认 60% 暴击阈值以及随机暴击、第四发保护保持不变。
<!-- MESH-AIO:RELEASE:v1.1.10:END -->

<!-- MESH-AIO:RELEASE:v1.1.9:START -->
## v1.1.9

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 재시도 속도·고착 시간을 메뉴에서 직접 조절할 수 있게 하고 기본 속도를 5ms로 높였습니다.

#### Jhin

- 치명타 활성 기준을 최소·기본 60%로 변경했습니다. 기존 저장값과 충돌하지 않도록 새 설정 키를 사용합니다.
- `Retry pulse` 슬라이더를 추가했습니다. 1~50ms 범위에서 실시간 조절할 수 있으며 기본값은 5ms입니다. 취소 확인 뒤 설정한 pulse가 만료되는 첫 pre-tick에 즉시 재공격합니다.
- `Anti-stuck timeout` 슬라이더를 추가했습니다. 500~10000ms 범위, 기본 3000ms이며 고정 횟수 제한 없이 이 시간 안에서 성공할 때까지 반복합니다. Crit과 보장 4타는 계속 즉시 통과합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Added user controls for Jhin's retry speed and anti-stuck duration, with a faster 5 ms default pulse.

#### Jhin

- Changed the critical activation threshold to a 60% minimum and default. A new setting key avoids conflicts with previously saved values.
- Added a `Retry pulse` slider, adjustable live from 1 to 50 ms and defaulting to 5 ms. The reattack is issued on the first pre-tick after the configured pulse expires.
- Added an `Anti-stuck timeout` slider from 500 to 10000 ms, defaulting to 3000 ms. With no fixed attempt cap, retries continue until success within this duration. Random crits and the guaranteed fourth shot still pass immediately.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 添加烬的重试速度与防卡死时间自定义设置，并将默认 pulse 提升为 5 毫秒。

#### Jhin

- 将暴击启用阈值的最低值和默认值改为 60%。使用新的设置键，避免与旧保存值冲突。
- 新增 `Retry pulse` 滑块，可在 1~50 毫秒之间实时调整，默认 5 毫秒。配置的 pulse 到期后的第一个 pre-tick 会立即重新攻击。
- 新增 `Anti-stuck timeout` 滑块，范围 500~10000 毫秒，默认 3000 毫秒。没有固定次数上限，会在该时间内持续重试直到成功。随机暴击和必定暴击第四发仍会立即放行。
<!-- MESH-AIO:RELEASE:v1.1.9:END -->

<!-- MESH-AIO:RELEASE:v1.1.8:START -->
## v1.1.8

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반탄 취소 후 재공격 대기 시간을 대폭 줄이고 고정 12회 제한을 제거했습니다.

#### Jhin

- 인게임에서 이동 취소가 정상 작동하는 것을 확인한 뒤, 취소 확인과 재공격을 기다리던 최소 시간을 80ms에서 10ms로 줄였습니다. 실제로는 다음 pre-tick에서 바로 같은 대상을 다시 공격합니다.
- 공격 잠금 pulse도 80/50ms에서 10ms로 줄이고 취소 실패 제한을 200ms에서 120ms로 단축해 실패 상태에서도 오래 멈추지 않습니다.
- 고정 12회 재시도 제한을 제거했습니다. 이제 성공할 때까지 빠르게 반복하며, 비정상 고착만 막는 대상별 전체 3초 제한을 유지합니다. Crit과 보장 4타는 계속 즉시 통과합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Greatly reduced Jhin's post-cancel reattack delay and removed the fixed 12-attempt limit.

#### Jhin

- After in-game confirmation that movement cancellation works, the minimum cancellation-to-reattack wait was reduced from 80 ms to 10 ms. The same target is now reattacked on the next available pre-tick.
- The attack-lock pulse was reduced from 80/50 ms to 10 ms, and the failed-cancellation timeout from 200 ms to 120 ms, preventing unnecessary stalls even on failure.
- Removed the fixed 12-attempt retry cap. Retries now continue rapidly until success, with only a three-second per-target anti-stuck timeout. Random crits and the guaranteed fourth shot still pass immediately.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 大幅缩短烬取消普通子弹后的重新攻击延迟，并移除固定 12 次限制。

#### Jhin

- 在游戏内确认移动取消正常工作后，将取消到重新攻击的最短等待时间从 80 毫秒缩短到 10 毫秒。现在会在下一个可用 pre-tick 立即重新攻击同一目标。
- 攻击锁定 pulse 从 80/50 毫秒缩短到 10 毫秒，取消失败超时从 200 毫秒缩短到 120 毫秒，即使失败也不会长时间停顿。
- 移除固定 12 次重试上限。现在会高速重试直到成功，仅保留每个目标 3 秒的防卡死总超时。随机暴击和必定暴击第四发仍会立即放行。
<!-- MESH-AIO:RELEASE:v1.1.8:END -->

<!-- MESH-AIO:RELEASE:v1.1.7:START -->
## v1.1.7

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반탄 감지는 정상이나 정지 명령이 windup을 끊지 못하던 런타임 문제를 실제 이동 취소 경로로 교체했습니다.

#### Jhin

- 새 F12 로그에서 일반탄 감지와 임계값 통과는 정상이나, `player:stop()` 이후 `attack_cancel` 없이 매번 0.2초 timeout이 발생하는 것을 확인했습니다. 메뉴 옵션 문제가 아니라 Hanbot Stop 명령이 진의 평타 windup을 끊지 못한 것이 원인이었습니다.
- 일반탄의 실제 `cb.spell` 시점부터 공격만 짧게 막고 마우스 방향 이동 명령을 반복해 windup을 취소합니다. 취소 확인 후 공격 pause가 자연 만료되면 같은 대상을 다시 공격합니다.
- 비평타 주문에서 남아 있던 이전 `cur_attack_name` 때문에 Q가 4타로 기록되던 진단 오분류도 수정했습니다. 이제 실제 기본 공격 이벤트에서만 보조 이름을 사용하며 Crit과 보장 4타 보호는 유지합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ineffective windup Stop path with real movement cancellation after confirming that ordinary-round detection itself was correct.

#### Jhin

- New F12 logs confirmed that ordinary-round detection and the threshold gate worked, but every `player:stop()` reached the 200 ms timeout without `attack_cancel`. The menu setup was correct; Hanbot's Stop command did not cancel Jhin's attack windup.
- Starting at the real ordinary-attack `cb.spell`, the script now briefly pauses attacks and repeatedly issues a movement order toward the mouse to cancel the windup. It reattacks the same target only after cancellation is confirmed and the attack pause expires naturally.
- Fixed stale `cur_attack_name` making Q appear as a fourth shot in diagnostics. The auxiliary orb attack name is now trusted only on a real basic-attack event, while random crit and guaranteed fourth-shot protection remains intact.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 在确认普通子弹识别正常后，将无法中断前摇的 Stop 流程改为真实移动取消流程。

#### Jhin

- 新的 F12 日志确认普通子弹识别和阈值判断都正常，但每次 `player:stop()` 都没有触发 `attack_cancel`，并在 200 毫秒后超时。菜单设置没有问题，原因是 Hanbot 的 Stop 命令无法中断烬的攻击前摇。
- 从真实普通攻击的 `cb.spell` 开始，现在会短暂暂停攻击并持续向鼠标方向发送移动命令来取消前摇。只有确认取消且攻击暂停自然结束后，才会重新攻击同一个目标。
- 修复旧的 `cur_attack_name` 导致 Q 在诊断中被误记为第四发的问题。现在仅在真实基本攻击事件中使用该辅助名称，同时继续保护随机暴击和必定暴击第四发。
<!-- MESH-AIO:RELEASE:v1.1.7:END -->

<!-- MESH-AIO:RELEASE:v1.1.6:START -->
## v1.1.6

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반 평타 취소 감지를 애니메이션 이벤트에서 실제 공격 시작 이벤트로 교체했습니다.

#### Jhin

- F12 로그에서 일반 평타의 `Attack1/2/3` 애니메이션 이벤트가 한 번도 오지 않고 `Reload_Recoil`만 들어오는 것을 확인했습니다. 애니메이션 콜백은 이제 진단 로그만 남기며 취소 상태를 변경하지 않습니다.
- 자기 `cb.spell`의 공식 공격 이름으로 일반탄을 감지해 80ms 전체 정지와 `player:stop()`을 즉시 발행합니다. 실제 `spell.target`만 저장하며, 대상이 없는 이벤트는 안전하게 무시합니다.
- `JhinCritAttack`, `JhinPassiveAttack`, `JhinBasicAttack4`, 현재 4타 버프와 오브워커 공격 이름을 함께 확인해 확률 치명타와 보장 4타는 절대 중단하지 않습니다. 80ms 재공격보다 길었던 120ms 제한도 제거해 성공 또는 안전 제한까지 연속 재시도할 수 있습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ordinary-attack cancellation trigger from animation events to the real attack-start event.

#### Jhin

- F12 logs confirmed that ordinary attacks never emitted `Attack1/2/3` animation events and only emitted `Reload_Recoil`. Animation callbacks are now diagnostic-only and cannot mutate retry state.
- Ordinary rounds are detected from Jhin's official attack names in his own `cb.spell`; the script immediately applies an 80 ms full pause and `player:stop()`. Only the exact `spell.target` is retained, and targetless events fail safely.
- `JhinCritAttack`, `JhinPassiveAttack`, `JhinBasicAttack4`, the live fourth-shot buff, and the orbwalker attack name jointly protect random crits and the guaranteed fourth shot. The obsolete 120 ms gate that blocked the 80 ms retry chain was removed so retries can continue until success or a safety cap.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的普通攻击取消触发方式从动画事件改为真实的攻击开始事件。

#### Jhin

- F12 日志确认普通攻击从未触发 `Attack1/2/3` 动画事件，只出现了 `Reload_Recoil`。动画回调现在仅用于诊断日志，不再修改重试状态。
- 现在通过烬自身 `cb.spell` 中的官方攻击名称识别普通子弹，并立即执行 80 毫秒整体暂停与 `player:stop()`。只保存准确的 `spell.target`，没有目标的事件会安全忽略。
- 同时检查 `JhinCritAttack`、`JhinPassiveAttack`、`JhinBasicAttack4`、当前第四发增益和走砍攻击名称，确保随机暴击及必定暴击第四发绝不被中断。已移除会阻断 80 毫秒重试链的旧 120 毫秒限制，使其能够持续重试直到成功或触发安全上限。
<!-- MESH-AIO:RELEASE:v1.1.6:END -->

<!-- MESH-AIO:RELEASE:v1.1.5:START -->
## v1.1.5

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 일반 평타 취소 방식을 실제 전체 행동 정지 명령으로 교체했습니다.

#### Jhin

- 이동 명령으로는 일반 Attack1~3 평타가 취소되지 않던 문제를 수정했습니다. 이제 전체 오브워커를 잠깐 정지하고 `player:stop()`을 발행해 현재 행동을 직접 중단합니다.
- 진 본인의 `attack_cancel` 또는 Stop 원점 80ms 뒤 windup 종료로 취소를 확인합니다. 유한 전체 정지가 자연 만료되면 reset 후 같은 유효 대상을 재공격하며, 중간 사용자 주문·200ms Stop 실패·사망·R 채널에서는 재공격하지 않습니다. Crit과 보장 4타 Attack4는 그대로 공격합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Replaced Jhin's ordinary-attack cancellation with the actual full action-stop command path.

#### Jhin

- Fixed ordinary Attack1-3 attacks not cancelling when only a movement order was used. The script now briefly pauses the full orbwalker and issues `player:stop()` to stop the current action directly.
- Cancellation is confirmed by Jhin's own `attack_cancel` or a stopped windup 80 ms from the original Stop. Once the finite full pause expires naturally, it resets and reattacks the same valid target; a manual user order, 200 ms stop failure, death, or Curtain Call discards the retry. `Crit` and guaranteed fourth-shot `Attack4` continue normally.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的普通攻击取消方式改为实际的“停止所有行动”命令流程。

#### Jhin

- 修复仅使用移动命令时无法取消普通 Attack1-3 攻击的问题。现在会短暂暂停整个走砍系统，并发送 `player:stop()` 直接停止当前行动。
- 通过烬自身的 `attack_cancel`，或从原始 Stop 起 80 毫秒后攻击前摇已经结束来确认取消。有限的整体暂停自然结束后，脚本会重置走砍并重新攻击同一个有效目标；若期间出现玩家手动命令、200 毫秒内 Stop 失败、角色死亡或开启大招，则放弃重试。`Crit` 与必定暴击的第四发 `Attack4` 会正常放行。
<!-- MESH-AIO:RELEASE:v1.1.5:END -->

<!-- MESH-AIO:RELEASE:v1.1.4:START -->
## v1.1.4

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 치명타 애니메이션 취소 후 재공격이 빠졌던 문제를 긴급 수정했습니다.

#### Jhin

- 일반 Attack1~3 모션을 취소한 뒤 다음 공격을 발행하지 않아 재시도가 멈추던 문제를 수정했습니다. 실제 `attack_cancel` 확인 50ms 뒤 첫 안전한 틱에서 오브워커를 초기화하고 같은 유효 대상을 재공격합니다.
- 진 본인의 취소 이벤트만 허용하고 대상별 한 체인을 최대 12회·1.5초로 제한하며, 한도 이후에는 초기화 조건까지 일반 공격을 허용합니다. Crit과 보장 4타 Attack4는 계속 보존합니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Hotfixed Jhin's missing reattack after a critical-animation cancellation.

#### Jhin

- Fixed the retry stopping after cancelling an ordinary Attack1-3 animation because no replacement attack was issued. The first safe tick 50 ms after a confirmed `attack_cancel` now resets the orbwalker and reattacks the same valid target.
- Only Jhin's own cancel event is accepted. Each target-specific chain is capped at 12 attempts or 1.5 seconds, after which ordinary attacks are allowed until a reset condition. `Crit` and the guaranteed fourth-shot `Attack4` remain protected.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 紧急修复烬取消暴击动画后没有重新发起普攻的问题。

#### Jhin

- 修复取消普通 Attack1-3 动画后未发出替代攻击，导致重试停止的问题。现在会在确认 `attack_cancel` 后 50 毫秒的第一个安全 tick 重置走砍，并重新攻击同一个有效目标。
- 仅接受烬自身的取消事件。每个目标的重试链最多 12 次或 1.5 秒，达到上限后会允许普通攻击，直到满足重置条件。继续保护 `Crit` 与必定暴击的第四发 `Attack4`。
<!-- MESH-AIO:RELEASE:v1.1.4:END -->

<!-- MESH-AIO:RELEASE:v1.1.3:START -->
## v1.1.3

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 궁 재사용, 치명타 재시도, W 평타 사거리 규칙을 실제 입력 상태에 맞게 교정했습니다.

#### Jhin

- R2 슬롯이 준비되지 않은 요청 때문에 다음 탄환이 약 2초까지 늦어질 수 있던 문제를 수정했습니다. 서버 강제 공식 1초는 유지하며, Auto는 보수적 간격을 지키고 Semi R 또는 Combo 키를 누르는 동안에는 슬롯이 준비되는 첫 틱부터 성공할 때까지 빠르게 재시도합니다.
- 치명타 재시도 기본 기준을 45%로 바로잡고 새로운 저장 키를 사용합니다. 문자열과 숫자 해시 애니메이션을 모두 식별하며 F12 진단에 실제 분류와 차단 조건을 표시합니다.
- 챔피언이 평타 사거리 안에 있으면 CC 상태여도 Combo, Harass, Auto, Killsteal에서 W를 사용하지 않습니다. 평타 사거리 안 W는 사용자가 Semi W 키를 누른 경우에만 허용됩니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Corrected Jhin's Curtain Call recast, critical retry, and W attack-range rules against live input state.

#### Jhin

- Fixed non-ready R2 requests delaying the next shot by up to roughly two seconds. The server-enforced official one-second minimum remains; Auto keeps its conservative interval, while a held Semi R or Combo input retries every tick from the first ready slot until the request succeeds.
- Corrected the critical-retry default threshold to 45% with a fresh save key. Both string and numeric-hash animation events are recognized, and F12 diagnostics now show the classification and active gates.
- W is never cast by Combo, Harass, Auto, or Killsteal against a champion inside attack range, even when the target is crowd controlled. Only a directly held Semi W may bypass this rule.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 根据实时输入状态修正了烬的大招再次施放、暴击重试以及 W 普攻距离规则。

#### Jhin

- 修复 R2 尚未就绪的请求导致下一发可能延迟到约两秒的问题。保留服务器强制的一秒官方最低间隔；自动模式维持保守间隔，按住 Semi R 或连招键时则从技能槽就绪的第一帧开始逐帧重试，直到请求成功。
- 将暴击重试默认阈值修正为 45%，并使用新的保存键。现在可识别字符串与数字哈希动画事件，F12 调试会显示实际分类与拦截条件。
- 当英雄位于普攻距离内时，即使目标处于控制状态，连招、消耗、自动逻辑和斩杀也不会使用 W；只有玩家直接按住 Semi W 时才允许例外。
<!-- MESH-AIO:RELEASE:v1.1.3:END -->

<!-- MESH-AIO:RELEASE:v1.1.2:START -->
## v1.1.2

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 체력바를 가리던 상단 패시브/치명타 상태 표시와 해당 설정 메뉴를 제거했습니다.

#### Jhin

- 챔피언 위에 표시되던 `CRIT xx% | E n | R ...` 텍스트를 제거해 체력바와 겹치지 않게 했습니다.
- 챔피언 아래의 기존 세로 핫키/상태 목록은 그대로 유지됩니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Removed Jhin's upper passive/critical status display and its settings menu because it overlapped the health bar.

#### Jhin

- Removed the `CRIT xx% | E n | R ...` text previously drawn above Jhin so it no longer covers the health bar.
- Kept the existing vertical hotkey/status list below the champion unchanged.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 移除了会遮挡烬生命条的上方被动/暴击状态显示及其设置菜单。

#### Jhin

- 移除了原先显示在烬上方的 `CRIT xx% | E n | R ...` 文本，使其不再遮挡生命条。
- 保留英雄下方现有的纵向快捷键/状态列表。
<!-- MESH-AIO:RELEASE:v1.1.2:END -->

<!-- MESH-AIO:RELEASE:v1.1.1:START -->
## v1.1.1

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- 진의 직선 예측 입력을 공식 Hanbot 스키마로 교정하고 같은 필드 오류를 차단하는 회귀 계약을 추가했습니다.

#### Jhin

- W 또는 R 탄환 예측 시 `pred/collision` 내부에서 `vec2 nil` 치명 오류가 발생하던 문제를 수정했습니다.
- W와 R의 실제 투사체 폭은 유지하면서 직선 충돌 판정이 요구하는 `width` 필드를 사용하도록 변경했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Corrected Jhin's linear prediction inputs to the Hanbot schema and added regression contracts that reject the same field mismatch.

#### Jhin

- Fixed the fatal `vec2 nil` error inside `pred/collision` when predicting W or Curtain Call shots.
- Preserved the official projectile widths while supplying the required `width` field for linear collision prediction.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- 将烬的直线预测输入修正为 Hanbot 所需格式，并新增回归契约以阻止相同字段错误再次出现。

#### Jhin

- 修复 W 或大招子弹预测进入 `pred/collision` 时触发的 `vec2 nil` 致命错误。
- 保留官方弹道宽度数值，同时改用直线碰撞预测所要求的 `width` 字段。
<!-- MESH-AIO:RELEASE:v1.1.1:END -->

<!-- MESH-AIO:RELEASE:v1.1.0:START -->
## v1.1.0

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 핵심 및 메뉴

- mesh-aio에 다섯 번째 챔피언 Jhin을 추가하고, 실제 Q/W/E/R 아이콘이 표시되는 접이식 메뉴와 사용자 지정 단축키를 연결했습니다.
- Riot 16.15.1/16.15 공식 데이터로 진의 피해량·사거리·시전 시간·투사체·함정·궁 탄환 계약을 고정하고 F12 진단을 추가했습니다.

#### Jhin

- Combo와 Harass에 Q/W/E 사용, 평타 사거리 안 비활성화, W 하드 CC 조건, 자동 처치·CC·정지 대상 반응을 각각 조절할 수 있게 했습니다.
- `MMB` Farm 토글에 Q/W/E 라인·정글 옵션과 최소 적중 조건을 추가하고, Q 연쇄 대상과 W 관통 경로를 보수적으로 선택하도록 했습니다.
- Semi W와 Semi R 키를 추가했습니다. R은 자동으로 시작하지 않으며, Semi R로 커튼 콜을 연 뒤 채널 중 실제 3500 사거리 탄환만 예측 조준합니다.
- 일반 치명타 `Crit` 모션과 보장 4타 `Attack4`를 분리하는 실험적 치명타 재시도 옵션을 추가했습니다. 기본값은 꺼짐이며 활성 기준은 45~100%로 설정할 수 있고, 보장 4타와 이미 치명타인 공격은 취소하지 않습니다.
- Q/W/E/R 실시간 범위, 패시브·치명타 상태, 콤보 피해 체력바, 처치 가능 표시와 세로형 핫키 상태줄을 추가했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### Core & Menu

- Added Jhin as the fifth mesh-aio champion with collapsible menus, live Q/W/E/R icons, and rebindable hotkeys.
- Locked Jhin's damage, range, cast-time, projectile, trap, and Curtain Call shot contracts to Riot 16.15.1/16.15 data and added F12 diagnostics.

#### Jhin

- Added separate Combo and Harass controls for Q/W/E, disable-inside-AA-range rules, hard-CC-only W behavior, killsteal, and automatic CC/immobile reactions.
- Added Q/W/E lane and jungle controls under the `MMB` Farm toggle, including minimum-hit settings and conservative Q-bounce/W-line selection.
- Added rebindable Semi W and Semi R. Curtain Call never starts automatically; Semi R opens it and only the active 3500-range shots are prediction-aimed during the channel.
- Added an experimental critical retry option that distinguishes random `Crit` attacks from the guaranteed fourth-shot `Attack4`. It is off by default, supports a 45-100% activation threshold, and never cancels an already-critical or guaranteed fourth shot.
- Added live Q/W/E/R ranges, passive and critical state text, combo-damage health bars, killable indicators, and the standard vertical hotkey status list.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka
- Jhin

#### 核心与菜单

- mesh-aio 新增第五名英雄 Jhin，并加入可折叠菜单、实时 Q/W/E/R 图标与可重新绑定的快捷键。
- 根据 Riot 16.15.1/16.15 官方数据固定烬的伤害、距离、施法时间、弹道、陷阱与大招子弹规则，并加入 F12 调试信息。

#### Jhin

- 为连招与消耗分别加入 Q/W/E 控制、普攻范围内禁用、W 仅对硬控目标、斩杀以及自动控制/静止目标反应选项。
- 在 `MMB` 清线开关中加入 Q/W/E 对线与野怪选项、最低命中数，以及保守的 Q 弹跳和 W 穿透路径选择。
- 新增可改键的半自动 W 与半自动 R。脚本不会自动开启谢幕；只有按下 Semi R 开启后，才会在引导期间预测瞄准实际 3500 距离的子弹。
- 新增实验性暴击重试选项，区分随机 `Crit` 与必定暴击的第四发 `Attack4`。默认关闭，可设置 45-100% 的启用阈值，并且不会取消已经暴击或必定暴击的第四发。
- 新增 Q/W/E/R 实时范围、被动与暴击状态、连招伤害生命条、可击杀提示以及标准纵向快捷键状态列表。
<!-- MESH-AIO:RELEASE:v1.1.0:END -->

<!-- MESH-AIO:RELEASE:v1.0.2:START -->
## v1.0.2

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- 기존 메뉴 설정과 사용자 X/Y 보정값을 유지하면서 티모 화면 표시 위치를 교정했습니다.

#### Teemo

- 패시브 `STEALTH`·공격 속도·은신 대기시간 표시가 체력바에 붙던 문제를 수정해, 다시 챔피언 머리 위 전용 위치에 표시되도록 했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- Corrected Teemo's on-screen indicator position while preserving existing menu settings and user X/Y offsets.

#### Teemo

- Fixed the passive `STEALTH`, attack-speed, and stealth-countdown text appearing on the health bar; it now uses the dedicated above-champion position again.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- 在保留现有菜单设置与用户 X/Y 偏移的同时，修正了提莫屏幕提示的位置。

#### Teemo

- 修复被动 `STEALTH`、攻速与隐身倒计时文字贴在生命条上的问题，现在会重新显示在英雄头顶的专用位置。
<!-- MESH-AIO:RELEASE:v1.0.2:END -->

<!-- MESH-AIO:RELEASE:v1.0.1:START -->
## v1.0.1

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- Riot 공식 챔피언 캐시와 네 챔피언의 핵심 피해 상수·계수·사거리·시전 시간을 자동 대조하는 회귀 검사를 추가했습니다.
- 파밍과 CC 판정에 사용하는 스킬 도착 시간을 공식 castFrame과 투사체 속도 기준으로 교정했습니다.

#### Locke

- R의 다중 적중 판정과 실제 시전이 동일한 예측 착지점을 사용하도록 통합했습니다.
- R 가장자리 적은 35유닛 안전 여유 또는 충분한 하드 CC가 있을 때만 계산하며, 선택한 대상은 중앙 단일 조준을 유지합니다.

#### Teemo

- Q 파밍 체력 예측에 공식 0.493초 시전시간과 투사체 이동시간을 반영했습니다.
- Semi R은 기본적으로 챔피언에게만 사용하며, 챔피언이 없을 때 정글 몬스터에 사용하는 동작을 별도 기본 OFF 옵션으로 분리했습니다.
- 샤드를 다시 불러온 뒤에도 실제 아군 버섯을 검사해 기존 버섯 주변에 중복 설치하지 않도록 수정했습니다.

#### Malphite

- 현재 방관 규칙에 맞게 구형 레벨 비례 물리 관통 계산을 제거해 W 피해 예측을 교정했습니다.
- 자동 R과 Semi Multi R의 최소 적중값을 2명으로 고정하고, R 착지시간·하드 CC·이동 여유·선택 타겟 중앙 조준을 반영했습니다.
- Tower Combat 토글을 두 Semi R 경로에도 적용하고 Q 파밍 예측 시간을 공식 0.333초로 교정했습니다.

#### Soraka

- Q-only 자동 Combo/Harass 계약에 맞게 킬 가능 원과 체력바 예상 피해를 Q 단독 피해로 수정했습니다.
- Q 시전시간을 공식 0.283초로 교정하고, 거리별 투사체 이동시간을 하드 CC·예측·스테이시스 판정에 반영했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- Added an automated regression check that compares the four champions' core damage constants, ratios, ranges, and cast timings against the local Riot-authoritative cache.
- Corrected farm and crowd-control impact timing to use official cast frames and missile speeds.

#### Locke

- Unified R multi-hit evaluation and casting so both use the same predicted landing point.
- Edge targets now count only with a 35-unit safety margin or sufficient hard CC, while a selected target stays centered as a single-target cast.

#### Teemo

- Updated Q farm-health prediction to include the official 0.493-second cast time and missile travel.
- Semi R is champion-only by default; jungle fallback is now a separate opt-in option that remains disabled by default.
- Live allied mushrooms are checked after shard reloads to prevent duplicate trap placement near existing mushrooms.

#### Malphite

- Removed the obsolete level-scaled lethality conversion so W physical-damage prediction follows the current penetration rule.
- Enforced a two-target minimum for Auto R and Semi Multi R and added landing-time, hard-CC, movement-margin, and selected-target centering checks.
- Applied Tower Combat gating to both Semi R paths and corrected Q farm prediction to the official 0.333-second cast time.

#### Soraka

- Aligned the killable circle and health-bar estimate with the Q-only automatic Combo/Harass contract.
- Corrected Q to the official 0.283-second cast time and included distance-based missile travel in hard-CC, prediction, and stasis timing.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- 新增自动回归检查，将四名英雄的核心伤害常量、系数、距离与施法时间和本地 Riot 官方缓存进行对照。
- 清线与控制判定的命中时间现在使用官方施法帧和飞行速度。

#### Locke

- R 的多目标判定与实际施放现在共用同一个预测落点。
- 边缘目标只有在保留 35 单位安全距离或拥有足够硬控时才会计入；选定目标时保持中央单目标施放。

#### Teemo

- Q 的补刀生命预测现在包含官方 0.493 秒施法时间和飞行时间。
- Semi R 默认只对英雄使用；无英雄时对野怪使用的逻辑已拆分为独立选项，并默认关闭。
- 重新载入分片后会直接检查场上的友方蘑菇，避免在已有蘑菇附近重复放置。

#### Malphite

- 移除过时的等级缩放穿甲换算，使 W 的物理伤害预测符合当前穿甲规则。
- Auto R 与 Semi Multi R 最少要求命中两名敌人，并加入落地时间、硬控、移动余量与选定目标中央瞄准判定。
- 两种 Semi R 都会遵守 Tower Combat 开关，Q 补刀预测时间修正为官方 0.333 秒。

#### Soraka

- 按照自动 Combo/Harass 只使用 Q 的规则，将可击杀圆圈与血条预估改为仅计算 Q 伤害。
- Q 施法时间修正为官方 0.283 秒，并在硬控、预测和凝滞计时中加入按距离计算的飞行时间。
<!-- MESH-AIO:RELEASE:v1.0.1:END -->

<!-- MESH-AIO:RELEASE:v1.0.0:START -->
## v1.0.0

### 한국어

#### 지원 챔피언

- Locke
- Teemo
- Malphite
- Soraka

#### 핵심 및 메뉴

- mesh-aio 단일 샤드에서 4개 챔피언을 자동 분기하고, 공용 인터럽트·스테이시스 모듈과 실시간 상태 표시 규칙을 모든 모듈에 일관되게 적용했습니다.
- 접을 수 있는 챔피언별 메뉴, 실제 스킬 아이콘, 사용자 지정 단축키와 쿨다운 연동 범위 표시를 유지하면서 런타임 충돌 방어 규칙을 보강했습니다.

#### Locke

- Q 위빙을 평타 백스윙 시작 후 0.12초 안에서만 허용하고, 사용할 수 없을 때 호출 스트림을 닫아 후반에 위빙이 영구 정지하던 문제를 수정했습니다.
- 존야·바드 R·리산드라 R로 정지된 적에게 무적 해제 순간 Q가 도착하도록 스테이시스 저격 로직을 추가했습니다.

#### Teemo

- AA → Q → AA 위빙 신호를 이중화하고 평타 사거리 밖에서는 Q를 직접 사용해, 공속이 높아진 뒤 콤보 Q가 멈추던 문제를 수정했습니다.
- 스테이시스 중 적 발밑에 R을 미리 설치하도록 추가하고, 비행시간과 1초 장전시간을 모두 반영해 해제 직후 확실하게 작동하도록 보정했습니다.
- Laugh Attack을 평타당 한 번으로 제한하고, 부활 후 상태 초기화와 만료된 독 추적 데이터 정리를 추가했습니다.

#### Malphite

- 전투 순서를 R → 착지 E → Q → AA-W-AA로 정리했으며, 평타 리셋이 아닌 E를 after-attack 경로에서 제거하고 W만 실제 평타 리셋으로 유지했습니다.
- R 다중 적중 반경을 325에서 공식 수치 270으로, 팜 Q 투사체 속도를 1400에서 1200으로 교정했습니다.
- 스테이시스 해제 순간 E가 맞도록 도착 시간을 0.242초로 보정하고 자동 저격 옵션을 추가했습니다.

#### Soraka

- 자동 Combo와 Harass는 Q만 사용하도록 정리하고, E는 수동 Force E·인터럽트·하드 CC·갭클로저·스테이시스·킬스틸 조건에서만 사용하도록 제한했습니다.
- 전 챔피언 채널링·차징 인터럽트 데이터베이스를 연결하고, 스테이시스 해제 순간 Q와 E가 도착해 점멸과 대시를 막도록 추가했습니다.
- 동일 챔피언 아군이 여러 명일 때도 각 아군의 W 우선순위와 체력 슬라이더가 독립적으로 적용되도록 수정했습니다.

### English

#### Supported Champions

- Locke
- Teemo
- Malphite
- Soraka

#### Core & Menu

- The single mesh-aio shard now dispatches all four champions while sharing the interrupt, stasis, and live status-display rules consistently across modules.
- Preserved collapsible champion menus, live spell icons, rebindable hotkeys, and cooldown-aware range drawings while strengthening runtime compatibility guards.

#### Locke

- Q weaving is now accepted only within 0.12 seconds of a fresh auto-attack backswing, and the invoke stream closes when Q cannot be used, preventing permanent late-game weave stalls.
- Added stasis timing so Q lands as Zhonya, Bard R, or Lissandra R invulnerability expires.

#### Teemo

- Reinforced the AA → Q → AA signal path and added direct Q casting outside auto range, fixing combo Q stalls at higher attack speeds.
- Added pre-placement of R under stasis targets and corrected the timing to include missile travel plus the full one-second arm time.
- Limited Laugh Attack to once per auto, reset runtime state after respawn, and cleaned expired poison tracking entries.

#### Malphite

- Standardized combat to R → landing E → Q → AA-W-AA, removed E from the after-attack path, and kept W as the only true auto-attack reset.
- Corrected the R multi-hit radius from 325 to the official 270 value and Q farm missile speed from 1400 to 1200.
- Added E stasis sniping with a corrected 0.242-second impact time so it hits immediately after invulnerability ends.

#### Soraka

- Automatic Combo and Harass now use Q only, while E is restricted to configured Force E, interrupt, hard-CC, gapcloser, stasis, and killsteal reactions.
- Connected the all-champion channel and charge interrupt database and added Q/E stasis timing that blocks immediate Flash or dash escapes.
- Fixed per-ally W priority and health sliders when multiple allied units use the same champion.

### 简体中文

#### 支持英雄

- Locke
- Teemo
- Malphite
- Soraka

#### 核心与菜单

- mesh-aio 单一分片现在会自动分配四名英雄，并在全部模块中统一使用打断、凝滞与实时状态显示规则。
- 保留可折叠的英雄菜单、真实技能图标、自定义快捷键和冷却联动范围显示，同时加强运行时兼容保护。

#### Locke

- Q 技能只会在普通攻击后摇开始后的 0.12 秒内衔接，无法施放时会关闭调用流，修复后期连招永久停止的问题。
- 新增凝滞结束狙击逻辑，使 Q 在中娅、巴德 R 或丽桑卓 R 的无敌结束瞬间命中。

#### Teemo

- 强化 AA → Q → AA 的双重触发信号，并在普攻距离外直接施放 Q，修复高攻速时连招 Q 停止的问题。
- 新增在凝滞目标脚下预先放置 R，并同时计算飞行时间与完整的一秒启用时间。
- 嘲笑动作现在每次普攻最多触发一次，同时新增复活状态重置与过期毒素记录清理。

#### Malphite

- 连招统一为 R → 落地 E → Q → AA-W-AA，E 不再进入攻击后触发路径，只有 W 保留真正的普攻重置。
- R 的多目标判定半径从 325 修正为官方数值 270，清线 Q 的飞行速度从 1400 修正为 1200。
- 新增 E 凝滞结束狙击，并把命中时间修正为 0.242 秒，使技能在无敌结束后立即命中。

#### Soraka

- 自动连招与消耗模式只使用 Q，E 仅在已配置的强制施放、打断、硬控、突进、凝滞和斩杀条件下使用。
- 接入全英雄引导与蓄力技能打断数据库，并新增 Q/E 凝滞结束计时以阻止目标立即闪现或位移。
- 修复队伍中存在多个相同英雄时，每个友军的 W 优先级与生命值滑块无法独立生效的问题。
<!-- MESH-AIO:RELEASE:v1.0.0:END -->
<!-- MESH-AIO:UPDATES:END -->
