<!-- 임시 이미지 나중에 바꿀듯? -->
<img src="https://media.discordapp.net/attachments/1007603247491579904/1033734437160091679/rc.png"  width="128" height="auto">
<!-- 마지막 수정 : 2022 / 11 / 30 -->
<!-- 리얼엑스에서 활동했었을 때 임시로 만들었던 코엑스 파일 업로드 22/11/12 -->
<!-- 서버 설치 가이드 작성 22 / 11 / 30 -->

## Raycity Client
[Server + Client + DB](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)

[Microsoft Sql Server 2019](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## Server Setup Guide

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

Thank you for being with me, Naro and Rerverse

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

## Config.xml
<!-- 카트라이더의 KartRider.xml , 에버플래닛의 GameClient.xml과 동일한 형식 카트라이더 개발진 어디 안간다! ㅋㅋㅋ-->

<!-- 작동이 안되는 명령어들은 0m에서 작동하는지 확인중.. -->
This xml file is a file that activates the private command contained in Raycity.exe

Currently, we are constantly looking for commands, and there are commands that do not work.

It is speculative, but some commands seem to be used in combination with other commands.

(ex. <datapackOff rawFolder＝'Raycity\DataRaw' />

#### Available command
passLoading - It forcibly skips the intro that appears when launching the game and moves to the login screen.

#### Unverified command
bypassMode , usePerfHud , carRenderLod2 , cameraRot , rawFolder , iamshuruk

1122qq - If you include this command and run the game, the game does not start and creates a dmp.

iamqa , enableDevInfo - It's an internal developer team command, but I couldn't find a use for it.

dataPackOff - A command that allows me to run the game with DataRaw(unpacked), but it doesn't work.


<!-- # 리얼 엑스 관련여담

1. 레이스와 안나가 올린 저격글은 "레인판매"를 제외하고 전부 거짓된 저격이다.
2.레인 판매는 전부 사실이다.
3.죄송합니다. -->
<!-- 학교 관련 일 때문에 프로젝트 임시 중단.. 그래도 시간 날 때 분석이라도 해보자! 
627 서버의 완성은 언제쯤..... -->
