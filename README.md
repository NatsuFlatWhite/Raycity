<img src="https://cdn.discordapp.com/attachments/1007603247491579904/1033734437160091679/rc.png"  width="128" height="auto">

## Raycity Client
[Server + Client + DB](https://drive.google.com/file/d/1FqvwlxtqDCkRy7KGYMwytcfSkeZxE_gc/view?usp=share_link)

[Microsoft Sql Server 2019](https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads)

## Server Setup Guide
- The Raycity server is optimized for SEA 590 (Release date : 2011-07-29)
- **The current database and server have not fully recovered and are incomplete**
- [Developer Discord](https://discord.gg/DRBYQnpS5S)
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
This xml file is a file that activates the private command contained in Raycity.exe

Currently, we are constantly looking for commands, and there are commands that do not work.

some commands seem to be used in combination with other commands.

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
 
