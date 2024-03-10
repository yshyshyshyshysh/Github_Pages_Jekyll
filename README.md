# Deploy and Build Static Webpages with Github Pages and Jekyll

-   只能部屬靜態網頁 ~ 部落格、實驗室網站、作品集都適合 ~<br>
-   以下分為[部屬網頁](#部屬網頁)和[套用現成的網頁主題](#套用現成的網頁主題)兩步驟


## 部屬網頁

#### Step 1. 建立 public repo
-   要 public 才可使用 GitHub Pages
-   若要建立個人網頁應取名為 **`YOURNAME.github.io`**
-   若要建立專案網頁則直接取名為 **`PROJECTNAME`**，這裡是建立專案網頁: **`test-Github_Pages`**

#### Step 2. 更改 repo 設定
-   到該 repo 的 settings 更改成 main branch

#### Step 3. 開啟測試網頁
-   部屬好了，隨便新增一個測試用檔案: **`test.txt`**
-   然後開啟該檔案的網址: https://yshyshyshyshysh.github.io/test-Github_Pages_Jekyll/test.txt


## 套用現成的網頁主題

#### Step 1. 選擇要用的靜態網站產生器（Static Site Generator）
-   由於 2022 年 github 刪除 select theme 的功能，只能改用 Jekyll 來套用現成的主題，或是用其他靜態檔案產生器像是 Hexo / Hugo，他們的語法和資源皆有差異
-   看了一下覺得 Jekyll 裡的模板比較好看 XD、資源也多，所以這裡用 Jekyll

#### Step 2. 在本地端安裝 Ruby 跟 Jekyll
-   [RubyInstaller](https://rubyinstaller.org/)
-   執行 **`gem install jekyll bundler`**

#### Step 3. 在本地端安裝想要的網站模板
-   我用 [BlogBox Jekyll Theme](https://jamstackthemes.dev/theme/blogbox-jekyll-theme/)
-   接著就按照他的說明進行安裝:<br> **`bundle config set --local path vendor/bundle`**<br> **`bundle install`**

#### Step 4. 裝好就可以預覽網頁
-   本地端啟動伺服器來預覽整個網站 (這裡使用 Gemfile 中指定的 gem 版本來運行才不會出錯): **`bundle exec jekyll serve --trace`**
-   或是將所有修改同步到 github，透過前面建立好的 Github Pages 的路徑也可以預覽某個分頁: https://yshyshyshyshysh.github.io/test-Github_Pages_Jekyll/index.html

#### Step 5. 撰寫內容
-   將自己的網頁內容建立在 _posts 資料夾下，檔名格式為 **`YYYY-MM-DD-{article_title}.md`**: **`2024-03-10-test.md`**
-   用 Step 4 的方式開啟就可以看到網頁中新加入的內容了 ~


## References

**About GitHub Pages**
-   [GitHub Pages 相關限制](https://docs.github.com/en/pages/getting-started-with-github-pages/about-github-pages#usage-limits)
-   [建立專案網頁步驟](https://www.youtube.com/watch?v=uegeSwdfWjQ)
-   [建立專案/個人網頁步驟](https://medium.com/%E9%80%B2%E6%93%8A%E7%9A%84-git-git-git/%E5%BE%9E%E9%9B%B6%E9%96%8B%E5%A7%8B-%E7%94%A8github-pages-%E4%B8%8A%E5%82%B3%E9%9D%9C%E6%85%8B%E7%B6%B2%E7%AB%99-fa2ae83e6276)

**About Jekyll Theme**
-   [Jekyll Quickstart](https://jekyllrb.com/docs/)
-   [Jekyll Themes 選擇主題](https://jekyllrb.com/docs/themes/)
-   [git clone 方式套用 Jekyll 主題](https://hackmd.io/@CynthiaChuang/Setting-Up-a-GitHub-Pages-Site-with-Jekyll)
-   [用 gem-based method / remote theme method 套用 Jekyll 主題](https://ktinglee.github.io/install-github-pages-blog-3/)

