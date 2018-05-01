# Retrospective 回顧

JB: 
呼! 終於到尾聲啦!
可是...我們原本預期這30天可以完成30個需求(User Story)，可是我們最後只完成了27個吧!

Lily: 
孩子，我們不是鐵人，難免事情無法完美。

Hachi: 
至少我們過程中學習了GOF的設計模式並且應用在這些實際的需求!

Lily:
你說的沒錯! Stay Agile! 最後，讓我們來想看看除了設計模式，還有哪些觀念和技巧能讓我們寫出更好的程式!


## 守、破、離

第一天有提到學習設計模式的步驟：
1. 買(借)本好書
2. 初步了解設計模式 (先有概念)
3. 模仿及練習書上範例
4. 重新再讀一次
5. 以實務需求思考及實作
6. 參考別人經驗

以上是**守**。
而當我們熟悉了設計模式和六大原則後，慢慢的在我們開發程式時就可以開始嘗試去組合、簡化、變化，這是**破**。
最後我們希望可以達到**離**的境界，也就是不管我們寫簡單或複雜的程式，都自然而然的寫出符合這些原則且容易維護、擴展和易讀的好程式，即使我們已經忘記了這個模式叫作什麼名字。

> 「以無法為有法，以無限為有限。」 - 李小龍


## 羽化

Kent Beck 提出的簡單設計原則
```
1. 執行完所有測試
2. 重構：禁止重複
3. 重構：具表達力
4. 重構：最小化類別及方法的數量，避免過度設計
(<<Clean Code 無瑕的程式碼 - 羽化>> 頁189)
```

這些原則提供了我們另一個明確的方向，
**未經過測試的程式碼是一顆未爆彈**，請建立單元測試來保護你的程式碼(和保護自己!)。
**過度設計**造成浪費，在進行設計前都應該先自問是否必須且合理。

好的程式碼不一定是**增加**，**減少**也是重構的重點，請遵守...
```
1. 廢棄多餘的註解
2. 移除被遺棄的程式碼
3. 避免模糊的意圖
4. 避免魔術數字
(<<Clean Code 無瑕的程式碼 - 程式碼的氣味和啟發>> 頁315)
```


### 唯一的不變就是變

現今的環境和需求變化非常的快，Programmer除了持續學習新的東西，也要持續維護和開發自己或別人的舊程式。
想像別人正在修改我們的程式碼，我們希望能帶給他人一個愉快的撰寫過程，而不是WTF ...


## UML和文件

快速變化的環境導致文件(Documentation)常被忽略，或是交差了事。
想像你現在剛接手一個不小的系統，並且需要快速的釐清這個系統的來龍去脈和需求，直接閱讀幾萬行的程式碼可能不是最好的選項。

```
1. 好的文件對於任何專案來說，都是不可或缺的。缺少它們，團隊就會迷失在程式碼的海洋之中。
2. 知道哪些東西不需要文件化，和知道哪些需要文件化，同等重要。
(<<無瑕的程式碼(敏捷完整篇)─物件導向原則、設計模式與C#實踐>> 頁205)
```

我極力建議在設計階段或是文件上使用UML來溝通，因為圖形比一堆文字更好閱讀和溝通。
而且，如果你需要和國外團隊合作，過多的文字描述相對下可能造成更多困惑和誤解 (Confusing and Misunderstanding)。

但是花費太多時間在繪製圖形(UML或流程圖...)也可能造成浪費。
所以何時該繪製圖示呢？

```
1. 當有幾個人需要理解設計中某個特定部分結構時
2. 團隊達成一致的共識
3. 你想要嘗試一個設計想法，而圖示有助於你進行思考
(<<無瑕的程式碼(敏捷完整篇)─物件導向原則、設計模式與C#實踐>> 頁203)
```


### Reference
- Clean Code 無瑕的程式碼
- 無瑕的程式碼(敏捷完整篇)─物件導向原則、設計模式與C#實踐

