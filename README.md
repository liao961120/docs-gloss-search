
# About

 [南島語料搜尋 (Gloss Search)](https://glosss.yongfu.name) 是用於搜尋 [台大語言所](https://linguistics.ntu.edu.tw) [田野調查課程](https://nol2.aca.ntu.edu.tw/nol/coursesearch/print_table.php?course_id=142%20M0210&class=&dpt_code=1420&ser_no=10017&semester=108-2&lang=CH) 所採集的語料的網頁程式。

This is the user guide for [南島語料搜尋 (Gloss Search)](https://glosss.yongfu.name), a web app for searching interlinear glosses written in Word (`.docx`) or plain text(`.txt`). [Gloss Search](https://glosss.yongfu.name) was created for the [Graduate Institute of Linguistics](https://linguistics.ntu.edu.tw) at National Taiwan University to facilitate linguistic fieldwork and documentation of Formosan Languages. It was inspired by [puerdon/corpus_processor](https://github.com/puerdon/corpus_processor), which does roughly the same job as **Gloss Search**, but in a Jupyter Notebook environment.


## Help {docsify-ignore}

若發現文件有不清楚或錯誤的地方，歡迎於該頁最下方**留言**，或直接點選最上方的 ![Edit Document](https://github.githubassets.com/images/icons/emoji/memo.png ':class=emoji') 至 [GitHub](https://github.com) 編輯文件。另外，也歡迎任何有興趣的人一同撰寫此份說明文件 (e.g. 英文版)。


## Features of Gloss Search {docsify-ignore}

- Search glosses with [Regular Expressions](https://en.wikipedia.org/wiki/Regular_expression) or **exact match**
- Restrict search space to specific **files** or **dates**
- Link **audio file** to a gloss
- **Copy-paste** plain-text gloss
- **Lexicon** generated from gloss lines *(could be used for inspecting transcription variations)*

  

## Developer's Notes {docsify-ignore}

```bash
# Preview locally with
docsify serve ./
```
