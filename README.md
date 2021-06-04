# js-calculator


form을 이용하여 틀(버튼,display)을 만들고

value값을 eval()를 이용하여 문자열을 계산하는 식으로 만들어줬다


검색해보니 eval는 사용하지 않는게 좋다고한다.

eval()은 인자로 받은 코드를 caller의 권한으로 수행하는 위험한 함수<br>
악의적인 영향을 받았을 수 있는 문자열을 eval()로 실행한다면,<br>
해당 웹페이지나 확장 프로그램의 권함으로 사용자의 기기에서 악의적인 코드를 수행하는 결과를 초래<br>
제3자 코드가 eval()이 호출된 위치의 스코프를 볼 수 있으며, 이를 이용해 비슷한 함수인 Function으로는 실현할 수 없는 공격이 가능<br>
최신 JS 엔진에서 여러 코드 구조를 최적화하는 것과 달리 eval()은 JS 인터프리터를 사용해야 하기 때문에 다른 대안들보다 느림<br>
최신 자바스크립트 인터프리터는 코드를 기계 코드로 변환함. 즉, 변수명의 개념이 완전히 사라짐<br>
eval()을 사용하면 브라우저는 기계 코드에 해당 변수가 있는지 확인하고 값을 대입하기 위해 길고 무거운 변수명 검색을 수행해야 함<br>
eval()을 통해 자료형 변경 등 변수에 변화가 일어날 수 있으며, 브라우저는 이에 대응하기 위해 기계 코드를 재작성해야 함<br>

-출처 https://velog.io/@modolee/javascript-eval-is-evil
