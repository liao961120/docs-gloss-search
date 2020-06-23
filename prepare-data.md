# 語料檔準備

{docsify-updated}

## 1.1 &nbsp; 內文格式

[點此](/_media/elicitation-sample.docx ":ignore")下載老師提供的轉寫語料檔範例。  
下方為 **1 個句子**的轉寫範例，支援的兩種格式：

1. **三行** gloss lines (切分且對齊之*族語*、*英文*、*中文*)；**三行** free lines (中英翻譯及註釋)

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


1. **一行**原始族語(未切分)；**三行** gloss lines (切分且對齊之*族語*、*英文*、*中文*)；**三行** free lines (中英翻譯及註釋)

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


### 1.1.1 &nbsp; 音檔嵌入

**Gloss Search** 具有**嵌入音檔**並從**指定時間播放**之功能。欲使用此功能，請先將音檔 (需小於 **100MB**) 上傳至自己的 Google Drive，並取得分享連結 (權限需設為*任何人皆可檢視*)，再於語料檔 free lines 的部份加入一行：

- `#a [Google Drive 分享連結] [該句於錄音檔之開始時間 (hh:mm:ss)]` (見下方實例最後一行)

	```
	19.
	kay lasitu mua cucubungu kilrumay ki sinsi lini

	kay   la-situ    mu-a     cucubungu  ki-lrumay  ki   sinsi     lini
	this  PL-student go-RLS   front      PASS-hit   OBL  teacher   3PL.GEN
	這    複數-學生    去-實現   前面        被-打      斜格  老師       他的

	#e The students went to the front to be hit by their teacher.
	#c 這些學生去前面被他們的老師打
	#n Only 1 RLS marker present when there are multiple verbs in a sentence.
	#a https://drive.google.com/file/d/19_Z0TAciVvfrJmHGE2gAErV_KhXJaQOq 00:35:57
	```

	此句語料在 **Gloss Search** 會被處理成下圖的樣子，其中音檔會直接從 `35分57秒` 開始播放：

	![](./_media/UI-audio-gloss.png ':size=65%')



### 1.1.2 &nbsp; 注意

1. `[編號].`：編號後的 **`.`** 是**必須**的，且 `[編號].` 需獨占一行
1. 使用 Word 編輯時，編號請**勿**使用**~~項目符號~~**
1. Gloss lines 的每個單位**皆**要有內容，若暫時不確定如何分析，請使用**底線** (`_`) 替代：

	```
	si-pa-quwas=mu     i     yaya
	CF-VBL-song=_      NOM   mother
	參焦-動化-歌=_      名詞   媽媽
	```
1. Gloss lines 中的**同一個切分單位**之內**不可以有空白**。若有多重意義，請使用 dot (`.`) 當作連接符號，例如下方的 `good.beautiful`, `好.漂亮`：

	```
	mathariri       kay     akaneane
	good.beautiful  this    food
	好.漂亮          這      食物
	```


1. 若 gloss lines **一行寫不下**，請依循下方格式換行：

	```
	[族語分析]
    [英文 Glossing]
    [中文 Glossing]
	[空行 (Optional)]
	[族語分析 (接續，第二行)]
    [英文 Glossing (接續，第二行)]
    [中文 Glossing (接續，第二行)]
	[空行 (Optional)]
	[族語分析 (接續，第三行，如果還有)]
    [英文 Glossing (接續，第三行，如果還有)]
    [中文 Glossing (接續，第三行，如果還有)]

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


## 1.3 &nbsp; 更新至 Gloss Search

**Gloss Search** 使用 Google Drive, Travis CI 與 GitHub 來達成線上更新的功能，其運作邏輯如下圖 (不知道這是什麼沒關係)：

![](https://img.yongfu.name/posts/gloss-search-webbased.png ':size=68%')

欲將語料更新至 **Gloss Search**，需兩步驟 (即上圖的 `1. Upload` 與 `2. Request data update`)：

1. 將語料檔 (`.docx`/`.txt`) 上傳至**指定的 Google Drive 資料夾** (請詢問老師)
1. 至 [Gloss Search](https://glosss.yongfu.name) 左欄點選 **Data Update** 再輸入 **密碼** (請詢問老師)

	![](./_media/UI-data-update.gif ':size=85%')

	約等待 3-5 分鐘後，語料應已更新在 **Gloss Search**。此時可至左欄點選 **Format Check** 檢查自己的語料格式是否正確

	![](./_media/UI-format-check.gif ':size=85%')