 <img src="https://raw.githubusercontent.com/imhatepython/Raycity/main/logo.png"  width="128" height="auto">
This project is not related to private servers currently operated for commercial purposes.</br>
We would like to inform you that this is a project created by an individual for the purpose of simple study and research.

## Raycity Client
[Server + Client + DB](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)

[Microsoft Sql Server 2019](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## Server Setup Guide
- The Raycity server is optimized for SEA 590 (Release date : 2011-07-29)
- **The current database and server have not fully recovered and are incomplete**
- [Developer Discord](https://discord.gg/DRBYQnpS5S) <!-- Discord Channel with pink princess and sick people  If you check this out. Run away from this game -->
### DataBase
Microsoft Sql Server 2019 install

[Database Restore](https://learn.microsoft.com/en-us/sql/relational-databases/backup-restore/restore-a-database-backup-using-ssms?view=sql-server-ver16)

Sql Server Configuration Manager ->  SQL Native Client 11.0 -> Client protocol Change all to Enabled

### Server
CenterServer - config.xml info_server.xml

GameServer , Agent - config.xml

enter your IP
</br>
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

Itemlist - You can search for items registered in the database (ex. itemlist Theta Engine 2.9 Normal)

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

## Config.xml
This xml file is a file that activates the private command contained in Raycity.exe

### List
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

## DataSub
저는 과거 이 2011 SG 다크시티 서버팩에선 데이터서브와 통신은 뉴스와 베스트 스크린샷 + etc의 일부 기능만 제대로 작동하는 줄 알았습니다.

하지만 그게 아니라 그 서버는 멀쩡한 서버였고 기타 통신까지 전부 가능한 공식 서버팩이 맞았습니다.

중요한 요점은 데이터서브에 있는 data00~21.0m 이 파일인데

이 파일은 특정 지정된 테이블의 수정이나 새로운 열이 추가가 된되면 그걸 받아와서 저장을 합니다.

이걸 본섭 파일로 생각을 한다면 서비스 종료 직전까지 유지된 스톡 아이템리스트 스트링백 +@ 파일들이 있는겁니다.

항상 리버스 레이시티에 대한 의문점이 많았는데 리버스도 이 파일의 암호화를 풀어서 데이터를 얻은걸로 추측이 됩니다.

파일 암호화가 생각보다 단순해서 내가 좀 친다 생각이 드신다면 한번 시도해 보시면 좋은 결과가 있을겁니다.
