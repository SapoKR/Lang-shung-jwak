```
                                                  @@@%%%%%@@                                        
                                                 @@::...@@@@                                        
                       @@@@                   @@-.....#@@                                           
                      @+::@                  @+.....*@@                               @+@           
                     @#:::@        @@@@****@@@.....=@************@@@@@              @@#:@           
                    @%:::@@   @@@%%.........%@.....@.................%%%%@@@        @:::@           
                    @::::@  @@@..............@.....@.......................@@      @@:::@@          
                   @:::::@@@-................-%....@%.......................--@@   @%::::@          
                  @@:::#@=....................=@***.=..........................=@ @%#%#::@          
                  @::*@*........................................................*@@*@*%@:@          
                 @#+#.............................................................@:#@**@@          
                @@@%...........................::::..............................:@@:@@#@           
                @@:............................:::...........................@@..@*@@:-@@           
               @-.............................::::............................-#.@**#@%=@           
              @+..............................::::............@................+*@****%*@@          
             @*.....................=@*.@.....::::............@.................@@*****%@@@@        
            @%...................--%%...@.....::::............@..................@*****#@%-@        
           @....................@@.......@.....:::............@@.@...............@*****@::@@@       
          @@..................%@-..-%....@......::...........%-@@-................@***@-:@=:=@      
         @@..................@=.....=@*..@........:..........@@==@................@**@=:@+--:@@     
         @.................+@.........+@.++................+@+....@@+++++++.......+%%@:@*:*@::@     
        @#...........=....@@.####@==....@=@..............=@@#..=@##.##@==.@........@@:=@:+@::@@@    
       @@............@....@........%%::..%%@:......@@...@%:%:@%..::%%@:.%@%........@%-@:-@:::@.%@@  
       @:............@....@..@@@@.....@@...@@@...@.:@...:@@@@..@@@...:@..@.........@:@--@:::@@..:@  
     @@-.............@...@...@#.---@#..--##-+@#...##-..#@+@-.#@-....#@-..@.........@#@:@=::#@....-@@
 @@@++.............*@@*..@....+@*....@*.--*---**@*@..*@*----@+..***++....@.........@@::@::*@........
##..........==....=@..@=.@......**@===@@--------+@==##-------##*........@*.........@@+:::@*.........
:::::....%%%%@....@....%%.............--------------------------........@..........@.%%%%...........
::::::::::::@@....@....................------------------------........@...........@................
::::::::::::@%%@--@.......................%@=--%%%%%%-------..........%@..........@::%%...%-@%%:::::
@#:::::::::::::::::@.....................@=.*@==....====@***.........*@..........*@:::+++++:::::::::
 @@++++::::::::::::*@+...................***....@...*............+@*@@+++*......+@:::::::::::::::::+
    @@#::::::::::::::#@=.........................................@::::::@.....==@:::::::::::=@@@@@@ 
  @@%::::::::::::::::::%@::...............................:::@%%%%:::::@....:@@@:::::::::::::@@     
  @@@:::::::::::::::::::::@@@@............................@:::::::::::@@..@@  @@::::::@@@@@@@@      
     @@@@%%%%@@@@@:::::##@   @@@@#####....................@:::####@@@@@@@@@    @@%%%%%@             
                @**@@@@@             @@@@@@@@@@@@@@@@@@@@@@@@@@                                     
                                                                                                    
```
# LANG-SHUNG-JWAK (랭슝좍)

랭슝좍은 트릭컬 리바이브의 리슝좍 밈에서 착안하여, 코드를 짜면서도 비비와 순수를 따잇하는 재미를 느끼기 위해 만들어진 언어입니다. 파이썬으로 구현되어 있습니다.

엄랭 Github에서 아이디어를 얻어 제작했습니다. [[엄랭 Github](https://github.com/rycont/umjunsik-lang)]

문자열 탐색 기반으로 코드가 짜여져 있어 예외 처리가 제대로 되지 않은 곳이 많을 수 있습니다 (오류가 많다는 뜻).

온라인으로 코드 실행할 수 있는 곳 [[여기](https://nabibear33.github.io/jwak/)]

## 개요

이 언어를 만들면서 주로 고려한 부분은 다음과 같습니다.

- 기본적인 프로그래밍 언어의 역할을 할 것.
- 코드를 읽었을 때, 실제 리슝좍이 말하는 듯한 느낌을 줄 것.
- 코드 작성자의 재량에 따라 코드를 각기 다양한 형태로 구현하여 작성자의 풍부한 감정을 드러낼 수 있도록 할 것.

코드 작성 TIP: 코드 작성 시 코드의 내용을 자신이 리슝좍이 된 것처럼 직접 말하면서 작성해 보세요. 좀 더 풍부한 감정을 코드에 담을 수 있습니다.


## 문법

랭슝좍에서 사용하는 키워드는 다음과 같습니다. 줄 단위로 명령어가 정의됩니다.

- 슝, 슈웅, 슈우웅, ...
- 좍, 좌악, 좌아악, ...
- 비비 ... 따잇
- 보호막
- 순수 ... 따잇
- ... 하는 재미 ...
- 에잇
- ,
- ~
- @
- ;
- ㅋ

아울러 표현의 자유도를 높이고 감정을 풍부하게 전달하기 위해 다음의 문자는 묶음 단위의 명령어 사이에 자유롭게 사용할 수 있습니다.
- ?
- !
- .
- " " (공백)

### 교주님

랭슝좍 언어는 반드시 시작 시 '교주님'을 사용합니다.
```python
교주님

# 이후 코드...
```

### 자료형

현재는 정수형만 지원되며, '좍', '좌악', '좌아악', ...을 이용합니다.

```python
좍          # 1
좌악        # 2
좌아악      # 3
좌아아악    # 4
# 이하 '아'가 추가될 때마다 1씩 증가
```

### 연산
자료형-자료형, 변수-변수, 변수-자료형 사이에 사용할 수 있습니다. 덧셈 '~', 뺄셈 ';', 곱셈 ',', 나눗셈 '@'을 이용합니다. 표현의 자유도를 높이기 위해 동일한 연산자를 연속하여 사용하는 것이 가능합니다 (예제 코드 두번째 줄 참고). 연산은 우선 순위 없이 무조건 왼쪽부터 진행됩니다.
```python
좍~좍           # 1+1
좍~~~~~~~~~~좍  # 1+1, '좍~좍'과 동일
좌악,좌아악     # 2x3
슝;좌아악       # 첫번째 변수에 저장된 값 - 3
슈웅;슈우웅@좍  # (두번째 변수에 저장된 값 - 세번째 변수에 저장된 값) / 1
```


### 변수 선언

문장의 맨 앞에 '슝', '슈웅', '슈우웅', ...을 사용하여 변수를 선언합니다. 기본적으로 0의 값으로 초기화되어 있습니다. 변수 선언시에는 다른 변수를 대입하거나 정수형 자료형을 이용하여 값을 저장해야 합니다. 아무 값도 넣지 않는 경우 0을 대입합니다.
```python
슝                      # 첫번째 변수에 0을 대입.
슝좍                    # 첫번째 변수에 1을 대입.
슝...?좍!!!            # 첫번째 변수에 1을 대입. (.?!를 적절히 배치)
슈웅좌아악,좌악,좌악     # 두번째 변수에 3x2x2=12를 대입.
슈우웅슈웅~슝           # 세번째 변수에 두번째 변수의 값 + 첫번째 변수의 값 = 7을 대입.
```


### 출력
#### 변수에 저장된 값에 해당하는 ASCII 코드값을 출력하고 싶은 경우
'비비따잇'으로 문장을 시작합니다. '따잇'은 '따따잇', '따따따잇'과 같이 '잇' 앞에 붙는 '따'의 개수를 자유롭게 변경할 수 있습니다. 이후 'ㅋ'의 개수를 이용하여 변수에 저장된 값을 출력합니다. 'ㅋ'의 개수가 n인 경우 n번째 변수의 값을 출력하게 됩니다. 'ㅋ'의 위치는 자유롭게 둘 수 있습니다. 단, '비ㅋ비', '따ㅋ잇'과 같이 각 단어의 사이에 위치해서는 안됩니다.
```python
비비따잇          # SyntaxError
비비따잇ㅋㅋ      # 두 번째 변수의 값 출력
비비ㅋ따따잇ㅋ    # 두 번째 변수의 값 출력
비비ㅋㅋㅋ따잇    # 세 번째 변수의 값 출력
비ㅋㅋ비따잇      # SyntaxError
비비따ㅋㅋㅋ잇    # SyntaxError
```
#### 변수에 저장된 값을 출력하고 싶은 경우
중간에 '보호막'을 추가합니다. 나머지 부분은 위와 동일합니다.
```python
비비보호막따잇        # SyntaxError
비비보호막따잇ㅋㅋ    # 두 번째 변수의 값 출력
비비ㅋ보호막따잇ㅋ    # 두 번째 변수의 값 출력
비비보호막ㅋㅋㅋ따잇  # 세 번째 변수의 값 출력
```

### 입력
'순수따잇'으로 문장을 시작합니다. '따잇'은 '따따잇', '따따따잇'과 같이 '잇' 앞에 붙는 '따'의 개수를 자유롭게 변경할 수 있습니다. 이후 'ㅋ'의 개수를 이용하여 입력한 값을 몇번째 변수에 저장할지 지정합니다. 'ㅋ'의 개수가 n인 경우 n번째 변수에 입력값을 저장합니다. 'ㅋ'의 위치는 자유롭게 둘 수 있습니다. 단, '순ㅋ수', '따ㅋ잇'과 같이 각 단어의 사이에 위치해서는 안됩니다.
```python
순수따잇          # SyntaxError
순수따따잇ㅋㅋ    # 입력된 값을 두 번째 변수에 저장
순ㅋㅋ수따잇      # SyntaxError
순수따ㅋㅋㅋ잇    # SyntaxError
```

### If문
{명령어} + '하는재미' + {조건}으로 구성됩니다. 만약 {조건}의 값이 0인 경우, {명령어}가 실행됩니다. {조건}이 빈 경우에도 {명령어}가 실행됩니다. {조건}의 값이 0이 아닌 경우 {명령어}는 실행되지 않습니다.
```python
비비따잇하는재미슝  # 첫 번째 변수의 값이 0이면 첫 번째 변수의 값 출력
```

### Goto문
'에잇'으로 문장을 시작합니다. 'ㅋ'의 개수가 이동하는 line 수를 의미합니다. '에잇'이 한번 사용된 경우 위로 이동하고, 두번 사용된 경우 아래로 이동합니다.
```python
에잇ㅋ            # 1줄 위로 이동
에잇에잇ㅋㅋㅋㅋ  # 4줄 아래로 이동
```


## Hello, world! 예제

다음의 예제를 통해 랭슝좍을 더욱 효과적으로 즐기는 방법을 알아보세요.
다음은 "Hello, world!"를 출력하는 기본 코드입니다.

```
교주님

슝좍,좌아아아아아아아악,좌아아아아아아악
슈웅좌아아아아아아아아악
슈우웅좍,좌아아악,슈웅~좌아아악
슈우우웅슈웅,슈웅~좌아아아아아아악
슈우우우웅좍~좍~슈웅,슈웅;좍
슈우우우우웅좍~슈웅,슈웅~좍 
슈우우우우우웅좌아아아아악,좌아아아아악;좌아아악
슈우우우우우우웅좍~슈웅,슈웅~슈웅;좌아아아아악
슈우우우우우우우웅슈웅,슈웅~좍
슈우우우우우우우우웅슈웅,슈웅
슈우우우우우우우우우웅슈웅~좍,좌아악

비비따잇
비비따잇ㅋㅋㅋㅋㅋㅋㅋㅋ
비비따잇ㅋㅋㅋ
비비따잇ㅋㅋㅋ
비비따잇ㅋㅋㅋㅋㅋ
비비따잇ㅋㅋ
비비따잇ㅋㅋㅋㅋㅋㅋ
비비따잇ㅋㅋㅋㅋ
비비따잇ㅋㅋㅋㅋㅋ
비비따잇ㅋㅋㅋㅋㅋㅋㅋ
비비따잇ㅋㅋㅋ
비비따잇ㅋㅋㅋㅋㅋㅋㅋㅋㅋ
비비따잇ㅋㅋㅋㅋㅋㅋㅋㅋㅋㅋ
```

기본 코드에서 'ㅋ', '!', '?', '.'과 공백을 적절히 배치하여 리슝좍이 실제로 말하는 듯한 코드를 작성해보세요.

```
교주님

슝좍?, 좌아아아아아아아악,... 좌아아아아아아악!!!!!
슈웅... 좌아아아아아아아아악!!
슈우웅좍???, 좌아아악,....!! 슈웅~ 좌아아악!
슈우우웅!! 슈웅, 슈웅?!~ 좌아아아아아아악????!!!
슈우우우웅.. 좍~좍~! 슈웅, 슈웅;;; 좍??
슈우우우우웅좍~... 슈웅!!, 슈웅~~~ 좍?! 
슈우우우우우웅...좌아아아아악!!!, 좌아아아아악;;;?!! 좌아아악!!
슈우우우우우우웅좍~!! 슈웅, 슈웅~~ 슈웅;;;?? 좌아아아아악!
슈우우우우우우우웅! 슈웅, 슈웅~ 좍!
슈우우우우우우우우웅... 슈웅, 슈웅!
슈우우우우우우우우우웅... 슈웅~ 좍!, 좌아악!

비비 따잇!?
비비 따잇ㅋㅋㅋㅋㅋㅋㅋㅋ
비비....ㅋㅋ 따잇!!ㅋ
비비 따잇ㅋㅋㅋ!!
비비ㅋㅋㅋㅋㅋ 따잇!!
비비ㅋㅋ 따잇?
비비ㅋ 따잇ㅋㅋㅋㅋㅋ
비비ㅋㅋㅋㅋ 따잇
비비?? 따잇ㅋㅋㅋㅋㅋ!!
비비ㅋㅋㅋ 따잇ㅋㅋㅋㅋ
비비 따잇ㅋㅋㅋ
비비 따잇ㅋㅋㅋㅋㅋㅋㅋㅋㅋ
비비ㅋㅋㅋㅋㅋㅋㅋ 따잇ㅋㅋㅋ!!!
```

출력
```python
Hello, world!
```

## 오류 예제

### 문법 오류

문법에 맞지 않게 코드가 작성된 경우 SyntaxError를 출력합니다.

예제 코드
```python
이건.. 다야님의 알..?? 에잇! 에잇!ㅋㅋㅋㅋ
```
출력
```
>> SyntaxError: 어떻게 이게 리슝좍이냐!
```

### 무한 루프

컴파일하는 line이 1백만 개가 넘어가면 무한 루프로 판단하여 RecursionError를 출력합니다.

예제 코드
```python
교주님

슝??????




에잇! 에잇!ㅋㅋㅋ
```
출력
```
>> RecursionError: Line 6에서 타임 패러독스!
```

## 로컬 실행

1. 깃허브 파일을 다운받고 압축을 풀어주세요.
2. 터미널을 열고 루트 폴더에서 다음 명령어를 실행하세요.
```bash
python -m jwak .\example\hello_world.jwak
```