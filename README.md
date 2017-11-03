# kkbox-labs

# First
先複製 testSearchArtist 這個測試案例，貼到底下
修改 method 名稱為 ##testSearchArtistForKajagoogoo

先去等待首頁的放大鏡跑出來，跑出來代表已經loading結束，點擊放大鏡會focus到輸入框中

目前沒有手機，無法檢測APP上的各個元素名稱，看網頁版KKBOX的搜尋欄名稱不是"search_src_text"，可能和手機板不一樣(?)
在搜尋欄裡面鍵入 "kajagoogoo" 
按下Enter 送出搜尋

等到畫面上方分頁欄位跑出 "ARTIST" 則代表該頁面loading 結束，點擊該分頁。

執行斷言，如果頁面上有 "Kajagoogoo (卡加咕咕合唱團)" 則 True。 也就沒事發生。



# Secend
先複製 testSearchSong 這個測試案例，貼到底下
修改 method 名稱為 ##testSearchSongForToo_shy

先去等待首頁的放大鏡跑出來，跑出來代表已經loading結束，點擊放大鏡會focus到輸入框中

目前沒有手機，無法檢測APP上的各個元素名稱，看網頁版KKBOX的搜尋欄名稱不是"search_src_text"，可能和手機板不一樣(?)
在搜尋欄裡面鍵入 "too shy" 
按下Enter 送出搜尋

等到畫面上方分頁欄位跑出 "SONG" 則代表該頁面loading 結束，點擊該分頁。

執行斷言，如果頁面上有 "Too Shy" 則 True。 也就沒事發生。