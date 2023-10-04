# Naver-Website-Clone
**HTML과 CSS를 사용하여 네이버 웹사이트 클론을 만들었습니다.**
-  [Naver-Website-Clone](https://skagn4929.github.io/HTML-basic-project/)

![Screenshot 2023-10-04 at 13 36 55](https://github.com/skagn4929/HTML-basic-project/assets/134206709/ca148b3e-5bf7-4992-9dda-afe8b160c12b)

---

## 1. 프로젝트의 동기   
**클론 코딩을 통한 HTML 과 CSS 언어의 학습**

## 2. 프로젝트 주요 내용
**우측 상단 광고 부분 이미지를 실제 네이버 사이트에서 추출하여 적용하였습니다.**

<img width="400" alt="3" src="https://github.com/skagn4929/HTML-basic-project/assets/134206709/38aa212c-57a3-4ed8-a3d8-458a7ec9e2bd">  →  <img width="400" src="https://github.com/skagn4929/HTML-basic-project/assets/134206709/943a01d2-1c45-4dea-ae4d-e3d17addc154">

```html
<div id="pc-main-ad-div-p_main_rollingboard_v1" data-hide-last-sibling="false" style="height: 240px">
  <div style="width: 420px;
              height: 240px;
              margin: 0px auto;
              position: relative;
              line-height: 0;">
    <a href="https://siape.veta.naver.com/fxclick?...생략...;">
      <img src="https://ssl.pstatic.net/melona/libs/1461/1461558/27ac0260c4273494c954_20230829182216631_3.jpg"
                width="100%" height="100%" />  → 부모 태그의 width, height 값이 정해져있으므로, 자식 태그의 width, height 값을 100%로 주게 되면 자동으로 부모 태그의 크기에 맞춰진다.
    </a>
```
