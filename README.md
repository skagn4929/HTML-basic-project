# Naver Homepage Clone
**[네이버](www.naver.com)를 HTML과 CSS만 활용하여 클론 코딩해 보았습니다.**

---

## 1. 프로젝트의 동기
**실제 웹사이트에서 HTML과 CSS가 어떻게 사용되었는지에 대한 이해와 효율적으로 클론 코딩을 하는 방법에 대한 학습**

## 2. 프로젝트 진행 과정
**네이버 홈페이지에서 개발자 도구를 이용하여 HTML과 CSS 내용을 확인 후 프로젝트에 적용한다.**

- HTML 내용은 Elements 탭에서 확인할 수 있으며, `<div id ='wrap'>···<div>`태그가 전체화면을 감싸고 있으므로 해당 태그를 가져와 적용한다.

![1](https://github.com/skagn4929/HTML-basic-project/assets/134206709/9f4a8bfa-e116-488f-9763-9813119ed653)

- CSS 내용은 Network 탭에서 확인할 수 있으며, 보통 main으로 시작하는 파일을 사용하므로 main.css 내용을 가져와 적용한다.

![2](https://github.com/skagn4929/HTML-basic-project/assets/134206709/fee28a38-9bf9-406b-b60f-98a3b43cebef)

- 해당 CSS 파일을 적용하기 전에 기본 브라우저의 CSS 적인 내용의 불일치를 없애기 위해 [reset.css](https://meyerweb.com/eric/tools/css/reset/)를 사용하여 일반화한다.

- 여기까지 진행하면 아래의 화면처럼 하얀 공간이 생기는데, 이 부분은 해당 홈페이지의 <script> 요소를 사용하지 않았기 때문에 발생한다.

<img width="1440" alt="4" src="https://github.com/skagn4929/HTML-basic-project/assets/134206709/2fb12123-8212-4f28-b972-fbeae5e237ab">

- 해당 공간은 `promtion_area`를 따로 만들어 다른 방식으로 적용한다.
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

---

## 3. 결과물
-  [Naver Homepage Clone](https://skagn4929.github.io/HTML-basic-project/)

![Screenshot 2023-10-04 at 13 36 55](https://github.com/skagn4929/HTML-basic-project/assets/134206709/ca148b3e-5bf7-4992-9dda-afe8b160c12b)
