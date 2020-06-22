
# About

This is the user guide for [南島語料搜尋 (Gloss Search)](https://glosss.yongfu.name), a web app for searching interlinear glosses written in Word (`.docx`) or plain text(`.txt`). [Gloss Search](https://glosss.yongfu.name) was created for [Graduate Institute of Linguistics](https://linguistics.ntu.edu.tw) at National Taiwan University to facilitate linguistic fieldwork and documentation of Formosan Languages.


## Features of Gloss Search {docsify-ignore}

- Search glosses with [Regular Expressions](https://en.wikipedia.org/wiki/Regular_expression) or **exact match**
- Restrict search space to specific **files** or **date**
- Link **audio file** to a gloss
- **Copy-paste** plain-text gloss
- **Lexicon** generated from gloss lines *(good for inspecting transcription variations)*


## Table of Contents {docsify-ignore}

1. [資料準備](prepare-data.md)
1. [搜尋模式](search-modes.md)
1. [正規表達式 (RegEx)](regex.md)
1. [進階功能](advanced.md)
    - 後端程式


## Developer's Note {docsify-ignore}

```bash
# Preview locally with
docsify serve ./
```