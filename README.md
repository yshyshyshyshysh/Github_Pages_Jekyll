# Deploy and Build Static Webpages with Github Pages

只能部屬靜態網頁 ~ 部落格、實驗室網站、作品集都適合 ~

## Steps <be>

**Step 1. 部屬網頁**

-   建立 public repo，要 public 才可使用 GitHub Pages。若要建立個人網頁應取名為 **`YOURNAME.github.io`**，若要建立專案網頁則直接取名為 **`PROJECTNAME`**，這裡建立的是專案網頁: **`test-Github_Pages`**
-   到該 repo 的 settings 更改成 main branch
-   部屬好了，開啟測試檔案的網址: **`https://yshyshyshyshysh.github.io/test-Github_Pages/test.txt`**

**Step 2. 套用網頁主題**

-   選擇要用的靜態網站產生器（Static Site Generator），由於 2022 年 github 刪除 select theme 的功能，只能改用 Jekyll 來套用現成的主題，或是用其他靜態檔案產生器像是 Hexo / Hugo，他們的語法和資源皆有差異。看了一下覺得 Jekyll 裡的模板比較好看 XD、資源也多，所以這裡用 Jekyll
-   在本地端安裝 Ruby 跟 Jekyll: **`gem install jekyll bundler`**
-   選擇想要的模板，我用 [BlogBox Jekyll Theme](https://jamstackthemes.dev/theme/blogbox-jekyll-theme/)，接著就按照他的說明進行安裝 ~


## References <br>

**About GitHub Pages**
-   [GitHub Pages 相關限制](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits)
-   [建立專案網頁步驟](https://www.youtube.com/watch?v=uegeSwdfWjQ)
-   [建立專案/個人網頁步驟](https://medium.com/%E9%80%B2%E6%93%8A%E7%9A%84-git-git-git/%E5%BE%9E%E9%9B%B6%E9%96%8B%E5%A7%8B-%E7%94%A8github-pages-%E4%B8%8A%E5%82%B3%E9%9D%9C%E6%85%8B%E7%B6%B2%E7%AB%99-fa2ae83e6276)

**About Jekyll Theme**
-   [Jekyll Quickstart](https://jekyllrb.com/docs/)
-   [Jekyll Themes](https://jekyllrb.com/docs/themes/)
-   [用 gem-based method / remote theme method 套用主題](https://ktinglee.github.io/install-github-pages-blog-3/)

