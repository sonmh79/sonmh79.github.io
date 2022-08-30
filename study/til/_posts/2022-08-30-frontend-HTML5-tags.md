---
tags: [til, frontend, html5, css]
---

# 220830_frontend_HTML5_tags

### <form>

`<form>` 의 속성값 `GET`, `POST` 방식이 있다.

`GET`은 주소 표시줄에 사용자가 입력한 내용이 표시된다, 길이 제한이 있다 (보안에 취약하다.)

`POST`는 http메시지의 body에 담아서 전송하기 때문에 내용 길이에 제한이 없다.

### <input/>

`<label>`로 `<input>`태그를 감싸면 라벨만 눌러도 입력을 할 수 있다. 특히, `checkbox`같은 `<input>`에 좋다.

`input:checkbox`들의 `name` 속성은 모두 일치시켜줘야 한다. 나중에 `request`에서 `name`으로 식별할 수 있다.

`input:submit`이나 `input:reset`은 자체 기능이 있지만, `<button>`은 자체 기능이 없고 자바스크립트와 연동을 통해 원하는 기능을 구현할 수 있다. 또한, contents를 포함할 수 있기 때문에 아이콘을 추가할 수 있고 CSS를 이용해 원하는 형태로 꾸밀 수 있다.

이중 `submit` 방지 - `form` 태그 속성을 `onclick = false` 를 입력해 한 번의 `submit`은 차단하고 자바스크립트와 연결된 메서드를 실행시킨다.

### <select>

`<select>` 태그에서 `multiple = “multiple”` 속성을 통해 다중 선택이 가능하다.

### <textarea>

`<textarea>` 내부에서 tab을 누르면 그대로 페이지에 적용되니 주의해야 한다.

### <span>

`<span>`은 `inline`태그이기 때문에 스페이스바나 엔터가 있으면 공백이 생길 수 있으니 주의해야 한다.

`<span>`은 좌우 `margin`만 적용된다.

### CSS 적용 순서

CSS는 인라인 > 내부 > 외부 순으로 적용된다.
