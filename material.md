# material

## 使用案例對應系統操作

| 使用案例: 個人檔案作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.人員可點擊會員帳號進入個人檔案 | clickPersonal_file(userID) |
| 2.會員登入後，點擊個人檔案 |  |
| 3.人員可預覽該會員的個人檔案 |  |
| 4.點擊個人檔案後可以看到自己的貼文、粉絲、追蹤者 | getInformation(userID) |
| 5.點擊編輯個人檔案可修改個人檔案 | modifyInformation(information) |
| 6.若點擊隱私設定和帳號安全可將帳號設為不公開 | modifySettings(member) |
| 7.若點擊其他會員帳號後可觀看該會員的公開個人檔案 |  |
| 8.系統管理員登入後可看到所有會員帳號 |  |
| 9.點擊會員帳號後可以看到該會員的個人資料 |  |

| 使用案例: 搜尋作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後進入首頁 | onFront_page(account_number) |
| 2.點擊搜尋欄位 | inputUserID(userID) |
| 3.輸入會員id搜尋想找的會員 |  |
| 4.點擊該會員可以查看該會員 |  |
| 5.返回首頁再次點擊搜尋會出現之前的搜尋紀錄 | getRecord(userID) |

| 使用案例: 註冊流程 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.當人員於系統介面，點擊註冊按鈕 | clickSign_up() |
| 2.輸入電子郵件或手機號碼、全名、用戶名稱、密碼 | addUser(email, password, uesrID) |
| 3.若全部輸入正確，可點擊註冊完成註冊 | saveUser(email, password, uesrID) |

| 使用案例: 登入流程 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.進入登入畫面 | clickSign_in() |
| 2.輸入帳號密碼 | inputSign_in(account_number, password) |
| 3.若登入成功則進入首頁 | onFront_page(account_number, password) |

| 使用案例: 基本資料作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後，進入個人檔案 | clickPersonal_file(userID) |
| 2.進入後，可修改姓名、用戶名稱、個人簡介等基本資料 | modifyInformation(information) |
| 3.若姓名、用戶名稱不為空且修改過，則提交即可點擊 |  |
| 4.系統檢查有錯時，將原本資料還原並要求重新輸入 | checkInformationItem(informationItem) |
| 5.按下提交後，更改為新的基本資料 | saveInformation(information) |
| 6.點擊切換為專業帳號 | modifySettings(member) |
| 7.選擇帳號類別，並填入資料 |  |
| 8.系統檢查是否有誤，無誤即可提交 | checkSettingsItem(memberItem) |
| 9.提交後按下完成 | saveNewState(Professional_membership) |

| 使用案例: 追蹤作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入完成後，首頁顯示系統隨機推薦的會員 | autoRandom_user(userID) |
| 2.按下追蹤 | clickTrack(userID) |
| 3.若對方帳號為公開，自己帳號也公開，則直接完成追隨 |  |
| 4.追隨後，對方帳號公開 | ConfirmBoth_parties(personal_file) |
| 5.按下取消在按取消追蹤可取消追蹤 |  |
| 6.取消後對方帳號若為私人則轉為不公開 |  |

| 使用案例: 貼文作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後，點擊貼文 | clickEssay(essay) |
| 2.上傳圖片或影片 |  |
| 3.點擊送出即可建立 | addEssay(essay) |
| 4.若點擊公開會員可觀看該會員的貼文 | getEssay(userID, essay) |
| 5.點擊評論可評論該會員的貼文 |  |
| 6.點擊珍藏可珍藏該會員的貼文 |  |
| 7.點擊分享可分享該會員的貼文 |  |
| 8.點擊個人檔案 | clickPersonal_file(userID) |
| 9.點擊貼文可以看到自己的貼文 |  |
| 10.點擊自己的貼文再按選擇可選擇刪除自己的貼文 | deleteEssay(essay) |
| 11.點擊刪除可刪除自己的貼文 |  |
| 12.若貼文內容不適當，系統管理員可直接刪除該貼文 |  |
| 13.點擊我的珍藏可觀看自己珍藏的貼文 | collectEssay(userID, essay) |

| 使用案例: 限時動態作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後，點擊限時動態 | clickDynamic(time-limited_dynamic) |
| 2.上傳圖片或影片 |  |
| 3.可選擇是否加上文字 |  |
| 4.點擊上傳即可上傳成功 | addDynamic(time-limited_dynamic) |
| 5.點擊該限時動態可刪除 | deleteDynamic(time-limited_dynamic) |
| 6.點擊刪除即可刪除成功 |  |
| 7.若限時動態內容不適當，系統管理員可直接刪除該限時動態 |  |
| 8.點擊其他會員查看限時動態 | getDynamic(userID, time-limited_dynamic) |
| 9.點擊限時動態可查看該會員上傳的限時動態 |  |
| 10.若有限時動態，則可回覆該會員的限時動態 |  |

| 使用案例: 聊天作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後，點擊訊息 | clickMessage(message) |
| 2.點擊或搜尋要發送的會員 |  |
| 3.輸入要傳送的訊息 | inputMessage(userID, message) |
| 4.點擊發送可看到聊天訊息 |  |
| 5.回覆對方的訊息 |  |
| 6.點擊自己發送的訊息 | recoverMessage(message) |
| 7.點擊收回可收回聊天訊息 |  |

| 使用案例: 探索作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.登入後，點擊探索 | clickExplore(userID, Essay) |
| 2.系統顯示其他公開會員的貼文圖片 |  |
| 3.點擊貼文圖片後可使用貼文作業的功能 | getEssay(userID, essay) |

| 使用案例: 通知作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| 1.點擊進入首頁 | onFront_page(account_number) |
| 2.當會員按下追蹤時 | ConfirmBoth_parties(personal_file) |
| 3.系統管理員會發送簡訊到被追蹤的會員裡 |  |
| 4.被追蹤的會員收到通知 | followUser_notice(userID) |

| 使用案例: 會員作業 |  |
| ----- | ----- |
| 主要成功情節 |  |
| (1)1.系統管理員登入後台首頁 | inputBackstage(userID, password) |
| 2.系統管理員於後台搜尋會員的帳號 | inputUserID(userID) |
| 3.選擇成為系統管理員 | modifyPosition(userID) |
| 4.會員身分更換成系統管理員 |  |
| (2)1.系統管理員觀看到同用戶多次違規 | banUser(userID) |
| 2.系統管理員多次警告無用 |  |
| 3.系統管理員封鎖此帳號 |  |
| 4.會員的帳號無法再使用 |  |
