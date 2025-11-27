# 6. 調查技巧：找到故事的「零號病人」

在資訊傳播中，「零號病人」是指消息的最初來源。找到它至關重要，但過程充滿陷阱。如同愛滋病「零號病人」的稱號源於一場誤讀（Patient 'O' 被錯看成 Patient '0'），調查記者也可能因為錯誤的搜尋方法而找錯源頭。

## 核心原則：不要信任網站內建的搜尋引擎

官方網站或資料庫內建的搜尋功能往往不可靠，它們可能無法索引所有內容（特別是PDF或舊文件），讓你誤以為「所見即所得」。

**正確做法：使用通用搜尋引擎進行「外部驗證」**

以美國證券交易委員會 (SEC) 網站為例，其內建搜尋「Dutch police」只能找到一筆2016年的資料。但事實上，最早的紀錄在2004年。

### 搜尋公式：

1.  **基本語法**：在 Google 等搜尋引擎中使用 `site:` 語法，將搜尋範圍限定在特定網站。
    ```
    "Dutch police" site:sec.gov
    ```
2.  **指定資料夾**：如果知道資訊可能位於特定資料夾（例如 `/public` 或 `/press-releases`），可以進一步縮小範圍。
    ```
    "mercer county bar association" site:njcourts.gov/public/
    ```
3.  **預測資料夾名稱**：對於多語言網站，可以嘗試預測英文內容的資料夾，如 `english.` 或 `/en/`。
    ```
    "siemens" site:english.mee.gov.cn
    ```

## 追蹤文件中的線索

有時資訊藏在文件中，而不是網頁上。

- **使用 `filetype:`**：如果你要找的是一份邀請函或報告，它很可能是PDF格式。使用 `filetype:pdf` 來限定搜尋。
- **避免猜測關鍵字**：一份邀請函不一定會寫「邀請函」三個字。與其猜測模糊的詞，不如使用**確定**的資訊，例如活動日期、主辦單位名稱。

### 綜合查詢範例：

要尋找 Friends of Science 於 2014年5月13日舉辦的活動邀請函（PDF格式）：
```
("May 13" OR "May 13th") 2014 filetype:pdf site:friendsofscience.org
```

- **反向搜尋**：若要尋找**其他機構**如何評論某個組織，可以從該組織的網站中排除 (`-site:`)。
    ```
    "friends of science" calgary filetype:pdf -site:friendsofscience.org
    ```