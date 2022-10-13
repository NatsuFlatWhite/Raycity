#### This project is currently on a temporary hiatus indefinitely.
<!-- 마지막 수정 : 2022 / 10 / 13 -->
## Raycity Client or Tools
https://drive.google.com/file/d/1OfNaw38EOSfhIWuixs0CWiziDXXGeREV/view?usp=sharing (Server + Client + DB + Tools)

https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads (MSSQL 2019)

<!-- ## Server Setup Guide

준비중 (예정에는 있는데 아직 모르겠음) -->

## Note
CarShop Legend Slot (Client -> Data -> ui -> shopstage)

New Town traffic cars

Saha Tunnel Village Portal opened in Dogok-dong Village

UsepassPatcher (Available in all versions)

Loginstage GameGrade load (However, it disappears when you login to the game.) 

Skill use information loads properly

You can enable news by changing the news URL in Raycity.0m to a local host or using hosting.

profile creation system Fixed Now it works fine. 

NPC mission on the field are partially functional

The Jamsil portal in the COEX Town has been modified to work for the client

Quest NPC illustration load normally

<!-- 609 이전 서버시절에 고친 리스트
Dest
럭키레인
오픈마켓
아이템 기간 무제한
사용 아이템 ex. 루마의 배터리 , 공구 상자 , 차량키 , 골드 키트 등등..
신비한 주사위


609 버전 업 / 2022 - 10 - 11 / 아직 배포 X
클라이언트 패킷 분석 완료 및 데이터베이스 프로시저와 테이블 수정 완료
차량 가격 본섭기준으로 수정 완료 다만, 자료가 없을 경우 1원으로 처리 (가이드북 Vol.1 기준)
한국 클라이언트 사용 가능 다만 609 한국 클라이언트가 없어서 미완성 627 서버로 실행해야함
버전업 진행 과정에서 고친 기능 리스트

유저 레벨 50
초광속의 영역
시즌 상점
NPC 기능 ex. 엔젤러스 , 모터쇼
빙고
기타 스트링백 (fontsize , NPC 대사)
게임 전체이용가 등급 안내 (%d 시간째 운전 중 입니다. 과도한 게임이용은 정상적인 일상생활에 지장을 줄 수 있습니다.)
도우미 기능 (도움주기 도움받기)
캡슐과 부적
필드 미션
로드파이터
퀘스트
급 별 레이싱 세타리그 추가
레이싱 트랙 텍스쳐 깨짐 현상 (부산 , F1)
전반적인 길드 시스템
코팅 페인트 부스터 페인트 2차 외형 골드 키
필드 시간대 자동 변경
전반적인 다크시티 기능들
레이스 UI 2 , 아이템 모드
폭주
레벨 부스터
낭만이 있는 네오위즈 인트로와 EA 인트로
미공개 개발자 전용 시스템 -->

### Racing
<!-- 더미트랙 삭제는 클라이언트에서 진행해 주세요. 레이스 서버 xml은 굳이 건들 필요 없어요! 
서버에 할당이 안되어있는 트랙이면 선택이 안됩니다. 그래서 서버쪽 xml은 냅두는편이 좋아요. -->

<!-- 펜스는 역시 600 이후 버전의 유물 파란펜스 -->
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
After changing the GlobalAccount -> RC_Account -> AccountState value to 126 register the admin IP in the AdminIPList to activate the admin console

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
This xml file is a file that activates the private command contained in Raycity.exe.

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
