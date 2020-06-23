# 資料準備

## 1.1 &nbsp; 語料檔內容

[點此](/_media/elicitation-sample.docx ":ignore")下載老師提供的轉寫語料檔範例。  
下方為 **1 個句子**的轉寫範例，有兩種支援的格式：

1. **三行** gloss lines (切分、對齊)；**三行** free lines (翻譯及註釋)

    ```
    [編號].
    [族語分析 (aligned)]
    [英文 Glossing (aligned)]
    [中文 Glossing (aligned)]
    [空行]
    #e [英文翻譯]
    #c [中文翻譯]
    #n [註釋]
    [空行]
    ```

	```
	2.
	si-pa-quwas=mu           i      yaya
	CF-VBL-song=1SG.GEN      NOM    mother
	參焦-動化-歌=1SG.屬格      名詞    媽媽
	
	#e I sing for mom.
	#c 我唱歌給媽媽聽。
	#n i 可以省略。
	```


1. **一行**原始族語(未切分)；**三行** gloss lines (切分、對齊)；**三行** free lines (翻譯及註釋)

    ```
    [編號].
    [族語轉寫 (原始)]
    [空行 (optional)]
    [族語分析 (aligned)]
    [英文 Glossing (aligned)]
    [中文 Glossing (aligned)]
    [空行]
    #e [英文翻譯]
    #c [中文翻譯]
    #n [註釋]
    [空行]
    ```

	```
	2.
	sipaquwasmu i yaya

	si-pa-quwas=mu           i      yaya
	CF-VBL-song=1SG.GEN      NOM    mother
	參焦-動化-歌=1SG.屬格      名詞    媽媽
	
	#e I sing for mom.
	#c 我唱歌給媽媽聽。
	#n i 可以省略。
    ```


### 1.1.1 &nbsp; 注意

1. 使用 Word 編輯時，`[編號].` (BTW, 編號後的 **`.`** 是**必須**的) 需獨占一行，且編號請**勿**使用**~~項目符號~~**。
1. 若 gloss lines **一行寫不下**，請依循下方格式換行：

	```
	[族語分析]
    [英文 Glossing]
    [中文 Glossing]
	[空行 (Optional)]
	[族語分析 (接續)]
    [英文 Glossing (接續)]
    [中文 Glossing (接續)]

	15.
	kay lasitu nguavavaeva mucucubungu kilrumay ki sinsilini

	kay   la-situ       ngu-a-va-vaeva   mu-cucubungu  ki-lrumay
	this  PL-student    ngu-RLS-RED-one  go-front      PASS-hit
	這    複數-學生       ngu-實現-重疊-一  去-前面        被-打

	ki   sinsi-lini
	OBL  teacher-3PL.GEN
	斜格  老師-他們的

	#e The students went to the front one by one to be hit by their teacher.
	#c 這些學生一個個到前面被他們的老師打
	```

	其它行，例如第一行未切分的**原始族語**與 **free lines** 請**勿換行**書寫。


## 1.2 &nbsp; 檔案格式

- 檔案類型  
支援的檔案格式有 `.docx` (請**勿**使用 `.doc`) 與 `.txt`。

- 檔名

	1. 檔案名稱的開頭必須是**日期**，且需符合 `yyyymmdd` 的格式。例如，`20200530.docx`, `20200531-liao.docx` 都是符合格式的檔名
	1. 若同一天有兩份以上的語料，可在日期後面直接加入數字 `yyyymmdd##`。例如 `2020053101-liao.docx`, `2020053102-liao.docx`


## 1.3 &nbsp; 將語料更新至 Gloss Search

**Gloss Search** 使用 Google Drive, Travis CI 與 GitHub 來達成線上更新的功能，其運作邏輯如下圖 (不知道這是什麼沒關係)：
![](https://img.yongfu.name/posts/gloss-search-webbased.png ':size=78%')

欲讓自己的語料更新至 **Gloss Search**，需要兩步驟 (即上圖的 `1. Upload` 與 `2. Request data update`)：

1. 將語料檔 (`.docx`/`.txt`) 上傳至**指定的 Google Drive 資料夾** (請詢問老師)
1. 至 [Gloss Search](https://glosss.yongfu.name) 左欄點選 **Data Update** 再輸入 **密碼** (請詢問老師)
	![](./_media/UI-data-update.gif ':size=85%')

