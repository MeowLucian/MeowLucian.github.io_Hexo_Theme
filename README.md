# MeowLucian.github.io_Hexo_code

My customized Hexo theme source code based on icarus theme.

Hexo 使用教學與客製化主題分享。

# 安裝需求
* [Node.js](https://nodejs.org/en/)
* [Git](https://git-scm.com/)

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

## 外掛
* Json-content : 用於站內搜尋功能
```
npm install -S hexo-generator-json-content
```
* Sitemap : 用於產生網站地圖關鍵字功能
```
npm install hexo-generator-sitemap --save
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

# 產生 Sitemap
* 到根目錄的 `_config.yml` 中的 `# Site` 分類底下添加 :
```
sitemap:
    path: sitemap.xml
```
輸入 [https://localhost:3600/sitemap.xml](https://localhost:3600/sitemap.xml)，查看所產生的 sitemap。

* 完成後同樣將 `# Site` 分類底下 `keywords` 添加關鍵字 :
```
keywords:
```

* 最後別忘了在 Google Search Console 提交剛剛所產生的 Sitemap 資訊 :

![Sitemap](https://drive.google.com/uc?export=download&id=1_sb5S_3vCOVyZUsjcehE0CdRIGossHmW)

# 註解
個人放置網頁的 Repository 上有特殊檔案不會自動產生，請不要刪除或被更新的網頁覆蓋掉
* `README.md` : Github Repository 說明檔案
* `CNAME` : 網站轉址檔案
* `googleccd03104bd8b0cd5.html` : Google Search Console 驗證檔案