# Start useing VuePress

:::info
VuePress 需要 Node.js >= 8.6
並使用 <font color="blue">Yarn</font> 進行套件管理
:::

1. 建立專案資料夾
    ```
    mkdir vuepress-starter //創建資料夾
    cd vuepress-starter // 進入資料夾
    yarn init //初始化專案
    ```
    ![](https://i.imgur.com/4p9Cyrj.png)
    ###### 設定可以全部用預設 Enter 到底
    
    ```
    yarn add -D vuepress //安裝 vuepress
    ```
    
    在 <font color="#f00">package.json</font> 裡新增
    ```
    "scripts": {
    "dev": "vuepress dev ./",
    "build": "vuepress build ./"
    },
    ```
    最後會長這樣
    
    ![](https://i.imgur.com/4OdK7st.png)


2. 新增第一份文件
    
    在根目錄新增 ```README.md``` 檔案，檔案裡面可以使用 Markdown 的語法
    使用教學參考 [HackMD 使用教學](https://hackmd.io/c/tutorials-tw/%2F%40docs%2Fcustomize-font-color-zh)
    
3. 輸入指令 ```yarn dev``` 讓專案跑起來

    ![](https://i.imgur.com/J2w2Q3R.png)
    ###### 看到這個就是成功 build 起來，可以透過 terminal 給的網址看見專案內容



---

# 頁面與分類

1. 新增一個資料夾 ==news== 
2. 在裡面新增兩個檔案
    ```
     README.md
     test.md
    ```
3. 到網頁上的網址列表輸入 <font color="blue">```http://localhost:8080/news/```</font>
    就會看見在 news 資料夾內 ==```README.md```== 檔案的內容
    
    ![](https://i.imgur.com/VqAVmOh.png)
    
    ![](https://i.imgur.com/FpozQBf.png)
    
    因為 VuePress 預設將資料夾內的 ==```README.md```== 視為根目錄文件
    如果想到看到 test.md 的內容，就只能輸入完整的路徑[http://localhost:8080/news/test.html](http://localhost:8080/news/test.html)
    這個 .html 則是因為 VuePress 將 .md 編譯為 HTML 文件的關係
    
    ![](https://i.imgur.com/i50XaBR.png)

    ![](https://i.imgur.com/6p48HcD.png)

    

    





