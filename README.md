#### This project is currently on a temporary hiatus indefinitely.
## Raycity Client or Tools
https://drive.google.com/file/d/1MXf-bWQRFGvc7D5m7Y7QLwMy9Hgh5xMu/view (Server + Client + DB + Tools)

https://drive.google.com/file/d/1kOW9Z_SOo3PGRzcsXoKW0Mr5URvfrHR7/view?usp=sharing (Daily Tool comdlg32.ocx)

https://www.microsoft.com/ko-kr/sql-server/sql-server-downloads (Mssql 2019)

## Complete Fix
CarShop Legend Slot (Client -> Data -> ui -> shopstage)

New Town traffic cars

Saha Tunnel Village(Dark City Town) Portal opened in Dogok-dong Village

UsepassPatcher (Available in all versions)

Loginstage 게임이용등급 load (However, it disappears when you login to the game.) 

Skill use information loads properly

You can enable news by changing the news URL in Raycity.0m to a local host or using hosting.

profile creation system Fixed Now it works fine. 

NPC mission on the field are partially functional

The Jamsil portal in the COEX Town has been modified to work for the client

Quest NPC illustration load normally

### Etc

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

goto - Field move command (kr d1 n1 g1 t1 t2 t3 t4 t5 tutorial r1 l1 l2 f1~f6 b1~b5)

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

<!-- 리얼엑스에 관하여, 이야기를 해봅니다. 어차피 볼 사람도 없으니깐.
우리를 욕하던 핑크 , 레이스도 결국 레인을 판매하던게 맞았다. 애초에 우리도 예상을 했고 레인을 판매하자는 계획도 쟤들도 판매하는데 우리는 왜 못파냐? 라는 식으로 시작했던거다.
물론 정말 잘못된 짓이 맞으며 나도 이 부분에선 별 말을 하지 않았고 하지도 못했다. 잘못이 맞으니깐. 하지만 레인 판매건 이후는 전부 "거짓말이 섞인 저격글이다."
내가 왜 19살인가.. 싶다 19살인건 "나로" 혼자 이며 리버스와 나는 아직 미성년자이다. 왜 뿌려도 내 얼굴만 뿌렸을까..
오히려 그 둘이 안뿌려진게 정말 다행이다. 지금 와서 본인들도 얼굴 가지고 있어봤자 뭐에 써먹는가? 
"그니깐 걔네들이 리얼디비 빼올려다가 짤린거임" 이라는 유동 댓글에는 맞다고 적었다. 우리는 리얼 디비 빼갈 생각도 없었다. 애초에 서버 파일 이야기 꺼낸건 본인들이다.
"틈만나면 남 아이피만 쳐 따고있고 실상은 그 아이피로 아무것도못하고" 라는 댓글도 있는데
난 남의 아이피를 따는 방법을 모른다. 관심도 없다. 그저 밀크 서버 시절 밀크가 서버 아이피를 준걸 그 둘에게만 보여줬을뿐 난 아이피 따는법 모른다.
"븅신새끼들이 어드민한테 빌붙어서 레인 20억씩 땡겨놓고" 본인들도 이거 써먹었다. 우리랑 같이 레인 복사 했고 어드민 계정 제일 잘 활용한 사람은 본인들이다.
"본인등판했노 병신새끼 그렇게 돈벌어서 친구들셋이서 배그사서 배그하고" 우리는 배그를 전부 기존에 구매를 했었고 레인 판매건이랑 관련이 없다.
그 돈은 본인이 정말 필요한곳에 썼다. 지금 생각하면 그냥 팔지말고 상황 구경이나 할걸 그랬다.
"태국관리자들한테 물어봐도 니네 하는거 좆도없구만" 이 부분은 우리쪽도 억울한게 우리는 스트링백을 전부 작성해서 넘겨줬다.
하지만 버그가 난다는 이유로 우리 스트링백은 적용되고 항상 제외되었는데 그래서 우리가 로닌에게 
"버그가 나는걸 우리 서버에서는 확인하지 못하니 너희 개발자 서버에서 작업을 해도 괜찮은가?" 라고 보냈으나 로닌은 안된다며 칼같이 답 했고. 우리쪽에서도 별 다른 해결 방법이 없었다.
나름 열심히 작업 했으나 적용은 되지 못했다. 그리고 갤에서 저렇게 떡밥 돌려지는것도 싫고 서로가 이야기를 해서 해결을 하는게 더 좋을거 같으니
따로 오픈톡을 파서 이야기를 했다. 대충 예전 일이라 잘 기억 안나는데 뭐 대충 우리 밀어 붙이고 우리가 질문 할때는 말 돌리는 식으로 진행 했었다. 결국 우리쪽에서는 별 다른 진전이 없었고 이야기를 끝냈다. 하지만 갤에서 똑같이 또 우리 욕을 하며 떡밥을 굴리는게 아닌가? 나로는 결국 갤에다가 상황 정리글 과 핑크 , 레이스에 대한 저격글을 썼으나
"레인 판거 자체부터가 잘못인데 쿨하게 넘어가는게.. 라고 댓글을 달았다고 정신도 없고 일 키우기도 싫으니 그냥 글 내렸다.."의 글을 봤고.. 뭐 우리 둘도 이해하며 그냥 조용하게 있자
라며 상황을 조용히 넘어갔다. 몇일 뒤가 지나고 난 뒤.. 리얼엑스에서 "핑크와 레이스가 어드민에서 퇴출 당하였다는 소식을 듣고" 재 빠르게 어떻게 짤린건지 확인하러 돌아다녔다.
Black이라는 이름으로 "일반 유저한테 레인을 판매하고 다녔다는것.." 우리는 이걸 보고 몇초정도 정적이 흘렀었다. 그리고 우리가 예상하던게 맞았다고..
이 글을 보고 있는 사람이라면 알텐데, "어드민 계정으로 레인 20억 땡기고 다니고." 여기서부터 문제가 되는거다. 우리는 이미 알고 있었고 우리보다 먼저 게임머니를 판매한건 본인들이었다.
그리고 이건 나로가 갤에 올렸던 글에 일부인데.. "레인을 판매한건 사실 이건 깔끔히 사실이니까 인정한다. 근데 [KR] King 너가 "Black"이 내 부계정이다 라고 "리얼엑스 한국 디스코드 어드민 음성방"에서 직접 말하지 않았나? 근데 왜 Black이라는 사람이 왜 레인을 판매하는거냐? " 라고 우리의 예상이 맞고 결국엔 확증이 있던건데 그 확증을 지나가듯이. 캡처를 못하고
녹음을 못하다보니 오히려 확증이 있는 상황인데 심증밖에 없어진거였다. 아직도 나는 리얼엑스에서 있었던 기억들이 나쁘다고 생각하지 않는다.
재미도 있었고 그에 맞게 억울한 일도 있었지만 뭐, 별 수 있나 우리는 대처를 너무 늦게했고 불리한 조건에서 싸우다 보니 이런 상황이 발생했다.
오늘도 조용히 난 레이시티판의 상황을 지켜본다. 그리고 레인 판매건 아직도 후회 하고있고 정말 잘못했다 우리한테 산 사람한테는 미안하다는 말을 전해주고 싶다..
한국 어드민이 레인을 판매한다고 해서 우리도 따라서 판매하면 안됐었는데 생각을 잘못했었다. 정말 미안하다. 
나 , 나로 , 리버스 전부 똑같은 생각이고 아직도 반성하고있다. 미안하다.


아무도 보지 않을 내 깃허브도 조용히 수정을 하며.. -->
