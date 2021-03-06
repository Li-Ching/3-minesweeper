# minesweeper踩地雷

## 1092物件導向程式設計小專題

### 第三組

***

* [成員](#成員)
* [分工](#分工)
* [遊戲說明](#遊戲說明)
* [程式碼註解](#程式碼註解)
* [小專題要求](#小專題要求)
  * [補充](#補充)
* [遊戲畫面](#遊戲畫面)

***

<h4 id="成員">成員</h4>

* 組長
  * 陳力菁 A9210256
* 組員
  * 李丹尼 A9210311
  * 張宥楨 A9250789

***

<h4 id="分工">分工</h4>

>找參考資料
>>陳力菁
>>
>>李丹尼
>>
>>張宥禎
>
>寫程式
>>陳力菁
>
>寫註解
>>李丹尼
>>
>>張宥禎
>
>最終檢查
>>陳力菁 

***

<h4 id="遊戲說明">遊戲說明</h4>

  在一張地圖上會有許多小方塊需要點開，點開小方塊後會顯示一個數字，這個數字就代表著以它為中心的九宮格內藏著幾顆地雷，只要點到地雷就輸了。
  踩地雷的獲勝條件是點開所有安全方塊，遊戲中也有**標記**功能可以標記地雷來避免自己誤觸。

***

<h4 id="程式碼註解">程式碼註解</h4>

* data field
  * `ROWS：行數`
  * `COLUMNS：列數`
  * `MINES：地雷數`
* minesweeper物件內容
  * `clearBoards：清除遊戲版面`
  * `placeMines：放置地雷`
  * `replaceMine：重新放置地雷`
  * `indexToChar：將數字變為字元`
  * `charToIndex：將字元變為數字`
  * `displayBoard：設置展示遊戲版面`
  * `isValid：確定行列的數目是否為正確`
  * `isMine：查看此位置是否為地雷`
  * `getNeighbours：取得相鄰地雷的數目`
  * `countAdjacentMines：數相鄰的地雷數目`
  * `uncoverBoard：設置揭開地板(移動)`
  * `markMines：確認是否標記正確的地雷`
  * `playMinesweeper：開始遊戲`
* main內容
  *  `srand(time(0))：設定種子數`
  *  `level：用於確定是否選擇遊戲等級`

***

<h4 id="小專題要求">小專題要求</h4>

- [x]  要有GitHub Commit 紀錄
- [x]  要寫分工(有不做事之情況請跟老師及助教反應)
- [x]  務必含有1個或以上之"物件"及其該有的內容及功能(包括data field、constructor、function、private)
- [x]  物件皆要封裝
- [x]  要做防呆

<h5 id="補充">補充</h5>

* 防呆
  * 在輸入數字方面有特別確認輸入內容是否為遊戲要求
  * 輸入save or flag中有避免輸入錯誤字元
* 覺得似乎可以再改進的部分
  * 在最一開始遊戲等級部分也許可以自行輸入格數及地雷數
  * 在已經有標記flag時，若是標記錯誤，在踩到地雷時顯示會使用#顯示所有地雷，但尚未做出顯示哪個flag其實是安全的
  * (待續...

***

<h4 id="遊戲畫面">遊戲畫面</h4>

![minesweeper](https://user-images.githubusercontent.com/79957564/123134978-e738dd80-d483-11eb-9c4b-73df10d74442.png)

