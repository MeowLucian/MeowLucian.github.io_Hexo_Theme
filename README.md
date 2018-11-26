# MeowLucian.github.io_Hexo_code

My customized Hexo theme source code based on icarus theme.

Hexo 使用教學與客製化主題分享。

# 安裝需求
* [Node.js](https://nodejs.org/en/)
* [Git](https://git-scm.com/)

# 安裝
## Hexo
```
npm install -g hexo-cli
```
## 建立 Hexo 基本檔案
```
hexo init <folder>
cd <folder>
npm install
```
## icarus 主題
* 預設主題
```
git clone https://github.com/ppoffice/hexo-theme-icarus.git themes/icarus
```
* 客製化主題
```
git clone https://github.com/MeowLucian/MeowLucian.github.io_Hexo_Theme.git themes/icarus
```

## Json-content 外掛
用於站內搜尋功能
```
npm install -S hexo-generator-json-content
```

# 設定
## 主題
編輯根目錄下的 `_config.yml`
```
theme: icarus
```
## 文章封面圖
7:3 比例呈現
## 網址連結
編輯根目錄下的 `_config.yml`
* Github Page 發佈 :
```
url: https://<yourname>.github.io
```
* 正式發佈 :
```
url: http://brain-garden.tw/
```
# 執行指令
## 產生 about 頁面
```
hexo new page about
```
## 使用 Hexo 產生靜態檔案
```
hexo g
```
## 開啟 Server
```
hexo s -p 3600
```
`-p` : 連接埠設定
## 瀏覽網頁
* [http://localhost:3600/](http://localhost:3600/)

# 上傳到 Github
複製 `public` 資料夾裡的內容，建立 Commit 並 Push 到 Github 上的 Repository