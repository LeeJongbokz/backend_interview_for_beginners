
# Java 입출력
<br>

-----------------------

### 자바 입출력에서 스트림이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 스트림이란 데이터를 운반하는데 사용되는 연결 통로를 의미합니다. 
</details>

-----------------------

### 자바 입출력에서 스트림의 구성적인 특징은?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 스트림은 먼저 보낸 데이터를 먼저 받는 FIFO 구조로 되어 있습니다. 
</details>

-----------------------

### 입력과 출력을 동시에 수행하려면 어떤 스트림이 필요한가요?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 입력 스트림(Input Stream), 출력 스트림(Output Stream)이 필요합니다. 
</details>

-----------------------

### 자바 입출력에서 스트림은 어떤 단위로 데이터를 전송하나요?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 스트림은 기본적으로 바이트 단위로 데이터를 전송합니다. 이를 바이트 스트림이라고 합니다.<br> 
  바이트 기반이라 함은 입출력의 단위가 1byte라는 뜻입니다.<br>
  ex) InputStream, OutputStream <br>
   
  자바에서는 한 문자를 의미하는 char형이 1byte가 아니라 2byte이기 때문에 <br>
  바이트기반의 스트림으로 2byte인 문자를 처리하는데 어려움이 있습니다. <br>
  따라서 이 점을 보완하기 위해 문자 기반의 스트림이 제공됩니다. <br>
  ex) Reader, Writer <br> 
</details>

-----------------------

### BufferedReader와 BufferedWriter를 사용하는 이유는?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ BufferedReader와 BufferedWriter는 버퍼를 이용해서 입출력 효율을 높일 수 있도록 <br>
  해주는 역할을 합니다. <br>
  버퍼를 이용하면 입출력의 효율이 매우 좋아질 수 있다는 장점이 있습니다.<br> 
  BufferedReader의 readLine()을 사용하면 데이터를 라인 단위로 읽을 수 있습니다. <br> 
</details>

-----------------------

### InputStreamReader와 OutputStreamReader를 사용하는 이유는?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ InputStreamReader와 OutputStreamReader는 바이트 기반 스트림을 문자 스트림으로 연결하는 역할을 합니다. <br>
  그리고 바이트 기반의 스트림의 데이터를 지정된 인코딩의 문자 데이터로 변환합니다. <br> 
</details>

-----------------------

### 직렬화(Serialization)이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 
+ 직렬화란 객체를 데이터 스트림으로 만드는 것을 뜻합니다. <br> 
  다시 얘기하면 객체에 저장된 데이터를 스트림에 쓰기(write)위해 연속적인(serial) 데이터로 변환하는 것을 말합니다. <br>
  반대로 스트림으로부터 데이터를 읽어서 객체를 만드는 것을 역직렬화(Deserialization)이라고 합니다. <br> 
</details>

-----------------------

### 직렬화(Serialization)가 왜 필요한가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 

</details>

-----------------------

### 직렬화(Serialization)의 단점은?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://techblog.woowahan.com/2551/] 

 - 역직렬화시 클래스 구조 변경의 문제가 있습니다. <br> 
   즉, 클래스의 멤버 변수 하나만 추가되어도, java.io.InvalidClassException이 발생합니다. <br> 
   클래스를 변경할 때는 serialVersionUID 값을 관리해주어야 클래스 변경 시 혼란을 줄일 수 있습니다. 
   
   serialVersionUID값이 같더라도, 멤버 변수 명은 같아도 멤버 변수 타입이 바뀌면 문제가 발생할 수 있습니다. 
   이는 primitive type에도 적용되면, 자바 직렬화는 타입에 엄격합니다. 
</details>

-----------------------

### SerialVersionUID란 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: ] 

 - 
</details>

-----------------------

### Blocking이란 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.youtube.com/watch?v=oEIoqGd-Sns] 

 - 자신의 작업을 진행하다가 다른 주체의 작업이 시작되면, <br> 
   다른 작업이 끝날 때까지 기다렸다가 자신의 작업을 시작하는 것을 의미합니다. <br> 
</details>

-----------------------

### Non-Blocking이란 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.youtube.com/watch?v=oEIoqGd-Sns] 

 - 다른 주체의 작업과 상관없이 자신의 작업을 하는 것을 의미합니다. <br> 
</details>

-----------------------

### Synchronous란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.youtube.com/watch?v=oEIoqGd-Sns] 

 - 작업을 동시에 수행하거나, 동시에 끝나거나, 끝나는 동시에 시작함을 의미합니다.  <br> 
</details>

-----------------------

### Asynchronous란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.youtube.com/watch?v=oEIoqGd-Sns] 

 - 시작, 종료가 일치하지 않으며, 끝나는 동시에 시작을 하지 않음을 의미합니다.   <br> 
</details>

-----------------------
