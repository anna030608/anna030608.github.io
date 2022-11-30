## Build 과정

### Github Page 만들기
1. 나의 github계정에 anna030608.github.io라는 이름으로 repository 만든다.
2. Remote Repository의 주소를 복사한다.
3. Git Bash를 실행시킨다.
4. "git clone <2번에서 복사한 주소 붙여넣기> <내가 저장할 path 넣기>"를 통해 clone 시킨다.
5. "git branch -M main"을 통해 현재 branch 이름을 master에서 main으로 바꾼다.
6. PAT를 만든다.
7. "git push origin main"을 통해 원격저장소에 반영한다.

### Jekyll 사이트 만들기
1. jekyll 윈도우용으로 다운받는다.
2. "cd <지정한 path>"로 내가 지정한 path로 디렉토리를 이동한다.
3. "jekyll -v"를 통해 jekyll 설치 확인 및 버전을 확인한다.
4. "jekyll new . --force"를 통해 현재 디렉토리에 jekyll을 설치한다.
5. "ls"를 통해 새로 생긴 파일이 있는지 확인한다.
6. "git add *"를 해서 새로운 파일 반영한다.
7. "git commit -m "커밋메세지""를 통해 저장한다.
8. "git push origin main"을 통해 원격저장소에 업로드한다.
9. "bundle exec jekyll serve"를 실행한다.
10. 브라우저에 "localhost:4000"에 접속한다.
11. 기본 테마로 된 jekyll 사이트가 생성되었는지 확인한다.

### Post 변경하기
1. _posts 폴더에 "YYYY-MM-DD-TITLE.md" 형태의 새 문서를 생성한다.
2. Markdown 문법에 따라 내용을 작성한다.
3. "git add _posts/YYYY-MM-DD-TITLE.md"를 한다.
4. "git commit -m "커밋메세지""로 커밋한다.
5. "git push origin main"으로 원격저장소에 업로드한다.
6. 변경 내용을 확인한다.

### Theme 입히기
1. "Mr.Green"이라는 jekyll theme를 찾는다.
2. 해당 깃허브 사이트에 들억서 zip파일을 다운받는다.
3. 다운받은 파일을 원래 파일위에 덮어쓴다.
4. "git status"를 하여 추가받을 게 따로 있는지 확인한다.
5. "git add *"를 해서 변경 사항을 반영한다.
6. "git commit -m "커밋메세지""로 커밋한다.
7. "git push origin main"으로 원격저장소에 업로드한다.
8. 테마가 잘 적용되었는지 확인한다.

### 댓글 기능 추가하기
1. "https://disqus.com" 접속한다.
2. 회원가입 및 사이트 정보를 입력한다.
3. "_config.yml"파일에 필요한 내용을 추가한다.
   (나는 "posts.yml", "main.yml", "en.yml"파일을 수정했다.)
4. "git add *"를 해서 변경 사항을 반영한다.
5. "git commit -m "커밋메세지""로 커밋한다.
6. "git push origin main"으로 원격저장소에 업로드한다.
7. 댓글 기능이 추가되었는지, 잘 작동하는지 확인한다.





## Mr. Green Jekyll Theme


---



### Introduction

<!-- outline-start -->

[Mr. Green](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme) is a multilingual theme generated with [Jekyll](https://jekyllrb.com/) and fully compatible with [GitHub Pages](https://pages.github.com/).

<!-- outline-end -->

I was going to make my website and thought if I did it as a template, I could share it with the open source community. That's why I decided to build it as a theme. I've worked so hard to make this possible, so please consider [supporting my work](#you-can-support-my-work). Thanks.

### Features

- Multilingual web site
  - English (default), Japanese, Brazilian Portuguese
- Recommended language offer feature
- Auto Navigation Button adder with icon enable disable options
- Layouts for `Home`, `About`, `Archives`, `Post-list`, `Links`, `Projects` and more
- Color scheme switching options (Dark light)
- Auto Contact option adder
- Auto image referrer (no need to add full path for images. Just add `:` in front of it.)
- image lazy loader, image viewer
- Cool Footer with creative commons licensing
- Movable Table of Contents modal box for Posts
- Post Share Options
- Post-listing by Category or Tags
- Comments for posts
  - [Disqus](https://disqus.com)
- Selectable numbered pagination or scroll to load type
- Sitemap feature
- Search Engine Optimization (SEO)
  - [Schema Markup](https://schema.org)
  - [Open Graph](https://ogp.me/)
  - [Twitter](https://developer.twitter.com/en/docs/twitter-for-websites/cards/overview/summary)
- Analytics (Google Analytics)
- Cookie consent feature
- Site Search feature
- Code Compression for small footprint (`HTML` `JS` `SCSS`)
- Mobile App support
- Mobile device friendly (Tested on Android and IOS)
- Well organized folder structure for developers (Tested on Chrome, Safari, FireFox)

### Installation

#### Github pages

1. [Fork the repo](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/fork).
1. Edit \_config.yml and change `url` like below and push changes.

   ```yaml
   url: "https://your_github_user_name.github.io"
   ```

1. Rename the repo name to `your_github_user_name.github.io`
1. Check Deploy status `Actions` tab on the repo.
1. When it's turned to green, your site is up and running at `https://your_github_user_name.github.io`

#### Local build

1. [Install Jekyll](https://jekyllrb.com/docs/installation/) to your OS
1. Clone or [download](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/releases/latest) the repo, in command prompt go to the folder run `bundle install` command
1. Build using `bundle exec jekyll serve --watch --host 0.0.0.0 --safe` command
    - with `--host 0.0.0.0` parameter you can access web server from same lan.
    - with `--safe` parameter you can make sure no 3rd party plugin added. (for Github pages development)
1. Your page will be up and running at the `0.0.0.0:4000/` address.

### Documentation

Check out [Mr. Green theme tutorials playlist](https://www.youtube.com/playlist?list=PLAymxPbYHgl-fFy5can7uZBMJtFWVcphD) on YouTube

### Credits

I want to thank these projects that gave me an opportunity to build my web site.

- [Jekyll](https://jekyllrb.com/) is a static site generator. It takes text written in your favorite markup language and uses layouts to create a static website. You can tweak the site’s look and feel, URLs, the data displayed on the page, and more. It is a wonderful project which is maintained by volunteers.

- [GitHub Pages](https://pages.github.com/) Hosted directly from your GitHub repository. Just push the changes and the site will be automatically generated.

Some of the sites that I find useful while I'm working on this project. [links page](https://jekyll-theme-mrgreen-demo.mrgreensworkshop.com/tabs/links.html)

### You Can Support My Work

Creating projects starting from nothing takes a great amount of time. Much appreciated if you consider supporting me so that I can continue projects like this and creating new contents for everyone.

- You can support me on [GitHub Sponsors](https://github.com/sponsors/MrGreensWorkshop "Support me on GitHub Sponsors") (monthly or one time)
- You can be one of my patrons on [Patreon](https://patreon.com/MrGreensWorkshop "Be my Patron") (monthly)
- You can tip me via [Ko-fi](https://ko-fi.com/MrGreensWorkshop "Tip Me via Ko-fi") (one time)

### Contribute

Pull Requests are welcome. Please check the instructions in the Issues and Pull Request templates.

### Contributors

Thank you for your contributions!

- Brazilian Portuguese translation by [Vitor DallAcqua](https://github.com/fandangos).

### License

As it says in the [MIT license](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/LICENSE.txt), you can use this theme anywhere as long as you include the license and copyright notice.

`Copyright (c) 2022 Mr. Green's Workshop https://www.MrGreensWorkshop.com`

Please add link to my page or leave the "Pwrd by Mr. Green" link in the footer so I can get credit for my work.

Thank you!

### Other Licenses

Mr. Green Jekyll Theme incorporates libraries written below. Without these libraries, I couldn't make this project possible.

| Library                              | file |
| :----------------------------------- | ---- |
| [jQuery v3.6.0](https://github.com/jquery/jquery/tree/3.6.0), Copyright [OpenJS Foundation](https://openjsf.org) and other contributors. jQuery is distributed under the terms of the MIT License. | [jquery-3.6.0.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/jquery-3.6.0.min.js) |
| [Bootstrap v3.3.7](https://github.com/twbs/bootstrap/tree/v3.3.7), Copyright (c) 2011-2016 Twitter, Inc. Bootstrap is distributed under the terms of the MIT License. | [bootstrap.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/bootstrap.min.js), [bootstrap.min.css](assets/css/bootstrap.min.css) |
| [Bootstrap Table of Contents v0.4.1](https://github.com/afeld/bootstrap-toc/tree/v0.4.1), Copyright (c) 2015 Aidan Feldman Aidan Feldman. Bootstrap Table of Contents is distributed under the terms of the MIT License. | [bootstrap-toc.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/bootstrap-toc.min.js), [bootstrap-toc.min.css](assets/css/bootstrap-toc.min.css) |
| [Font Awesome v4.7.0](https://github.com/FortAwesome/Font-Awesome/tree/v4.7.0), Copyright (c) 2017 Dave Gandy. The Font Awesome font is distributed under the terms of the [SIL OFL 1.1](http://scripts.sil.org/OFL). Font Awesome CSS, LESS, and Sass files are distributed under the terms of the [MIT License](https://opensource.org/licenses/mit-license.html). | [font-awesome.min.css](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/css/font-awesome.min.css), [FontAwesome](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/fonts/) |
| [Lozad.js v1.16.0](https://github.com/ApoorvSaxena/lozad.js/tree/v1.16.0), Copyright (c) 2017 Apoorv Saxena. Lozad.js is distributed under the terms of the MIT License. | [lozad.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/lozad.min.js) |
| [Magnific Popup v1.1.0](https://github.com/dimsemenov/Magnific-Popup/tree/1.1.0), Copyright (c) 2014-2016 Dmitry Semenov, http://dimsemenov.com. Magnific Popup is distributed under the terms of the MIT License. | [jquery.magnific-popup.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/jquery.magnific-popup.min.js), [magnific-popup.css](assets/css/magnific-popup.css) |
| [Simple-Jekyll-Search v1.9.2](https://github.com/christian-fei/Simple-Jekyll-Search/tree/v1.9.2), Copyright (c) 2015 Christian Fei. Simple-Jekyll-Search is distributed under the terms of the MIT License. | [simple-jekyll-search-1.9.2.min.js](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/assets/js/simple-jekyll-search-1.9.2.min.js) |
| [Compress HTML in Jekyll v3.1.0](https://github.com/penibelst/jekyll-compress-html/tree/v3.1.0), Copyright (c) 2014 Anatol Broder. Compress HTML in Jekyll is distributed under the terms of the MIT License. | [compress.liquid](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme/blob/main/_layouts/util/compress.liquid) |

[Mr. Green Jekyll Theme](https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
