# **TIL**
>*Today i learned* \
>*2023. 03. 23.*   

1. **Numpy (넘파이)**
- 파이썬에서 행렬 계산이 용이하게끔 도와주는 라이브러리
- 동적 메모리 할당이 아닌 정적 메모리 할당으로 처리함.

2. **넘파이 내장 메소드**

- 행렬 만들기
```python
import numpy as np #넘파이 모듈 불러오기
v1 = np.array([1,2,3,4]) #[대괄호] 안 값으로 행렬 만들기
v1.shape #v1 행렬의 차원, 형태 확인
v1.reshape([2,2]) #v1 행렬을 2x2 행렬로 변환하기

#ex 1. 예시문제
#bmi가 25보다 작은 경우를 구하시오
import numpy as np
heights=[1.83,1.76,1.69,1.86,1.77,1.73]
weights=[86,74,59,95,80,68]

np_heights=np.array(heights)
np_weights=np.array(weights)

bmi=np_weights/(np_heights**2)

print(bmi<25)
```


- 행렬의 곱셈 (내적)
```python
#모두 같은 표현이다.
a.dot(b)
np.dot(a,b)
a@b
```


- 행렬의 곱셈 (내적)
```python
#모두 같은 표현이다.
a.dot(b)
np.dot(a,b)
a@b
```


- 브로드캐스팅(broadcasting) 연상
```python
#하나의 행렬과 스칼라 값들 간 연산이나 행렬과 벡터 간의 연산  
#(broadcasting = 방송국의 전파가 퍼지듯 뒤에 있는 스칼라 값이 모든 요소에 퍼지듯이 연산)


```