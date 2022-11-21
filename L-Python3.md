
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
## for  & if 
```python3

a=[]
for i in range(0,5):
    a.append(i)

a= [ i for i in range(0,5)]

-------

True if len(a)< 1 else False

```



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

- abs(num)  //  절대 값


- from operator import mul
- from functools import reduce
    - reduce(mul,arr)

## `num`
- len(str(num) : 자리수
- list(map(int, str(number))) : 자리수 

---
## set
- 중복을 허용하지 않는다.
- 순서가 없다(Unordered).

----
## String
- sorted(string)  : 정렬 
    - 이걸로 정렬은 가능하나 비교는 안 된다.

---
### enumerate() 함수


                    >>> for entry in enumerate(['A', 'B', 'C']):
                    ...     print(entry)
                    ...
                    (0, 'A')
                    (1, 'B')
                    (2, 'C')

                  >>> for i, letter in enumerate(['A', 'B', 'C']):
                    ...     print(i, letter)
                    ...
                    0 A
                    1 B
                    2 C
                   
                   >>> for i, letter in enumerate(['A', 'B', 'C'], start=1):
                    ...     print(i, letter)
                    ...
                    1 A
                    2 B
                    3 C
                    
----
##  dictionary
dict()

index 와  val 이 있으며 

2중 list와 비슷 


----
### append(x)와 extend(iterable)가 있고 두 함수의 차이점

![](https://mblogthumb-phinf.pstatic.net/MjAxOTA1MTlfNTEg/MDAxNTU4MjI1MjMzNzQ1.vrwM5Kdp03SAYSqqUHk1GHYreCf93CR4QgPXcAFlJ-gg.XL21JskF0EemeEjXwH4eMjX6r-pk9SQcCgInuygX_WMg.PNG.wideeyed/61.png?type=w800)
![](https://mblogthumb-phinf.pstatic.net/MjAxOTA1MTlfMTI0/MDAxNTU4MjI1MjMzNzQ2.Tz9nIxxXFQZtID2B_rhyFCCzDxvwPT5qKcbjWgbZ7Bsg.uX0GSdyXHHqBf-xziMDrrh5WJvKNfNAmCMkF0nTZFlEg.PNG.wideeyed/63.png?type=w800)

                  
