# MeowLucian.github.io_Hexo_code
My customized Hexo theme source code based on miho theme

## 一、安裝需求
* [Node.js](https://nodejs.org/en/)
* [Git](https://git-scm.com/)

## 二、安裝 
### 2.1 Hexo
```
npm install -g hexo-cli
```
### 2.2 建立 Hexo 基本檔案
```
hexo init <folder>
cd <folder>
npm install
```
### 2.3 miho 主題
```
git clone https://github.com/WongMinHo/hexo-theme-miho.git themes/miho
```
### 2.4 Json-content 外掛
用於站內搜尋功能
```
npm install hexo-generator-json-content --save
```

## 三、設定
### 3.1 主題
編輯根目錄下的 `_config.yml`
```
theme: miho
```
### 3.2 文章封面圖
7:3 比例呈現
### 3.3 網址連結
編輯根目錄下的 `_config.yml`
* 內網測試 :
```
url: http://localhost:3600/
```
* 正式發佈 :
```
url: https://<yourname>.github.io
```
## 四、Hexo 執行指令
### 4.1 產生 about 頁面
```
hexo new page about
```
### 4.2 使用 Hexo 產生靜態檔案
```
hexo g
```
### 4.3 開啟 Server
```
hexo s -p 3600
```
`-p` : 連接埠設定
### 4.4 瀏覽網頁
* [http://localhost:3600/](http://localhost:3600/)

## 五、上傳到 Github
複製 `public` 資料夾裡的內容，建立 Commit 並 Push 到 Github 上的 Repository
