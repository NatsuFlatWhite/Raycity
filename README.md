<!-- 임시 이미지 나중에 바꿀듯? -->
<img src="https://cdn.discordapp.com/attachments/1007603247491579904/1033734437160091679/rc.png"  width="128" height="auto">
<!-- 마지막 수정 : 2022 / 12 / 11 -->
<!-- 리얼엑스에서 활동했었을 때 임시로 만들었던 코엑스 파일 업로드 22/11/12 -->
<!-- 서버 설치 가이드 작성 22 / 11 / 30 -->
<!-- 과연 레이시티가 누군가의 의해 오픈소스로 627서버를 배포하는 날이 올까요? 
현재의 레이시티 개발자들은 몇몇 사람들 빼곤 단순한 패킷 분석도 하지 못합니다. 
단순한 클라이언트 버전 업그레이드도 못하고 있네요. 사실상 일반적인 개발자는 많이 쳐야 609까지 밖에 못간다고 생각합니다.
리버스가 627 서버를 공개하는게 아닌 이상 완전히 복원된 레이시티를 플레이 하기는 힘들다고 생각합니다.
저 역시 독자적으로 에뮬레이터를 개발하고 있고 데이터베이스를 복원하고 있지만 제 능력 부족으로 한계점은 결코 존재합니다.
저의 어린시절에 이 게임성에 빠져 열심히 플레이했던 게임인 만큼 좋은 일이 있었으면 좋겠습니다.
다들 포기하지 않고 열심히 해주셨으면 좋겠어요. -->

## Raycity Client
[Server + Client + DB](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)
<!-- 레이시티 갤러리에서 공개했던 데이터베이스 -->
[Microsoft Sql Server 2019](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## Server Setup Guide
- The Raycity server is optimized for SEA 590 (Release date : 2011-07-29)
<!-- 많은 사람들이 이 서버는 580에 맞게 제작된 서버라고 이야기 하지만 580은 11년 4월까지 사용된 버전이며 다크시티가 출시되지 않았음..
하지만 SEA 590은 이때 다크시티가 출시 되었다. 또 한 서버가 릴리즈 된 날짜와 거의 같은걸 생각하면 590이라 95% 확신중..
한국에서는 591에 다크시티가 출시된 걸 생각한다면 590은 SEA 내수용 버전이라 생각이 된다. (아닐수도 있음.. 너무 정보와 자료가 없어서..) -->
- **The current database and server have not fully recovered and are incomplete**
### DataBase
Microsoft Sql Server 2019 install

[Database Restore](https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/restore-a-database-backup-using-ssms?view=sql-server-ver16)

Sql Server Configuration Manager ->  SQL Native Client 11.0 -> Client protocol Change all to Enabled

### Server
CenterServer - config.xml info_server.xml

GameServer , Agent - config.xml

enter your IP

To connect the DB to the center server you must enter the server address, ID, password in config.xml

### Client
Tools -> Daily Tools -> thunterhk.exe -> Client -> 0m decrypt -> Raycity.0m Select

[HxD](https://mh-nexus.de/en/downloads.php?product=HxD20)

Modify the server IP and port through HxD

Change the Port from 2180 to 2080

thunterhk.exe -> Client -> 0m encrypt

## Note
CarShop Legend Slot (Client -> Data -> ui -> shopstage)

New Town traffic cars

Saha Tunnel Village Portal opened in Dogok-dong Village

UsepassPatcher (Available in all versions)

Loginstage GameGrade load (However, it disappears when you login to the game.) 

Skill use information loads properly

You can enable news by changing the news host URL in Raycity.0m to a local host or using hosting

profile creation system Fixed Now it works fine. 

NPC mission on the field are partially functional

The Jamsil portal in the COEX Town has been modified to work for the client

Quest NPC illustration load normally

### Racing
Changed the field racing fence to blue

Added a dummy racing track (A track that has been removed from the official server has also been added)

## Korean Stringbag

As of December 19, 2021, Korean-related files have been released

The in-game stringbag has about 2000 rows written

Almost all sets in the set list have been translated into Korean

All translations of the arealist have been completed

Some of the items on the itemlist have been translated into Korean

Thank you for being with me, Naro and Reverse

## Admin Console
<!-- 최초 작성 211118 나로 / 번역본 업로드 220510 -->
After changing the GlobalAccount -> RC_Account -> AccountState value to 126 Change the admin IP in the AdminIPList to activate the admin console

### Command List
help - You can check some commands

pcbang - Activate the PCRoom(ICafe) buff

legendpoint - You can earn Legend Point 

loadcar - Loads the currently worn car (ex. Xtreme , LE Race)

misson - Clear the Field NPC mission with grades that match the value (1-Poor 2-Normal 3-Good 4-Great 5-Exellent)

race track - The field racing track is changed to match the value (See RaceAgent -> Track.xml for detailed values)

race finish - finish the race immediately

wcolor 255 255 255 - You can change the color of the weather by entering a command to match the RGB values.

run start - Ignore the count and start the extreme race

run stop - You can end an extreme race that is currently in progress

Itemlist - You can search for items registered in the database (ex. itemlist Zeta Engine 2.9 Normal)

move - You can move to a reset position near the coordinates you entered. (Go to the entered coordinates when used in field racing)

pos - It tells you the coordinates of where you are

goto - Field move command (kr d1 n1 g1 t1 t2 t3 t4 t5 tutorial r1 l1 l2 f1 f2 f3 f4 f5 f6 b1 b2 b3 b4 b5)

freecam - Camera Free view

car - Registering a vehicle value creates a CheatCar.

loadracecar - Change to LE mode car. (ex. loadracecar gabriel)

item - You can create an item by entering the item value.

setitem - Enter a setitem value to create a setitem

rain - Add GameMoney

rp - Add RacePoint

inventory - You can check the items you have in the inventory window

movplay - Automated driving without destination (Value : 0 stop 1 start)

loadenv - Change the weather (sunset, day, sunrise, night, night_kr, night_d1)
<!-- 콘솔 명령어도 찾아야 하는데... -->
## Config.xml
<!-- 카트라이더의 KartRider.xml , 에버플래닛의 GameClient.xml과 동일한 형식 카트라이더 개발진 어디 안간다! ㅋㅋㅋ -->

<!-- 이 명령어의 순서는 rawFolder부터 시작해서 usePerfHud가 마지막이다. 위 2개의 게임을 통해 이 xml을 알고있다면 무슨 말인지 알 수 있다. -->
<!-- usePerfHud
carRenderLod2
dataPackOff
channel
server
loginId
enable
bypassMode
iamqa
1122qq
pw
iamshuruk
passLoading
enableDevInfo
cameraRot
autoRUN
rawFolder -->
This xml file is a file that activates the private command contained in Raycity.exe

Currently, we are constantly looking for commands, and there are commands that do not work.

some commands seem to be used in combination with other commands.

#### Available command
passLoading - It forcibly skips the intro that appears when launching the game and moves to the login screen.

#### Unverified command
bypassMode , usePerfHud , carRenderLod2 , cameraRot , rawFolder , iamshuruk

1122qq - If you include this command and run the game, the game does not start and creates a dmp.

iamqa , enableDevInfo - It's an internal developer team command, but I couldn't find a use for it.

dataPackOff - A command that allows me to run the game with DataRaw(unpacked), but it doesn't work.

<!-- ## Server Packet List
패킷 정리가 완료되면 업로드 예정 -->

<!-- # 리얼 엑스 관련여담

1. 레이스와 안나가 올린 저격글은 "레인판매"를 제외하고 전부 거짓된 저격이다.
2.레인 판매는 전부 사실이다.
3.죄송합니다. -->

<!-- 아랑드롱 박
-1579.264 -588.0891 29.36226

큐라백작
-5825.348 6864.091 27.10461

완소희
-1619.394 8157.803 16.42972

도매상 부쉬
2212.535 780.2515 14.56935 -->
