# Naver Clone Coding
**[네이버](https://www.naver.com/)를 HTML과 CSS만 활용하여 클론 코딩해 보았습니다.**

---

## 1. 프로젝트의 동기
**실제 웹사이트에서 HTML과 CSS가 어떻게 사용되는지에 대한 이해와 효율적으로 클론 코딩을 하는 방법에 대한 학습**

## 2. 프로젝트 진행 과정
**네이버 홈페이지에서 개발자 도구를 이용하여 HTML과 CSS 내용을 확인 후 본 프로젝트에 적용하였다.**

- HTML 내용은 Elements 탭에서 확인할 수 있으며, `<div id ='wrap'>···<div>`태그가 전체화면을 감싸고 있으므로 해당 태그를 가져와 적용하였다.

![1](https://github.com/skagn4929/HTML-basic-project/assets/134206709/9f4a8bfa-e116-488f-9763-9813119ed653)

- CSS 내용을 확인하는 방법 중 Network 탭에서 확인하는 방법을 채택하여 CSS 파일을 체크하였고, 이 중 main.css 파일의 내용이 가장 적합하다고 판단하여 main.css 내용을 가져와 적용하였다.

![2](https://github.com/skagn4929/HTML-basic-project/assets/134206709/fee28a38-9bf9-406b-b60f-98a3b43cebef)

- 웹 브라우저마다 기본적으로 제공하는 CSS 스타일이 조금씩 다른데 이러한 차이 때문에 동일한 웹 페이지가 브라우저마다 다르게 보일 수 있다. 이러한 차이를 [reset.css](https://meyerweb.com/eric/tools/css/reset/)를 사용하면 웹 페이지에 적용하는 스타일이 브라우저마다 동일하게 보이도록 기본 CSS 스타일을 초기화해준다.

- 여기까지 진행하면 아래의 화면처럼 비어있는 배너가 생기는데, 이는 네이버에서 자체적으로 사용하는 nclk_v2라는 함수(또는 모듈)을 본 프로젝트에서는 사용하고 있지 않기 때문에 발생하는 문제이다.

<img width="1440" alt="4" src="https://github.com/skagn4929/HTML-basic-project/assets/134206709/2fb12123-8212-4f28-b972-fbeae5e237ab">

- 본 프로젝트에서는 비어있는 배너의 이미지 파일을 따로 가져와서 적용해 주고, 클릭 시 간단한 confirm 이벤트를 실행시키는 것으로 오버라이딩 하였다.

```html
  <div id="promotion_area" onclick=""
    style="width: 100%;
           height: auto;
           margin: 0px auto;
           line-height: 0;
           height: 100%;"
  ></div>
```
```html
  <script>
    document
      .getElementById('promotion_area')
      .addEventListener('click', function () {
        const isConfirmed = window.confirm('이벤트 페이지 클릭')
        if (isConfirmed) {
          // 사용자가 'OK'를 클릭했을 때의 로직을 여기에 작성
        }
      })
  </script>
```


## 3. 결과물
-  [Naver Homepage Clone](https://skagn4929.github.io/HTML-basic-project/)

![Screenshot 2023-10-04 at 13 36 55](https://github.com/skagn4929/HTML-basic-project/assets/134206709/ca148b3e-5bf7-4992-9dda-afe8b160c12b)
