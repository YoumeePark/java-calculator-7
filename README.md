# java-calculator-precourse
주요 기능
1. 입력 처리:
Scanner를 사용하여 콘솔로부터 문자열을 입력받습니다.
입력된 문자열은 숫자를 포함하며, 기본 또는 커스텀 구분자로 구분됩니다.

2. 숫자 덧셈 (add 메서드):
문자열이 null이거나 빈 문자열일 경우 0을 반환합니다.
문자열에서 구분자(쉼표(,)와 콜론(:))를 기준으로 숫자를 추출한 후, 각 숫자를 더해 결과를 반환합니다.

3. 기본 구분자 지원 (split 메서드):
기본적으로 쉼표(,)와 콜론(:)을 구분자로 사용하여 숫자를 분리합니다.

4. 커스텀 구분자 지원 (splitWithCustomDelimiter 메서드):
입력이 //로 시작하면, 커스텀 구분자를 사용하여 숫자를 분리합니다.
구분자는 //와 개행 문자(\n) 사이에 정의되며, 구분자를 기준으로 나머지 숫자 부분을 분리합니다.
잘못된 형식의 구분자를 입력할 경우 IllegalArgumentException이 발생합니다.

5. 숫자의 합계 계산 (sum 메서드):
분리된 문자열 배열을 순회하며, 각 요소를 정수로 변환하고 양수만 더합니다.
음수는 허용되지 않으며, 음수가 포함되면 IllegalArgumentException을 발생시킵니다.

6. 숫자 변환 및 예외 처리 (toPositiveInt 메서드):
문자열을 정수로 변환하고, 변환된 값이 음수인 경우 예외를 발생시킵니다.
입력이 숫자가 아닐 경우 IllegalArgumentException을 발생시킵니다.

7. 변수 설명
input: 사용자로부터 입력받은 문자열.
result: 덧셈 계산 결과를 저장하는 변수.
numbers: 구분자를 기준으로 분리된 숫자 문자열 배열.
delimiter: 커스텀 구분자가 있을 경우, 이를 저장하는 변수.
num: 문자열을 정수로 변환한 값.
