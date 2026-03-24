##index.html

1) <link rel="stylesheet" href="style.css">
- 스타일 시트 불러오기

2) <input id="display" readonly>
- 사용자에게 입력 받음/ 읽기 전용

3) <button onclick="appendToDisplay('+')" class="operator-btn">+</button>
- onclick = 클릭 이벤트
- appendToDisplay('+') = 함수 호출

4) <script src = "index.js"></script>
- <script></script> = 자바스크립트 실행 태그


---

##index.js

1) const display = document.getElementById("display");
- HTML에서 id="display"인 요소를 display라는 변수에 저장

2) function appendToDisplay(input){
- 함수 선언

3) display.value += input;
- 현재 값 뒤에 input 붙이기

4) function clearDisplay(){
     display.value = "";
- C 버튼 함수 (초기화)

5) function calculate(){
- = 버튼 함수 (계산 실행)

6) try {
      display.value = eval(display.value);
- 에러 날 수도 있는 코드 실행 시도
- display.main = "1+2*3" 같은 문자열
- **eval()** = 문자열을 진짜 계산식으로 실행

7) catch {
      display.value = "Error";
- 에러 발생 시 "Error" 출력
