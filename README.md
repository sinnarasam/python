# python

https://docs.python.org/3.9/library/

https://pandas.pydata.org/docs/reference/index.html

# 실습 예제: 중복된 숫자 제거하기

	# 숫자 리스트
	arr = [1, 2, 2, 3, 4, 4, 5, 6, 6, 7]  # 중복된 숫자들이 포함된 리스트
	result = []  # 중복이 제거된 숫자를 저장할 리스트
	
	# arr 리스트에서 중복 제거하여 result 리스트에 저장
	for value in arr:
	    if value not in result:  # result 리스트에 없는 숫자만 추가
	        result.append(value)
	
	# 결과 출력
	print("중복 제거된 리스트:", result)

# 파이썬에서의 object 타입
	x = "Hello"  # 문자열은 객체
	y = 123  # 정수도 객체
	z = [1, 2, 3]  # 리스트 역시 객체

이 모든 변수들은 사실 object 클래스에서 파생된 객체입니다. 그래서 파이썬에서 object는 모든 데이터 타입의 기반이 됩니다.

	import pandas as pd
	
	data = {
	    '이름': ['Alice', 'Bob', 'Charlie'],
	    '나이': [25, 30, 35]
	}
	
	df = pd.DataFrame(data)
	
	print(df.dtypes)


# 숫자 출력

# 1부터 5까지 숫자를 출력, 각 숫자는 ', '로 구분
	# 1부터 5까지 숫자를 출력, 각 숫자는 ', '로 구분
	for i in range(1, 6):
	    print(i, end=', ')
# 리스트의 각 항목을 출력
	# 리스트의 각 항목을 출력
	fruits = ['apple', 'banana', 'cherry', 'date']
	for fruit in fruits:
	    print(fruit, end=', ')
# 1부터 10까지의 숫자 중에서 짝수만 출력
	# 1부터 10까지의 숫자 중에서 짝수만 출력
	for i in range(1, 11):
	    if i % 2 == 0:
	        print(i, end=', ')
# 리스트의 갯수에 따라 반복 해서 리스트의 값 출력
	numbers = [10, 20, 30, 40, 50]
	for i in range(len(numbers)):
	    if i == len(numbers) - 1:
	        print(numbers[i], end='')  # 마지막 항목에선 콤마 생략
	    else:
	        print(numbers[i], end=', ')
# 문자열의 각 문자를 출력
	# 문자열의 각 문자를 출력
	text = "hello"
	for char in text:
	    print(char, end=', ')


# Pandas 행,열 선택 방법
	data.iloc[0] # data의 첫번째 행만
	data.iloc[1] # 두번째 행만
	data.iloc[-1] # 마지막 행만
	# Columns:
	data.iloc[:,0] # 첫번째 열만
	data.iloc[:,1] # 두번째 열만
	data.iloc[:,-1] # 마지막 열만


