# 進階使用

{docsify-updated}

**Gloss Search** 的後端程式可以在個人電腦上運行。使用這個方式的好處是，在編輯過語料檔後，可以**即時**顯示修正過後的語料。



### Dependencies: Python 3

若電腦沒有 [Python 3](https://www.python.org/downloads/) (3.7 以上)，請先安裝 (可見此[安裝教學](https://lopentu.github.io/PythonForHumanities/slides/week2.html#/))。接著請[下載](https://github.com/liao961120/gloss-search/archive/master.zip)並解壓 `gloss-search-master.zip`。


### run_app.py

直接執行 `gloss-search-master/` 裡的 `run_app.py` 是最簡單的使用方式。在 (第一次) 執行前，請先修改 `run_app.py` 內的**檔案路徑** (至 `server.py` 以及 Word 文件所在之資料夾)。(以 Windows 為例，) 若你將 `gloss-search-master/` 置於**桌面**，且桌面有另一**存放語料檔 (`.docx`) 的資料夾** (`Linguistic_Fieldwork/`)，則要至 `run_app.py` 將其中的這兩行改成這樣 （請修改下方的`<使用者名稱>`）：

```python
SERVER_SCRIPT_PATH = r'C:\Users\<使用者名稱>\Desktop\gloss-search-master\server.py'  # 主程式路徑
DOCX_FOLDER_PATH = r'C:\Users\<使用者名稱>\Desktop\Linguistic_Fieldwork'             # 語料檔資料夾
```

完成此設置後，只要**不更動語料檔資料夾及主程式資料夾位置**，下次在執行此程式時，僅需下方的兩個步驟即可：

1. 開啟 Terminal 執行 `run_app.py` (注意作業系統)

    ```bash
    python run_app.py    # if you're on Windows
    python3 run_app.py   # if you're on Mac
    ```

1. 前往 <https://glosss.yongfu.name> 查詢語料
    
    - 至左欄選擇 `Database > Local`


---

<br>

<details>
<summary><span style="font-size:1rem;font-weight:bold">English Version<span></summary>

### Dependencies: Python 3 {docsify-ignore}

To run this program, [Python 3](https://www.python.org/downloads/) (above 3.7) is required. Yon need to install it if you don't have it on your computer.
Then, download [`gloss-search-master.zip`](https://github.com/liao961120/gloss-search/archive/master.zip) and extract it to a folder (you would need the path to this folder later).

### run_app.py {docsify-ignore}

There is a python script `run_app.py` inside the extracted zip file (`gloss-search-master.zip`). To use this program, you need to execute this script in the terminal. But BEFORE THE FIRST TIME you run this script, you have to edit two lines in `run_app.py` that set the absolute paths to the folder of the docx files and `server.py`, the script essential to this program:

```python
SERVER_SCRIPT_PATH = r'/Users/<username>/Desktop/gloss-search-master/server.py'  # path to gloss-search-master/server.py 
DOCX_FOLDER_PATH = r'/Users/<username>/Desktop/Linguistic_Fieldwork/'            # path to the folder of docx files
```

Suppose you use Mac and `gloss-search-master.zip` is extracted to `gloss-search-master/` on your desktop. Also, you have your interlinear glosses (`.docx` files) saved in another folder, `Linguistic_Fieldwork/`, on your desktop. Then the paths you set in `run_app.py` should look very similar to the above example, except that you have to change `<username>` to that of yours.

After this setup, you can start the program with the steps below (as long as you keep the locations of the folders constant, you won't have to repeat the steps mentioned above the next time you start the program):

1. Open the terminal and execute `run_app.py` with one of the command below (depends on your os):

    ```bash
    python run_app.py    # if you're on Windows
    python3 run_app.py   # if you're on Mac
    ```

1. Visit <https://glosss.yongfu.name> to search the docx files:
    - On the left menu bar, select `Database > Local` to search files on your computer

</details>