# python

### 실습 예제: 중복된 숫자 제거하기
# 숫자 리스트
arr = [1, 2, 2, 3, 4, 4, 5, 6, 6, 7]  # 중복된 숫자들이 포함된 리스트
result = []  # 중복이 제거된 숫자를 저장할 리스트

# arr 리스트에서 중복 제거하여 result 리스트에 저장
for value in arr:
    if value not in result:  # result 리스트에 없는 숫자만 추가
        result.append(value)

# 결과 출력
print("중복 제거된 리스트:", result)
