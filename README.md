# Golang
Golang!

#import "fmt"

fmt는 입력/출력에 이용된다
예) fmt.Println("")


#함수 선언은 func

func add(x int, y int) int {
  return x+y
}
패러미터 뒤에 타입을 선언, 리턴 타임은 함수 선언부 뒤쪽에 쓴다
func add(x,y int) int 형식으로 묶어서 선언도 가능



#리턴의 두가지 방법

1. func re(a,b int) (int, int){
    return a,b
    }

2. func re(a,b int) (c,d int){
    return
    }
    
리턴도 여러 값을 한번에 return 가능
예) return param1, param2


#변수선언

var a int
var a,b int
var a,b,c = 4, 5, "StringEX"
var (
  a int
  b bool
  c String
)

a := 3 으로 var 생략할 수 있으나 '함수 안에서만 가능'


#기본자료형

bool = true/false
string = 문자열

int / int8 / int16 / int32 / int64

uint / uint8 / uint16 / uint32 / uint64 / uintptr
(비트 길이에 따라)

byte = uint8
rune = uint32
float32 / float64
complex64 / complex 128

묵시적 형 변환이 불가능

디폴트 값은
숫자 : 0
boolean : false
string : ""

상수 선언은 const
var보다 정밀하게 범위를 저장할 수 있음
예) Big_const = 1 << 100


#for문

for i:=0; i<10; i++{
  sum += i
}

#while문처럼 사용 가능

sum := 1
for sum < 1000{
  sum += sum
}
