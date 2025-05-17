<p align="center">
  <<b>한국어</b>
  |
  <a href="https://github.com/NatsuFlatWhite/Raycity">English</a>>
</p>

##

<img src="title.jpg"  width="auto" height="auto">

<p align="center">
  수천대가 함께 서울을 달리는 레이싱특별시 레이시티~
  
[레이싱특별시 레이시티](https://mm.pmang.kr/pmang/raycity/event/20130329/popup.html#none)는 [제이투엠소프트](https://www.ea.com/ko-kr/ea-studios/ea-korea)에서 개발하고 [네오위즈 게임즈](https://www.neowiz.com)사의 게임 포털 [피망](http://file.pmang.com/html/pmang/404/game/314_error.html)<!-- 이 링크는 http로 들어가면 레이시티 이미지가 뜬다.-->에서 서비스가 되었던 게임입니다. </br>
또한, 채널링 서비스를 통해 [투니랜드](https://youtu.be/5IUQHmeKHD0?si=juyYJT0nqMHy-X_c)와 [벅스 피망](https://game.bugs.co.kr/)에서도 플레이가 가능했습니다.
##
이 리포지토리는 **상업적인 목적의 개인 서버**와는 관련이 없습니다.

## 유틸리티
[DB / 서버 / 클라이언트](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)

[Microsoft Sql Server](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## 서버 설정 가이드
- 해당 레이시티 서버는 지역코드 SG(SEA) 1.590.0.1 다크시티 1차 업데이트 버전에 최적화 되어 있습니다. (릴리즈 날짜 : 2011-07-29)
- **더 높은 클라이언트**를 구동하려면 **패킷 분석**과 **역공학**이 필요합니다.
- **현재 데이터베이스 및 서버는 완전히 복구되지 않았으며 불완전합니다.**

### SSMS DataBase
Microsoft Sql Server를 설치합니다.

[데이터베이스 복원](https://learn.microsoft.com/ko-kr/sql/relational-databases/backup-restore/restore-a-database-backup-using-ssms?view=sql-server-ver16)을 합니다.

Sql Server 구성 관리자 → SQL Native Client 11.0 구성 → 클라이언트 프로토콜을 모두 사용으로 변경합니다.</br>

### 서버
CenterServer - config.xml info_server.xml

GameServer , Agent - config.xml

해당 xml에 IP를 입력합니다.

DB를 센터 서버에 연결하려면 config.xml에서 서버 이름과 계정 정보를 입력해야 연동됩니다.

### 클라이언트
Tools → Daily Tools → thunterhk.exe → Client → 0m decrypt → Raycity.0m을 선택합니다.

[HxD](https://mh-nexus.de/en/downloads.php?product=HxD20)를 설치합니다.

HxD를 통해 IP와 포트를 수정하세요.

포트를 2180에서 2080으로 변경하세요.

thunterhk.exe → 0m encrypt

## 레이싱
필드 레이싱 펜스를 파란색으로 변경 하였습니다. [(해당 펜스는 한국 서버만 적용된 펜스입니다.)](https://blog.naver.com/kt1455/90146161907) 

공식 서버에서 사용되지 않았거나 삭제된 트랙을 추가했습니다.

레이싱 UI 2를 불러옵니다.

한국 서버 기능인 재입장 버튼을 사용할 수 있습니다.

## 치트 코드
Database → GlobalAccount → RC_Account → AccountState 값을 126으로 변경한 후 AdminIPList에서 관리자 IP를 변경하여 관리자 콘솔을 활성화합니다.

### 명령어 리스트
help - 일부 커맨드를 확인할 수 있습니다.

pcbang - 레이시티 PC방 버프를 획득합니다.

legendpoint - 레전드 포인트를 획득합니다. 

loadcar - 급 별 레이싱 혹은 질주/폭주에서 원래 차량을 불러옵니다.

misson - 필드 NPC 미션을 원하는 단계로 클리어합니다. (1-Poor 2-Normal 3-Good 4-Great 5-Exellent)

race track - 레이싱 트랙을 변경합니다. (자세한 값은 Track.xml을 참고하세요.)

race finish - 레이싱 경기를 완주합니다.

wcolor R G B - RGB 값을 입력하여 날씨 색상을 변경할 수 있습니다.

run start - 질주/폭주를 시작합니다.

run stop - 질주/폭주를 종료합니다.

Itemlist - 아이템리스트에 등록된 아이템을 검색할 수 있습니다. (예: itemlist 김박사의 트리플 캡슐)

move - 입력한 좌표 근처의 재설정 위치로 이동합니다. (필드 레이싱의 경우 입력한 좌표로 이동합니다.)

pos - 본인의 좌표를 알려줍니다.

goto - 필드 이동 명령어 (kr d1 n1 g1 t1 t2 t3 t4 t5 tutorial r1 l1 l2 f1 f2 f3 f4 f5 f6 b1 b2 b3 b4 b5)

freecam - 프리카메라를 활성화합니다.

car - 차량 번호를 입력하면 치트카가 생성됩니다.

loadracecar - 급 별 레이싱 차량으로 변경할 수 있습니다. (예: loadracecar gabriel)

item - 아이템 코드 혹은 아이템 이름을 입력하면 아이템을 받을 수 있습니다.

setitem - 세트 아이템 코드를 입력하면 세트아이템을 받을 수 있습니다.

rain - 레인을 추가합니다.

rp - RP를 추가합니다.

inventory - 물품창에 보유하고 있는 아이템을 확인할 수 있습니다.

movplay - 추격차량이 됩니다. (값 : 0 stop / 1 start)

loadenv - 날씨를 변경할 수 있습니다. (sunset, day, sunrise, night, night_kr, night_d1)

headlight - 헤드라이트를 켜거나 끌 수 있습니다.

signborad - 간판을 끄거나 켤 수 있습니다.

이 외의 명령어는 분석을 통해 얻을 수 있습니다.

## Config.xml
이 xml 파일은 Raycity.exe에 포함된 내부 개발자 전용 명령어를 활성화하는 파일입니다.
</br>
- usePerfHud는 Use Performance Heads Up DisPlay의 약자입니다.</br>
- DevInfo를 활성화하면 개발자 전용 콘솔이 활성화되고 passPatcher가 기본적으로 작동합니다.</br>
- dataPackOff를 사용하면 DataRaw 폴더를 통해 언팩된 데이터로 게임을 실행할 수 있습니다.</br> 
- passLoading이 활성화 된다면 게임 시작 시 비디오 인트로 및 로딩이 무시됩니다.</br>
- iamshuruk는 일부 명령에 대한 활성화 키 역할을 합니다.</br>
- iamqa는 QA 팀에서 사용하는 기능을 제공합니다.</br>
- bypassMode는 ID 입력/채널 진입 과정을 생략하고 접속할 수 있습니다.

### 리스트
usePerfHud
carRenderLod2
dataPackOff
bypassMode enable loginId channel
iamqa
iamshuruk pw 1122qq
passLoading
enableDevInfo
cameraRot
autoRUN
rawFolder 

## 데이터 서브
데이터 서브에 있는 data00~21.0m에 파일에 관한 설명입니다.

이 파일은 특정 테이블을 수정하거나 새 열을 추가할 때 받아와서 저장합니다.

이걸 본섭 파일울 가정하여 생각한다면 서비스 종료 직전까지 사용 된 스톡, 아이템리스트, 스트링백, 로드파이터+@ 파일을 얻을 수 있습니다.

본섭 데이터를 가지고 있는 서버의 경우 이 방법을 통해 얻어낸 걸로 추측할 수 있습니다.

파일 암호화가 <!-- JMD 파일의 KRData 암호화 구조를 알고 있다면..--> 생각보다 단순해서 내가 좀 친다 생각이 드신다면 한 번 시도해 보시면 좋은 결과가 있을겁니다.
