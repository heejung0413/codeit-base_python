<h1> 파이썬: 함수의 추상화 </h1>

<h3> return</h3>

</br>

    def square(x):
    print("함수 시작")
    return x*x
    print("함수 끝")
    
    print(square(3))
    print("hello world")

    #실행결과 
    함수 시작
    9
    hello world

- 즉, return 이후 어떤 코드를 써도 실행되지 않음 ->이런 코드를 데드코드라고 함

<h3> ⭐ return vs print ⭐ </h3>

</br>

    def print_sqaure(x):
        print (x*x)
    
    def return_square(x):
        return x*x


    return_square(3) #아무것도 안나옴 
    print(return_square(3)) #9
    print_sqaure(3) #9
    print(print_sqaure(3)) #9, none

<h3> 옵셔널 파라메타 </h3>

</br> 

    def myself(name, age, nationality="한국"):
    print("내 이름은 {}".format(name))
    print("나이는 {}살".format(age))
    print("국적은 {}".format(nationality))


    myself("코드잇", 1, "미국")  # 옵셔널 파라미터를 제공하는 경우
    print()
    myself("코드잇", 1)  # 옵셔널 파라미터를 제공하지 않는 경우


</br> 

    #결괏값
    내 이름은 코드잇
    나이는 1살
    국적은 미국

    내 이름은 코드잇
    나이는 1살
    국적은 한국

 - 옵셔널 파라메타는 꼭 마지막에 !! 

 <h3> syntactic sugar </h3>

 </br> 

    x=x+1
    x+=1

    x=x*2
    x*=2

    x=x/2
    x/=2


 <h3> scope(범위) </h3>

 </br>

    x=2 #글로벌 변수

    def my_fuction(x):
    x=3  # 로컬 변수
    print(x)

    print(my_fuction(3)) -> 3

- scope은 변수가 가능한 범위
- 로컬변수는 함수내에서만
- 글로벌 변수는 모든 곳에서
- 함수 내의 변수에서는 로컬변수 -> 글로벌 변수를 찾음

<h3> 상수 </h3>

- 절대 변하지 않는 값 
- 상수는 대부분 대문자로 해놓아야 확실히 알 수 없음
상수는 어떤 일이든 바꾸지 않는 변수


</br>
    
    PI=3.14 

    def calculate_area(r):
    return PI *r*r

    radius=4
    print("반지름이 {}면, 넓이는 {}". format(radius, calcurate_area(radius)))