# RegEx 搜尋

{docsify-updated}

**Gloss Search** 的[搜尋模式](search-modes.md)預設使用[正規表達式 (Regular Expression)](https://zh.wikipedia.org/zh-tw/正規表示式)。Regular Expression (簡稱 RegEx) 是一套用來**描述字串規律**的語法。使用 RegEx 能幫助我們大幅提升搜尋語料的效率，對於不了解 RegEx 的使用者，非常建議去學習這套用途廣泛的語法。網路上有相當多的資源，例如 [YouTube 教學](https://www.youtube.com/playlist?list=PL4cUxeGkcC9g6m_6Sld9Q4jzqdqHd2HiD)、[互動式教學](https://regexone.com)、部落格文章等。


**Gloss Search** 用於控制是否為 RegEx 搜尋的按鈕位於網頁右上方，預設為開啟：  
![](_media/UI-regex-btn.png ':size=40%')  
![](_media/UI-regex-btn2.png ':size=40%')


## 3.1 &nbsp; 範例

此使用說明不提供 RegEx 教學 (因為內容不少)，使用者可以多多利用上方提供的學習資源。這邊僅提供在使用 **Gloss Search** 時，非常實用的幾個 RegEx 範例。

1. 搜尋**某文件**的**所有句子**。以 `Kui/2020053101.docx` 為例，可以[限縮搜尋範圍](search-modes?id=docx-filter) 至 `Kui/2020053101.docx`，再輸入**萬用字元** (`.`)
1. 搜尋同**詞根**上的不同**詞綴**。例如，霧台魯凱靜態動詞 (e.g. _**thariri**_ '漂亮') 的兩種可能的前綴 `ka-` 與 `ma-`：

	<details>
	<summary>(RegEx)</summary>

	```regex
	^(ma|ka)thariri$
	```

	- `^`: 字串開頭
	- `$`: 字串結尾
	- `(ma|ka)`: `ma` 或 `ka`
	- `^(ma|ka)`: 以 `ma` 或 `ka` 開頭
	</details>
1. 限縮特定時間範圍。例如，只搜尋**三、五月**的語料，可在 docx filter 輸入：

	<details>
	<summary>(RegEx)</summary>

	```regex
	Kui/20200[356]
	```

	如此，就會搜尋以 `Kui/202003`, `Kui/202005` 開頭的文件路徑，例如：

	- `Kui/20200318.docx`, `Kui/20200325.docx`, `Kui/20200508`, `Kui/20200515`, ...
	</details>

<!-- 
2. Regular Expression
	Match anything `.`
	How to get all gloss in a particular file (. + Docx filter)
	Character set `[]`
		How to search in a specific time range
	Groups `()` + OR `|`
		How to search for diff. affixes on the same stem
 -->
