
## `Class`
```python3
class Solution:
    def average(self, salary: List[int]) -> float:
```
#### ` :  `
- salary : List[int]
  - 인자의 tyep을 명시하는 뿐 실제로 다를 수 도 있다.
  - > 인자로 salary 이라는 인자로 들어왔고 list 형태이며  int  type이다

#### ` -> `
- -> float:
  - 해당 함수의 return type을 명시   
  

---
##  `list와 numpy array 차이`

리스트는 숫자형, 문자열 등 모든 자료를 타입을 보존하여 가질 수 있습니다.
- (여러 가지 자료형 허용)

 반면, 넘파이 어레이는 숫자형과 문자열이 섞이면 모두 문자열로 전환됩니다.
 - (한 가지 자료형만 허용)

```python
# 리스트 연산

a = [1, 3, 5]
b = [2, 4, 6]

a + b # [1, 3, 5, 2, 4, 6]

# 허용하지 않음 : a - b, a * b, a / b

a * 3 # [1, 3, 5, 1, 3, 5, 1, 3, 5]

-----
# 넘파이 어레이 연산

a = np.array([1, 3, 5])
b = np.array([2, 4, 6])

a + b # array([ 3,  7, 11])
a * b # array([ 2, 12, 30])

a + 2 # array([3, 5, 7])
a * 3 # array([ 3,  9, 15])
```
## `Array & list`
- sum(arr)
- len(arr)
- max(arr)
- min(arr)
- 
- from operator import mul
- from functools import reduce
    - reduce(mul,arr)

## `num`
- len(str(num) : 자리수
- list(map(int, str(number))) : 자리수 

