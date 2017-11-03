# Brian's test case practice

## 搜尋歌手 kajagoogoo
先複製 testSearchArtist 這個測試案例，貼到底下
修改 method 名稱為 ###testSearchArtistForKajagoogoo

先去等待首頁的放大鏡跑出來，跑出來代表已經loading結束，點擊放大鏡會focus到輸入框中

目前沒有手機，無法檢測APP上的各個元素名稱，看網頁版KKBOX的搜尋欄名稱不是"search_src_text"，可能和手機板不一樣(?)
在搜尋欄裡面鍵入 "kajagoogoo" 
按下Enter 送出搜尋

等到畫面上方分頁欄位跑出 "ARTIST" 則代表該頁面loading 結束，點擊該分頁。

執行斷言，如果頁面上有 "Kajagoogoo (卡加咕咕合唱團)" 則 True。 也就沒事發生。



## 搜尋歌曲 too shy
先複製 testSearchSong 這個測試案例，貼到底下
修改 method 名稱為 ###testSearchSongForToo_shy

先去等待首頁的放大鏡跑出來，跑出來代表已經loading結束，點擊放大鏡會focus到輸入框中

目前沒有手機，無法檢測APP上的各個元素名稱，看網頁版KKBOX的搜尋欄名稱不是"search_src_text"，可能和手機板不一樣(?)
在搜尋欄裡面鍵入 "too shy" 
按下Enter 送出搜尋

等到畫面上方分頁欄位跑出 "SONG" 則代表該頁面loading 結束，點擊該分頁。

執行斷言，如果頁面上有 "Too Shy" 則 True。 也就沒事發生。



## 搜尋專輯 5566
先研究一下 TODO 的部分，去仔細看一下 
kkbox.openSearch().search("linkin park").checkArtistResult("Linkin Park (聯合公園)");
各方法為何?

看了一下 TestBuilder、KKPage、KKSearchPage 等類別的結構跟方法。
(KKLoginPage 是 @BeforeClass 用的)

複製 checkTopResult 去改寫，多增加尋找 "album" 的指令，其他以此類推。
(用網頁>檢查 看該按鈕的href，看他在get search=XXXX，去猜手機APP可能是哪個字)



## 搜尋歌單 蔡依林
複製 checkAlbumResult 去改寫，多增加尋找 "playlist" 的指令，其他以此類推。