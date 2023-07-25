<h1> 파이썬 프로그래밍 시작하기</h1>
<h2> 기본 개념 - 자료형 개요 </h2>

- 숫자열: 정수, 소수
- 문자열: 따옴표 안에 있는 것들

</br>

    2는 숫자열
    "2"는 문자열

-불린: 참과 거짓 

<h2> 기본 개념 - 추상화 개요 </h2>
<h3>변수</h3>

- 값을 저장함
- 복잡한 디테일을 숨기는 용도

</br>

    burger_price=4750
    fries_price=1490

    print(burger_price *2)
    print(burger_price+fries_price)


<h3>함수(Function)</h3>

- 명령 저장
- 예를들어, print() 함수
- 추상화 -> 복잡한 식을 하나의 함수로만 보여주는 것 

</br>

    burger_price=4750

    print(burger_price *2)
    #print()는 파이썬 안의 내장함수

</br>

    #파이썬의 함수 정의
    def hello():
        print("hello")
        print("welcome to codeit")

    #함수 불러오기 
    hello()


<h3>파라미터(parameter)</h3>

- 함수 안의 변수를 정하는 것 

</br>

    def print_sum(a,b):
        print(a+b)

    print_sum(7,3)

<h3>리턴(return)</h3>

- 값을 돌려주는 것

</br>

    예제1
    def get_square(x);
         return x*x

    print(get_square(3))

    #결괏값은 9

    예제2
    def get_square(x);
         return x*x

    y= get_square(3)
    print(y)

    예제3 
    def get_square(x);
         return x*x

    print(get_square(3)+get_square(4))
    #결괏값은 9+16 =25




