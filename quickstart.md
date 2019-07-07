---
layout: page
title: 빠르게 시작하기
permalink: /quickstart
class: page-quickstart
navItemTitle: quickstart
---

## 시작하기 전에

이 문서는 포트폴리오 웹사이트를 필요로 하는 창작자가 라이트닝 테마를 이용해 손쉽게 포트폴리오를 구축할 수 있도록 하기 위해 작성했습니다. 라이트닝 테마를 사용하기 위해서는 몇 가지 준비해야할 사항들이 있습니다. 여러분이 창작 활동과 함께 웹 개발을 해왔다면 사전 준비는 그리 어렵지 않습니다. 하지만 웹 개발이 처음이라면, 대부분의 분들이 처음일 거라고 생각합니다만, 라이트닝 테마의 첫 화면을 보기 위해 매우 긴 여정을 떠나야 할지도 모릅니다.

가장 좋은 방법은 주변의 동료와 협력하는 것입니다. 정확히 표현하자면 협력이라기 보다는 도움을 얻는 것에 가깝지만, 여러분도 나중에 그 동료의 다른 일을 도와주면 협력이라고 할 수 있겠죠. 만약 주변에 웹 개발을 할 수 있는 동료가 있다면 이 문서를 공유하세요. 동료와 약속을 잡아서 여러분의 노트북에 몇 가지 프로그램을 설치하고 이상없이 잘 동작하는지 확인하기 위한 아래의 사전 준비 과정을 진행해보세요.

사전 준비를 도와줄 동료가 없어도 너무 걱정하지 않아도 됩니다. 여러분이 보고 있는 이 문서 외에도 [공식 문서](/docs)와 [지원받기/지원하기](/support)를 이용하면 여러분의 포트폴리오 웹사이트를 완성할 수 있을 것입니다.

### 사전 준비

지킬로 빌드한 웹사이트는 정적 웹페이지를 호스팅할 수 있는 서버만 있다면 얼마든지 배포가 가능합니다. 이 문서에서는 지킬을 제작하고 관리하는 깃허브의 깃허브 페이지를 활용해 웹사이트를 만듭니다. 먼저 [깃허브](https://github.com)에 가입해야 합니다.

필요한 프로그램을 CLI 기반과 GUI 기반으로 나누어 설명하겠습니다. 프로그램 설치에 앞서 지킬은 루비 언어로 이루어져 있기 때문에 루비 설치가 필요합니다. 필요한 CLI 프로그램은 지킬과 깃입니다. 라이트닝 테마는 지킬을 기반으로 실행되므로 반드시 지킬이 있어야만 합니다. 또한 깃허브 페이지에 업로드 하기 위해서는 여러분의 컴퓨터에 깃을 설치해야 합니다. 루비와 각 프로그램에 대한 정보는 다음 링크에서 확인 가능합니다.

- 깃: [https://git-scm.com](https://git-scm.com/)
- 루비: [https://www.ruby-lang.org/ko/](https://www.ruby-lang.org/ko/)
- 지킬: [https://jekyllrb-ko.github.io/](https://jekyllrb-ko.github.io/)

GUI 기반의 프로그램은 코드에디터와 이미지에디터, 터미널 에뮬레이터 등이 필요합니다. 깃을 편리하게 이용하기 위해 GUI기반의 깃클라이언트 사용도 고려해볼만 합니다. 이 프로그램들은 어떤 걸 사용해도 무방합니다. 아래는 추천하는 프로그램의 목록이지만, 반드시 아래의 프로그램을 사용해야 하는 것은 아닙니다.

- 코드에디터 - Visual Studio Code: [https://code.visualstudio.com/](https://code.visualstudio.com/)
- 이미지에디터 - PhotoscapeX: [http://x.photoscape.org/](http://x.photoscape.org/)
- 터미널 에뮬레이터 - iTerm2(Windows는 [Git Bash](https://gitforwindows.org/) 사용): [https://www.iterm2.com/](https://www.iterm2.com/)
- 깃클라이언트 - Sourcetree: [https://www.sourcetreeapp.com/](https://www.sourcetreeapp.com/)

루비 언어와 각 프로그램의 설치와 사용 방법은 이 문서에서 설명하지 않겠습니다. 앞서 말씀드린대로 이 사전 준비과정만으로도 긴 여정이 될 수 있습니다. 동료의 이름을 크게 불러보세요.

> 지킬 테마의 "빠르게 시작하기" 문서에서 고리타분하게 깃, 루비, 지킬이 필요하고, 어떤 프로그램을 설치해야하는지까지 설명하고 있느냐고 불만이 있을 수 있습니다. 이 문서의 잠재적인 독자가 지킬을 잘 다루는 웹 개발자가 아니라 웹 개발을 처음 접해보는 사람이라는 점을 감안해서 편하게 읽어주세요.

어떤 방법을 동원했던지 간에 위 프로그램이 모두 준비가 됐다면 프로그램이 잘 설치됐는지 확인합니다. GUI 기반의 프로그램은 아이콘을 눌러 직접 실행해보세요. CLI 프로그램의 설치 상태를 확인하기 위해 터미널 에뮬레이터를 실행해 아래의 명령어를 입력해봅시다.

````sh
$ git --version
git version 2.17.0
$ ruby --version
ruby 2.5.1p57 (2018-03-29 revision 63029) [x86_64-darwin16]
$ jekyll --version
jekyll 3.8.3
````

깃과 루비, 지킬의 버전이 이상없이 출력된다면, 다른 모든 프로그램이 잘 설치됐다고 간주하고 포트폴리오 웹사이트 제작을 시작해봅시다. 버전 숫자는 실행 시점에 따라 조금 다를 수 있습니다.

## 새로운 프로젝트로 시작하기

````sh
$ mkdir YOUR-WEBSITE
$ cd YOUR-WEBSITE
````

필요한 파일 목록입니다.

````sh
├─ LICENSE
├─ README.md
├─ _data
│   ├─ author.yml
│   ├─ navigation.yml
│   └─ settings.yml
├─ _posts
│   ├─ artworks
│   │   ├─ 2018-08-06-ARTWORK-TITLE.md
│   │   └─ 2018-08-06-ANOTHER-ARTWORK-TITLE.md
│   └─ texts
│       ├─ 2018-08-06-TEXT-TITLE.md
│       └─ 2018-08-06-ANOTHER-TEXT-TITLE.md
├─ assets
│   └─ images
│       └─ artworks
│           ├─ ARTWORK-IMAGE.jpg
│           └─ ANOTHER-ARTWORK-IMAGE.jpg
├─ _config.yml
├─ Gemfile
├─ index.md
├─ texts.md
├─ cv.md
└─ .gitignore

````

`Gemfile`

````sh
source "https://rubygems.org"

group :jekyll_plugins do
  gem "jekyll-seo-tag"
  gem "jekyll-feed"
  gem "jekyll-remote-theme"
end

````

`Gemfile`을 작성한 후 `bundle install` 명령으로 실행에 필요한 젬을 설치합니다.

````sh
$ bundle install
Fetching gem metadata from https://rubygems.org/................
Fetching gem metadata from https://rubygems.org/..
Resolving dependencies...
Using public_suffix 3.0.2
Using addressable 2.5.2
Using bundler 1.16.3
Using colorator 1.1.0
Using concurrent-ruby 1.0.5
Using eventmachine 1.2.7
Using http_parser.rb 0.6.0
Using em-websocket 0.5.1
Using ffi 1.9.25
Using forwardable-extended 2.6.0
.
.
.
Using jekyll-remote-theme 0.3.1
Using jekyll-seo-tag 2.5.0
Bundle complete! 3 Gemfile dependencies, 30 gems now installed.
Use `bundle info [gemname]` to see where a bundled gem is installed.

````

`_config.yml`

````yml
title: PORTFOLIO-TITLE
description: PORTFOLIO-DESCRIPTION
permalink: none
remote_theme: jekyll-theme-lightning/lightning
````

`_data/author.yml`

````yml
name: paikwiki
email: paikwiki@gmail.com
description: Geek with the keys
copyright_year: 2018
exhibitions:
  -
    title: Solo Exhibition
    list:
      - 2018 the 2nd Solo Exhibition @Somewhere
      - 2018 the 1st Solo Exhibition @Somewhere
  -
    title: Group Exhibition
    list:
      - 2018 the 2nd Exhibition @Somewhere
      - 2018 the 1st Exhibition @Somewhere

````

`_data/navigation.yml`

````yml
items:
  - title: artwork
    url: /
  - title: text
    url: /texts
  - title: cv
    url: /cv
````

`_data/settings.yml`

````yml
locale: ~
navigation:
  uppercase: true
text:
  showDate: false
footer:
  copyright: ~
````

`index.md`

````md
---
layout: artworks
title: ARTWORK-PAGE-TITLE
item: artwork
permalink: /
navItemTitle: artwork
og:
  title: ARTWORK-PAGE-TITLE
  description: PAGE-DESCRIPTION
  image: ~
  card: summary_large_image
---

````

`texts.md`

````md
---
layout: texts
title: TEXT-PAGE-TITLE
item: text
permalink: /texts
navItemTitle: text
og:
  title: TEXT-PAGE-TITLE
  description: PAGE-DESCRIPTION
  image: ~
  card: summary_large_image
---

````

`cv.md`

````md
---
layout: cv
title: CV
permalink: /cv
navItemTitle: cv
og:
  title: CV - ARTIST-NAME
  description: PAGE-DESCRIPTION
  image: ~
  card: summary_large_image
---

````

`.gitignore`

````sh
Gemfile.lock
_site
.sass-cache

````

## 데모 웹사이트 가져와서 시작하기

데모 웹사이트를 가져와서 시작할 수 있습니다.

```sh
$ git clone DEMO-WEBSITE-GIT-REPOSITORY
$ cd DEMO-WEBSITE
````

다운받은 폴더를 코드에디터에서 열어 수정합니다. 먼저 `_config.yml`에서 웹사이트의 환경세팅을 수정합니다.

 `_data/_settings.yml`에는 라이트닝 테마에 대한 세팅 정보가 있고, `_data/author.yml`에는 창작자의 정보가 있습니다.

`_posts/artworks`에는  `_posts/texts` 폴더 안의 파일을 수정합니다.

작품 이미지는 `assets/images/artworks`와 `assets/images/drawings` 폴더에 있으며 각 폴더 안의 `thumbs` 폴더에 작품의 썸네일 이미지가 있습니다.
