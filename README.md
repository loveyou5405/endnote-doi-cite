# Word 論文 EndNote 引用助手

這個 Codex skill 會把 Word 論文括弧內的 DOI 或論文網址，轉成可在 Word 的 EndNote 外掛中編輯的引用。預設依首次出現順序編號，若學校或期刊有指定格式，請一併告知。

## 怎麼用

1. 將包含 `SKILL.md` 和 `references/` 的資料夾放到 Codex 的個人 skills 目錄，資料夾命名為 `endnote-doi-cite`。Windows 通常是 `%USERPROFILE%\.codex\skills\endnote-doi-cite`。
2. 在 Codex 開新對話，提供 Word 檔案與要使用的 EndNote library。
3. 輸入「用 `$endnote-doi-cite` 幫我處理這份 Word 的引用」。

## 引用流程

1. 先另存黃色標記確認版，讓你核對哪些括弧要轉成引用。
2. 收到確認後，核對 PubMed、Crossref 或出版社資料，重用 library 中已有的紀錄，並匯入缺少的文獻。
3. 在另一份 Word 副本插入正式的 EndNote 引用，同一括弧內的多篇文獻會合為一組。
4. 儲存後核對引文位置、文獻識別碼、群組、參考文獻清單及封面和正文文字。

## 支援的括弧內容

- DOI，例如 `(10.3322/caac.21834)`
- DOI 網址，例如 `(https://doi.org/10.3322/caac.21834)`
- PubMed、PMC 或出版社的文章網址
- 同一括弧內的多個 DOI 或論文網址，也支援混用

網址需能核對到特定文章。若網址無法開啟、連到期刊首頁，或 DOI 有疑義，會保留整組黃色標記並列出待確認事項。

這是供 Codex 執行的流程說明。產生可編輯的引文需要 Microsoft Word、EndNote library 和可用的 Cite While You Write 外掛。
