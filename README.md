# python

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


