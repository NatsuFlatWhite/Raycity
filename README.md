<p align="center">
  <<a href="https://github.com/NatsuFlatWhite/Raycity/blob/main/KR.md">한국어</a>
  |
  <b>English</b>>
</p>

##

<img src="title.jpg"  width="auto" height="auto">

<p align="center">
  레이시티
  |
  Raycity
  |
  光線飛車
  |
  光速城市
</p>

[Raycity](https://mm.pmang.kr/pmang/raycity/event/20130329/popup.html#none) is an openworld MMO Racing Game set in Seoul developed by [J2M Soft](https://www.ea.com/ko-kr/ea-studios/ea-korea)</br>
published by [Neowiz](https://www.neowiz.com)'s Game Portal [Pmang](http://file.pmang.com/html/pmang/404/game/314_error.html)

##
 
This project is not related to private servers currently operated for **commercial purposes**</br>
inform you that this is created by an individual for the purpose of simple study and research

## Raycity Client
[Server + Client + DB](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)

[Microsoft Sql Server](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## Server Setup Guide
- The Raycity server is optimized for SEA 590 (Release date : 2011-07-29)
- **Running higher clients** requires internal **packet modification** of the server
- **The current database and server have not fully recovered and are incomplete**

### DataBase
Microsoft Sql Server install

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
Legend System

New Town (Dark City) Traffic Cars

Saha Tunnel Village Portal opened in Dogok-dong Village

LuckySpot Lucky Rain

Facebook

Take A Rest and Korean Grade

Beginner Help manual

File recovery system (Fileinfo.0m Features that only existed on Korea server)

UsepassPatcher (Available in all versions)

Skill use information loads properly

profile creation system Fixed Now it works fine. 

Field NPC missions operate normally

The Jamsil portal in the COEX Town has been modified to work for the client

Quest NPC illustration load normally / The NPC dialogue script is displayed

Guild System and Zone Battle

RoadFight 

[Korea Game Forced Shutdown System](https://www.law.go.kr/%EB%B2%95%EB%A0%B9/%EC%B2%AD%EC%86%8C%EB%85%84%EB%B3%B4%ED%98%B8%EB%B2%95/(20210101,17761,20201229)/%EC%A0%9C26%EC%A1%B0) <!-- wrShutdownMsg 셧다운시간이 되어 게임이 종료 됩니다. -->

Field Environment Event / Xtreme Night

Under Neon / Emblem / TPart / Saver

LevelBoost

Crash Time

### Datasub
Web Loading Image

Upload Image

AD

News

Manual

### Racing
Changed the field racing fence to blue (Fence that was only patched on the Korean live server)

Added a dummy racing track (A track that has been removed from the official server has also been added)

Load UI.2 and item mode

Rejoin Button

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

wcolor R G B - You can change the color of the weather by entering a command to match the RGB values.

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

headlight - Turns the headlights on and off

signborad - Turn the signboard light on and off

Other commands can be found through analysis

## Config.xml
This xml file is a file that activates the **Private Command** contained in Raycity.exe
</br>
- usePerfHud is short for Performance Heads Up DisPlay</br>
- If you enableDevInfo The developer-only console is activated & UsepassPatcher will work by default.</br>
- When using dataPackOff you can run the game with the data unpacked through the DataRaw folder.</br> 
- passLoading is activated the video intro and loading at the beginning of the game are bypassed</br>
- iamshuruk acts as an activation key for some commands</br>
- iamqa provides private functions used by the QA team (For example you can gain access to the internal QA server) </br>
- bypassMode omits the ID input/channel entry process</br>
- RawFolder is a command related to the DataRaw folder

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
This is a description of the data00~21.0m files.

This file receives and saves when a specific table is modified or a new column is added.

That means that the official server save data contains stock, itemlist, Stringbag, Road Fighter+@ files that were maintained until just before the end of the service.

In the case of a private server containing the original data it is likely that the contents of the file were obtained by decrypting the file.

