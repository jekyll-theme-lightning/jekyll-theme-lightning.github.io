---
layout: text
categories: doc
title: 커스텀 스타일과 자바스크립트 추가하기
class: docs-wrapper
order: 4
permalink: /custom-css-and-js
---

라이트닝 테마에 커스텀 스타일과 자바스크립트를 추가할 때, `assets/custom.css`와 `assets/custom.js`를 사용할 수 있습니다.

````sh
└─ assets
    ├─ images
    ├─ custom.css
    └─ custom.js
````

`assets` 폴더는 지킬이 정적 사이트를 생성할 때 사용하는 자산(assets)을 저장하는 폴더입니다. 라이트닝 테마에서는 이 폴더를 이용해 사용자가 레이아웃 파일을 수정하지 않고 간단하게 스타일이나 스크립트를 추가할 수 있는 방법을 제공합니다. 정적 사이트 생성시 `custom.css`와 `custom.js`가 있는지 체크하여 있을 경우에는 해당 파일의 코드를 기본 레이아웃에 적용합니다.
