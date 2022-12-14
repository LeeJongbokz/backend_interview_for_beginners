# OS

### 인터럽트란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>

[참고: 운영체제]

+ 사건이 발생하면 하드웨어나 소프트웨어로부터 발생한 인터럽트에 의해 신호가 보내어집니다. <br> 
  하드웨어는 어느 순간이든 시스템 버스를 통해 CPU에 신호를 보내 인터럽트를 발생시킬 수 있습니다. <br> 
  
  소프트웨어는 시스템 호출이라 불리는 특별한 연산을 실행하여 인터럽트를 발생시킬 수 있습니다. <br> 
  
  CPU가 인터럽트 되면, CPU는 하던 일을 중단하고, 즉시 고정된 위치로 실행을 옮깁니다. <br> 
  이러한 고정된 위치는 일반적으로 인터럽트를 위한 서비스 루틴이 위치한 시작주소를 가지고  있습니다. <br> 
  그리고 인터럽트 서비스 루틴이 실행됩니다. <br> 
   
  인터럽트 서비스 루틴의 실행이 완료되면, CPU는 인터럽트 되었던 연산을 재개합니다. <br> 
  이러한 연산의 시간 일정(time line)이 그림 1.3에 있습니다. <br>
   
  인터럽트는 컴퓨터 구조의 중요한 부분입니다. <br> 
  각 컴퓨터 설계는 자신의 인터럽트 메커니즘을 가지고 있으며, 몇 가지 기능은 공통적입니다. <br> 
  인터럽트는 적절한 서비스 루틴으로 제어를 전달합니다. <br> 
  이러한 전달을 처리하는 직선적인 방법은 인터럽트 정보를 조사하는 일반적인 루틴을 호출하는 방법입니다. <br> 
  이 루틴은 이어 인터럽트 고유의 핸들러(handler)를 호출합니다. <br> 
   
  
</details>

-----------------------

### 저장 장치 구조란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>

[참고: 운영체제]

+ CPU는 명령어를 단지 메모리로부터 가져올 수 있으므로, 프로그램을 수행하려면 프로그램이 반드시 메모리에 있어야 합니다. <br> 
  범용 컴퓨터는 대부분의 프로그램을 주 메모리(Random-Access Memory)라 불리는 재기록 가능한 메모리에서 가져옵니다. <br> 
  주 메모리는 Dynamic Random-Access Memory(DRAM)라 불리는 반도체 기술로 구현됩니다. <br> 
   
  컴퓨터는 다른 형태의 메모리도 사용합니다. 우리는 이미 읽기 전용 메모리인 ROM과 전기적으로 소거 가능한 <br> 
  프로그램 가능-읽기 전용 메모리 EEPROM을 살펴 보았습니다. <br> 
  ROM은 변경할 수 없으므로 앞에 설명한 부트스트랩 프로그램과 같은 정적 프로그램을 저장합니다. <br> 
   
  ROM의 이러한 불변성은 게임 카트리지에 유용합니다. EEPROM은 변경할 수는 있으나 자주 변경할 수 없으며 <br>
  따라서 대부분 정적 프로그램을 저장하고 있습니다. <br> 
  예를 들면, 스마트폰은 공장에서 설치한 프로그램을 저장하기 위해 EEPROM을 사용합니다. <br>
   
  모든 형태의 메모리는 바이트의 배열을 제공합니다. 각 바이트는 자신의 주소를 가지고 있습니다. <br> 
  상호 작용은 특정 메모리 주소들에 대한 일련의 적재(load) 또는 저장(store) 명령을 통하여 이루어집니다. <br> 
  
  적재 명령은 주 메모리로부터 CPU 내부의 레지스터로 한 바이트 또는 한 워드를 옮기는 것입니다. <br> 
  반대로 저장 명령은 레지스터의 내용을 주 메모리로 옮깁니다. <br> 
  명시적인 적재, 저장 명령 외에, CPU는 실행을 위해 자동적으로 주 메모리로부터 명령을 적재합니다. <br> 
  
</details>

-----------------------

### 프로세스란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 

+ 비공식적으로, 프로세스란 실행중인 프로그램입니다.  <br>
  프로세스는 때로는 텍스트 섹션으로 알려진 프로그램 코드 이상의 무엇입니다. <br> 
  프로세스는 또한 프로그램 카운터의 값과 처리기 레지스터의 내용으로 대표되는 현재 활동을 포함합니다. <br> 
  
  프로세스는 일반적으로 함수의 매개변수, 복귀 주소와 로컬 변수와 같은 임시적인 자료를 가지는 프로세스 스택과 <br>
  전역 변수들을 수록하는 데이터 섹션을 포함합니다. <br> 
  또한, 프로세스는 프로세스 실행 중에 동적으로할당되는 메모리인 힙을 포함합니다. <br>
   
  우리는 프로그램 그 자체는 프로세스가 아님을 강조합니다. <br> 
  프로그램은 명령어 리스트를 내용으로 가진 디스크에 저장된 파일(실행 파일이라고 불림)과 같은 수동적인 존재(passive entity)입니다. <br>
  이와는 대조적으로 프로세스는 다음에 실행할 명령어를 지정하는 프로그램 카운터와 <br> 
  관련된 자원의 집합을 가진 능동적인 존재(active entity)입니다. <br> 
   
  실행 파일이 메모리에 적재될 때, 프로그램은 프로세스가 됩니다. <br> 
  실행 파일을 메모리에 적재하는 일반적인 두 가지 방식은 실행 파일을 나타내는 아이콘을 더블 클릭하는 방식과 <br> 
  명령어 라인 상에서 prog.exe 또는 a.out과 같이 파일 이름을 입력하는 방식입니다. <br> 
</details>


-----------------------


### 프로세스 스케줄링이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 

+ 다중 프로그래밍의 목적은 CPU 이용을 최대화하기 위하여 항상 어떤 프로세스가 실행되도록 하는데 있습니다. <br> 
  시분할의 목적은 각 프로그램이 실행되는 동안 사용자가 상호 작용할 수 있도록 프로세스들 사이에서 CPU를 빈번하게 교체하는 것입니다. <br> 
  
  이 목적을 달성하기 위해 프로세스 스케줄러는 CPU에서 실행가능한 여러 프로세스들 중에서 하나의 프로세스를 선택합니다. <br> 
  단일 처리기 시스템에서는 실행 중인 프로세스가 한 개 이상일 수 없습니다. <br> 
  
  만일 프로세스들이 여러 개 있다면, 나머지 프로세스들은 CPU가 자유로워 다시 스케줄 될 때까지 대기해야만 합니다. <br> 
</details>


-----------------------


### LRU 알고리즘이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 페이지 교체 알고리즘의 한 종류로서, 가장 오랜 기간 사용되지 않은 페이지를 교체하는 알고리즘입니다. <br> 
   
</details>


-----------------------

### 프로세스와 스레드의 차이점은?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 프로세스는 실행중인 프로그램을 의미하며, 메모리를 할당 받은 프로그램을 의미합니다. <br>
  스레드는 프로세스의 하위 개념으로서, 하나의 프로세스는 다수의 실행 스레드를 가질 수 있으며, <br>
  실제 코드를 실행하는 단위입니다. 
  스레드는 프로세스보다 생성 비용이 저렴하며, 여러 스레드는 힙(heap)이라는 메모리 공간을 공유합니다. 
   
</details>


-----------------------


### 멀티 프로세스 대신 멀티 스레드를 사용하는 이유는?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 멀티 스레드 방식은 멀티 프로세스 방식에 비해 생성 비용(메모리 공간)이 저렴하며, context switch 비용이 적습니다. <br>
  또한 캐싱 측면에서도 스레드 모델의 성능이 더 좋습니다.  
   
   
</details>


-----------------------

### 임계 구역(Critical Section)이란? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 임계 구역은 다른 프로세스와 공유하는 변수를 변경하거나, 테이블을 갱신하거나 파일을 쓰거나 하는 등의 작업을 수행하는 <br>
  영역을 의미합니다. <br> 
  이 때, 한 프로세스가 자신의 임계 구역에서 수행하는 동안에는 다른 프로세스들은 그들의 임계구역에 들어갈 수 없습니다. <br>
  즉, 동시에 두 프로세스가 그들의 임계구역 안에서 실행할 수 없습니다. 
   
</details>

-----------------------


### 스레드 안전(Thread safe)란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 멀티 스레드 프로그래밍에서 함수, 변수, 객체 등이 여러 스레드로부터 동시에 접근이 이루어져도, <br> 
  프로그램의 실행에 문제가 없음을 나타낸다. <br> 
   
   
</details>


-----------------------


### 스레드 안전한 코드를 작성하는 방법은 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 1) Synchronized 함수 사용
  2) Synchronized 블록 사용
  3) ReentrantLock 사용
  4) 세마포어 사용 
  5) 모니터 사용 등이 있습니다. 
   
 <br> 
   
   
</details>


-----------------------

### Mutex Lock이란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ Mutex Lock은 임계 구역을 보호하고 경쟁 조건을 방지하기 위해 사용되는 락을 의미합니다. <br>
  즉, 프로세스는 임계구역에 들어가기 전에 반드시 락을 획득해야 하고, <br>
  임계구역을 빠져 나올 때, 락을 반환해야 한다. <br> 
  acquire() 함수가 락을 획득하고, release() 함수가 락을 반환한다. <br>  
  acquire() 또는 relase() 함수 호출은 원자적으로 수행되어야 한다. <br>
  이 방식의 단점은 바쁜 대기(busy waiting)을 해야 한다는 것이다. <br>
  프로세스가 임계구역에 있는 동안 임계 구역에 들어가기 원하는 다른 프로세스들은 <br>
  acquire() 함수를 호출하는 반복문을 계속 실행해야 한다. <br>
  사실 이러한 유형의 mutex 락은 락이 가용해지기를 기다리면서 프로세스가 계속 회전을 하고 있기 때문에 <br>
  spinlock이라고도 부른다. 
   
</details>


-----------------------

### 세마포어란? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 세마포어는 mutex와 유사하게 동작하지만, 프로세스들이 자신들의 행동을 더 정교하게 동기화할 수 있는 방법을 제공하는 <br>
  강력한 도구입니다. <br> 
  세마포어는 리소스의 상태를 나타내는 일종의 카운터라고 할 수 있습니다. <br>  
   
  세마포 S는 정수 변수로서, 초기화를 제외하고는, 단지 두 개의 표준 원자적 연산 wait()와 signal()로만 접근이 가능힙니다. <br> 
  wait()와 signal() 연산 시 세마포의 정수 값을 변경하는 연산은 반드시 분리되지 않고 수행되어야 합니다. <br>
  즉, 한 스레드가 세마포 값을 변경하면, 다른 어떤 스레드도 동시에 동일한 세마포 값을 변경할 수 없습니다. 
   
 <br> 
   
   
</details>


-----------------------

### 세마포어의 종류에는 무엇이 있습니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 운영체제는 카운팅(counting)과 이진(binary) 세마포를 구분합니다. <br> 
  카운팅 세마포의 값은 제한 없는 영역(domain)을 갖습니다. <br>
  이진 세마포의 값은 0과 1사이의 값만 가능합니다. <br> 
   
 <br> 
   
   
</details>


-----------------------



### 시분할(또는 멀티 태스킹)이란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 다중 프로그래밍의 논리적 확장으로, 시분할 시스템에서는 CPU가 다수의 작업들을 교대로 수행하지만, <br>
  매우 빈번하게 교대가 일어나기 때문에 프로그램이 실행되는 동안에 사용자들은 각자 자기의 프로그램과 <br>
  상호 작용할 수 있다. 
</details>


-----------------------

### 프로세스란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 실행 중인 프로그램을 의미하며, 현대의 시분할 시스템에서 작업의 단위입니다. <br> 
  하나의 시스템은 프로세스들의 집합입니다. <br> 
</details>


-----------------------

### 프로세스의 상태란 무엇입니까? 무엇 무엇이 있습니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 프로세스 상태에는 새로운(new), 실행(running), 대기(waiting), 준비 완료(ready), 종료(terminated)가 있습니다. <br>
  새로운(new)은 프로세스가 생성 중임을 의미하고, <br>
  실행(running)은 명령어가 실행되고 있음을 의미하고, <br> 
  대기(waiting)는 프로세스가 어떤 사건(입출력 완료 또는 신호의 수신 등)이 일어나기를 기다리는 것을 의미하고, <br> 
  준비 완료(ready)는 프로세스가 처리기에 할당되기를 기다리는 것을 의미하며, <br>
  종료(terminated)는 프로세스의 실행이 종료되었음을 의미합니다. <br> 
</details>


-----------------------


### DeadLock이란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 
+ 다중 프로그래밍 환경에서는 여러 프로세스들이 한정된 자원을 사용하려고 서로 경쟁할 수 있습니다. <br> 
  한 프로세스가 자원을 요청했을 때, 자원을 사용할 수 없는 상황이 발생할 수 있고, <br>
  그 경우 프로세스는 대기 상태로 들어갑니다. <br> 
  이처럼 대기 중인 프로세스들이 결코 다시는 그 상태를 변경시킬 수 없으면 <br>
  이런 상황을 교착상태라 부릅니다. 
</details>

-----------------------

### DeadLock이 성립하기 위한 4가지 조건은 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 
+ 교착 상태에서는 프로세스들은 결코 실행을 끝낼 수 없으며, 시스템 자원이 묶여 있어서 <br>
  다른 작업을 시작하는 것도 불가능합니다. <br>
  교착 상태 문제를 취급하는 다양한 방법들을 논의하기 전에 <br> 
  교착상태의 성격을 규정하는 특징을 더 자세히 살펴보아야 합니다. <br>
   
  (1) 상호 배제(Mutual Exclusion)
   - 최소한 하나의 자원이 비공유 모드로 점유되어야 합니다. <br> 
     비공유 모드에서는 한 번에 한 프로세스만이 그 자원을 사용할 수 있습니다. <br> 
     다른 프로세스가 그 자원을 요청하면, 요청 프로세스는 자원이 방출될 때까지 <br> 
     반드시 지연되어야 합니다. <br> 
   
  (2) 점유하며 대기(Hold-and-wait)
   - 프로세스는 최소한 하나의 자원을 점유한 채, <br>
     현재 다른 프로세스에 의해 점유된 자원을 추가로 얻기 위해 반드시 대기해야 합니다. <br> 
     
  (3) 비선점(No preemption)
   - 자원들을 선점할 수 없어야 합니다. <br> 
     즉, 자원이 강제적으로 방출될 수 없고, 점유하고 있는 프로세스가 태스크를 종료한 후 <br>
     그 프로세스에 의해 자발적으로만 방출될 수 있습니다. 
   
  (4) 순환 대기(Circular wait)
   - 대기하고 있는 프로세스의 집합 {P0, P1, ... Pn}에서 P0는 P1이 점유한 자원을 대기하고, <br> 
     P1은 P2가 점유한 자원을 대기하고, <br>
     P2, ... Pn-1은 Pn이 점유한 자원을 대기하며, Pn은 P0가 점유한 자원을 대기합니다. <br> 
   
  - 우리는 교착 상태가 발생하려면, 앞의 네 가지 조건이 성립되어야 함을 강조합니다. <br> 
    순환 대기 조건은 점유하며 대기 조건을 암시하므로, ><br> 
    네 조건이 완전히 독립적인 것은 아닙니다. <br> 
    그러나 각 조건을 별개로 간주하는 것이 유용합니다. 
</details>

-----------------------


### 교착 상태는 무엇을 통해 보다 정확하게 기술할 수 있습니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 
+ 교착상태는 시스템 자원 할당 그래프라고 하는 방향 그래프로 보다 정확하게 기술할 수 있습니다. <br> 
  이 그래프는 정점(vertex) V의 집합과 간선(edge) E의 집합으로 구성됩니다. <br> 
  정점 V의 집합은 시스템 내의 모든 활성 프로세스의 집합인 P = {P1, P2, P3, ... Pn]과 <br>
  시스템 내의 모든 자원 타입의 집합인 R = {R1, R2, R3, ..., Rm}의 두 가지 타입으로 구별됩니다. <br> 
  
  프로세스 Pi로부터 자원 타입 Rj로의 방향 간선(directed edge)은 Pi -> Rj로 표현하며, <br>
  이것은 프로세스 Pi가 자원 타입 Rj의 인스턴스를 하나 요청하는 것으로 <br> 
  현재 이 자원을 기다리는 상태입니다. <br> 
  
  자원 타입 Rj로부터 프로세스 Pi로의 방향 간선은 Rj->Pi로 표현하며, <br> 
  이것은 자원 타입 Rj의 한 인스턴스가 프로세스 Pi에 할당된 것을 의미합니다. <br> 
   
  방향 간선 Pi->Rj는 요청 간선(request edge)이라 부르고, <br> 
  방향 간선 Rj->Pi는 할당 간선(assignment edge)이라 합니다. <br> 
   
</details>

-----------------------



### DeadLock을 해결하기 위한 4가지 방법은 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 운영체제] 
+  원칙적으로 교착 상태 문제를 처리하는 데는 다음과 같은 세 가지 다른 방법이 있습니다. <br> 
   
   1) 시스템이 결코 교착상태가 되지 않도록 보장하기 위하여 교착상태를 예방하거나 회피하는 프로토콜을 사용합니다. <br> 
   2) 시스템이 교착상태가 되도록 허용한 다음에 회복시키는 방법이 있습니다. <br> 
   3) 문제를 무시하고, 교착상태가 시스템에서 결코 발생하지 않는 척을 합니다. <br> 
   
   세 번째 해결안이 Linux와 Windows를 포함해 대부분의 운영체제가 사용하는 방법입니다. <br> 
   이렇다면 교착상태를 처리하는 프로그램을 작성하는 것은 응용 개발자의 몫입니다. <br> 
   
   교착상태가 발생하지 않도록 하기 위해 시스템은 교착 상태 예방(prevention) 혹은 회피(avoidance) 기법 중 하나를 사용할 수 있습니다. <br> 
   교착상태 예방은 데드락 발생의 필요조건들 중 적어도 하나가 성립하지 않도록 보장하는 일련의 방법입니다. <br> 
   이들 방법은 자원이 어떻게 요청될 수 있는지를 제한함으로써 교착상태를 예방합니다. <br> 
   
   교착상태 회피는 반면에, 프로세스가 일생동안 요구하고 사용할 자원에 대한 부가적인 정보를 미리 제공할 것을 요구합니다. <br> 
   이러한 추가적인 지식을 가지고, 운영체제는 각 요청을 위해 그 프로세스가 기다려야 할지 않을지를 결정할 수 있습니다. <br> 
   각 요구는 시스템이 현재 요청이 만족될 수 있는지, 또는 반드시 지연시켜야 하는지를 결정하기 위해, <br> 
   현재 유용한 자원들과 각 프로세스에 현재 할당된 자원들, 각 프로세스의 미래의 요청과 방출을 고려하도록 요구합니다. <br> 
   
   만약 시스템이 교착상태 예방 혹은 교착상태 회피 알고리즘을 사용하지 않으면, 교착상태가 발생할 수 있습니다 .<br> 
   이런 환경에서 시스템은 교착상태가 발생했는지 결정하기 위해 <br> 
   시스템의 상태를 조사하는 알고리즘과 그리고 교착상태로부터 복구하기 위한 알고리즘을 제공할 수 있습니다. <br> 
   
   교착상태를 탐지하고 복구하는 알고리즘이 없다면, 시스템은 교착상태에 이를 수 있고, <br> 
   그럼에도 불구하고 교착상태가 발생한 것을 인식하지 못할 수 있습니다. <br>
   이 경우 탐지되지 않은 교착상태는 수행이 불가능한 프로세스에 의해 자원이 점유되어 있고, <br> 
   그리고 많은 프로세스들이 이러한 자원을 요청함에 따라 계속 교착상태로 진입하기 때문에 <br> 
   시스템 성능을 저하시키게 됩니다. <br> 
   결국 시스템은 작동을 정지하고, 수작업으로 다시 시작할 필요가 있습니다. <br> 
   
   비록 이 방법이 교착상태 문제에 대한 실현 가능한 해결 방안처럼 보이지는 않지만 <br>
   앞서 언급한 것처럼 몇몇 운영체제에서 여전히 사용되고 있습니다. <br> 
   비용은 중요한 고려 사항 중의 하나입니다. <br> 
   
   교착상태를 무시하는 것이 다른 처리 방법에 비해 비용이 적게 듭니다. <br>
   많은 시스템에서 교착상태는 드물게(이를테면 일 년에 한 번) 발생하기 때문에 <br> 
   다른 처리 방법을 사용하는 부가적인 비용은 그만한 가치가 없을 수 있습니다 .<br> 
   
   게다가 다른 조건으로부터 복구하는 데 사용되는 방법을 교착상태로부터 복구하는데 사용할 수 있습니다. <br> 
   이런 상황에서는 시스템이 교착 상태에 있지 않지만, 동결된 상태에 있을 수 있습니다. <br> 
   
</details>

-----------------------

### 메모리 관리 전략이란 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 공룡책] 
   
+ 메모리 관리 알고리즘은 단순 하드웨어 방식에서 페이징과 세그먼트 방법까지 다양하며, <br>
  각 방법은 고유의 장,단점을 갖고 있습니다. <br> 
  
  가장 간단한 공간 할당 방법은 메모리를 똑같은 고정된 크기로 분할(partition)하는 것입니다. <br> 
  각 분할마다 한 프로세스를 가지고 이 때, 분할의 개수를 다중 프로그래밍 정도(multiprogramming degree)라고 합니다. <br>
  한 분할이 비게 되면 한 프로세스가 입력 큐(input queue)에서 선택되어 빈 분할에 들어옵니다. <br>
  그 프로세스가 끝나면 그 분할은 다른 프로세스를 위해 사용될 수 있습니다. <br>  
   
  가변 분할 기법에서 운영체제는 메모리의 어떤 부분이 사용되고 있고, 어떤 부분이 사용되지 않고 있는가를 파악할 수 있는 테이블을 유지합니다. <br> 
  초기에 모든 메모리 공간은 한 개의 큰 사용 가능한 블록으로 간주됩니다. <br> 
  이 경우 한 개의 공간(hole)이 있다고  표현합니다. <br> 
  앞으로 보겠지만 결국에는 메모리는 다양한 크기의 공간의 집합을 포함하게 됩니다.<br> 
   
   
</details>

-----------------------


### 동적 메모리 할당 문제에 대한 해결책은 무엇이 있는가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 공룡책] 
   
+ 최초 적합(First Fit), 최적 적합(Best Fit), 최악 적합(Worst Fit) 등이 있습니다. 
  
  1) 최초 적합(First Fit)
  - 첫 번째 사용 가능한 가용 공간을 할당합니다. 검색은 집합의 시작에서부터 하거나, <br>
    지난 번 검색이 끝났던 곳에서 시작될 수 있습니다. <br>
    충분히 큰 가용 공간을 찾았을 때, 검색을 끝낼 수 있습니다. <br> 
    
  2) 최적 적합(Best Fit)
  - 사용 가능한 공간들 중에서 가장 작은 것을 택합니다. 리스트가 크기 순으로 되어 있지 않다면 <br>
    전 리스트를 검색해야만 합니다. <br>
    이 방법은 아주 작은 가용 공간을 만들어냅니다. <br> 
   
  3) 최악 적합(Worst Fit)
  - 가장 큰 가용 공간을 택합니다. 이 방식을 할당해 주고 남게되는 자유 공간은 충분히 커서 <br>
    다른 프로세스들을 위하여 유용하게 사용될 수 있습니다. <br> 
    이 때, 자유 공간들이 크기 순으로 정렬되어 있지 않다면 전 리스트를 다 검색해야만 합니다. <br> 
   
   
</details>

-----------------------

### 가상 메모리란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 가상 메모리라는 것은 프로세스 전체가 메모리 내에 올라오지 않더라도 실행이 가능하도록 하는 기법입니다. <br> 
  이 기법의 주요 장점 중 하나는 사용자 프로그램이 물리 메모리보다 커져도 된다는 점입니다. <br> 
  가상 메모리는 물리 메모리로부터 사용자 관점의 논리 메모리를 분리시켜 메인 메모리를 균일한 크기의 저장 공간으로 구성된 <br>
  엄청나게 큰 배열로 추상화 시켜 줍니다. <br> 
  이 기법을 통해 프로그래머는 메모리의 크기 제약으로부터 자유로워집니다. 
   
[참고: incutv]    
+ 가상 메모리라는 것은 프로그램 전체가 아닌 필요한 일부분만 메모리에 올리는 기법입니다. <br> 
  즉, 가상 메모리는 프로세스의 물리 메모리와 논리 메모리를 분리하기 위해 생겨난 것입니다. 
  
  가상 메모리가 없는 경우를 생각하면, <br> 
  RAM의 메모리가 4GB라고 하고, 프로세스 A, B에 필요한 메모리가 4GB라고 한다면, <br> 
  메모리에 프로세스 A가 먼저 할당이 된다면, 프로세스 B는 할당할 메모리가 부족하여 사용할 수 없다. <br> 
   
  가상 메모리가 있는 경우는, 
  RAM의 메모리가 4GB라고 하고, 프로세스 A,B,C가 있다고 하면, <br> 
  프로세스가 현재 사용되는 메모리만큼만 물리 메모리(RAM)에 할당과 해제를 반복하여 <br>
  메모리를 사용한다면 여러 프로세스를 사용할 수 있다. <br> 
   
   
</details>

-----------------------


### 가상화란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+  
</details>

-----------------------

### 가상머신이란 무엇입니까?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+  
</details>

-----------------------

### 캐시의 지역성 원리란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />

+ 캐시 메모리는 속도가 빠른 장치와 느린 장치간의 속도차에 따른 병목 현상을 줄이기 위한 범용 메모리입니다. <br> 
  이러한 역할을 수행하기 위해서는 CPU가 어떤 데이터를 원할 것인가를 어느 정도 예측할 수 있어야 한다. 
   
  1) 캐시 메모리에서 원하는 데이터를 찾는 다면, 메인 메모리까지 가서 찾지 않아도 되기 때문에 성능 향상 <br> 
  2) 캐시 메모리에 원하는 데이터에 적중률 성능의 관건 <br> 
  -> 이 때, 적중률을 높이기 위해 데이터 지역성 원리를 사용한다. 
   
  시간 지역성 
  - 최근에 참조된 주소의 내용은 곧 다음에 다시 참조되는 특성 
   
  공간 지역성
  - 대부분의 실제 프로그램이 참조된 주소와 인접한 주소의 내용이 다시 참조되는 특성 
  -> 캐시 메모리에 데이터를 저장할 때, 공간 지역성을 최대한 활용하기 위해, 
     해당 데이터뿐만 아니라 옆 주소의 데이터도 같이 가져와 미래에 쓰일 것을 대비한다. 
 
   
</details>

-----------------------


### 무어의 법칙이란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 대량 생산한 칩상의 트랜지스터 수가 약 18개월마다 2배씩 증가하는 것을 의미합니다. 
</details>

-----------------------

### 무어의 법칙에 따라 개수가 급증한 트랜지스터는 처음엔 무엇을 높이는데 쓰였습니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 클록 속도(clock speed)를 높이는 데 쓰였습니다. <br> 
  클록 속도가 증가하면 초당 더 많은 명령어를 처리할 수 있기 때문입니다. 
</details>

-----------------------

### 클록 속도란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.intel.co.kr/content/www/kr/ko/gaming/resources/cpu-clock-speed.html]
   
+ 클럭 속도는 CPU가 초당 실행하는 사이클 수를 GHz 단위로 측정한 것입니다. <br>
  사이클은 기술적으로는 내부 발진기에 의해 동기화된 펄스를 의미하지만, <br>
  여기에서는 CPU 속도를 이해하는데 도움이 되는 기본적인 단위라고 보시면 됩니다. <br> 
  사이클마다 프로세서 내 수십억 개의 트랜지스터가 열리고 닫힙니다. <br> 
   
</details>

-----------------------

### 클록 속도가 증가하니 발생한 문제는 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 칩이 빨라질수록 데이터도 더 빨리 움직여야 하는데, <br> 
  시간이 갈수록 프로세서 코어의 데이터 수요를 메인 메모리가 맞추기 어려워졌습니다. 
   
</details>

-----------------------

### CPU 캐시란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ CPU 캐시는 CPU에 있는 메모리 영역입니다. <br> 
  레지스터보다는 느리지만, 메인 메모리보다는 훨씬 빠릅니다. <br> 
  자주 액세스하는 메모리 위치는 CPU가 메인 메모리를 재참조하지 않게 <br> 
  사본을 떠서 CPU 캐시에 보관하자는 아이디어입니다. 
   
</details>

-----------------------

### CPU 캐시의 종류에는 무엇이 있습니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ CPU와 가장 가까운 캐시가 L1, 그 다음 캐시가 L2 식으로 명명합니다. <br> 
  프로세서 아키텍처에 따라 캐시 개수 및 설정 상태는 제각각이지만, <br> 
  일반적으로 각 실행 코어에 전용 프라이빗 캐시 L1, L2를 두고, <br> 
  일부 또는 전체 코어가 공유하는 L3 캐시를 둡니다. <br> 
   
  이렇게 캐시 아키텍처를 이용해 액세스 시간을 줄이고 코어가 처리할 데이터를 계속 채워 넣습니다. <br> 
  클록 속도와 액세스 시간 차이 때문에 최신 CPU는 더 많은 예산을 캐시에 투자합니다. <br> 
</details>

-----------------------

### 변환 색인 버퍼(Translaction Lookaside Buffer)란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 여러 캐시에서 아주 긴요하게 쓰이는 장치로서, <br> 
  가상 메모리 주소를 물리 메모리 주소로 매핑하는 페이지 테이블의 캐시 역할을 수행합니다. <br> 
   
</details>

-----------------------

### 페이지 테이블(Page Table)이란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://code-lab1.tistory.com/55]
   
+ 페이징이란 논리 주소의 메모리를 고정된 크기의 페이지(Page)로 나누어 관리하는 기법입니다. <br> 
  페이징은 아래와 같은 특징들을 갖고 있습니다. <br> 
   
  1) 물리주소 공간(Physical Address)은 연속적이지 않을 수 있습니다. <br> 
  2) 물리주소 공간을 페이지와 같은 사이즈로 나눈 것들을 프레임(Frame)이라고 합니다. <br> 
  3) 페이지 사이즈(=프레임 사이즈)는 하드웨어에 의해 정해집니다. <br> 
  4) 페이지의 크기는 일반적으로 2의 제곱수를 사용합니다. <br> 
     일반적으로 4KB(2^12) ~ 1GB(2^20) <br> 
  5) 페이지 테이블(Page Table)을 이용해 논리주소에서 프레임을 가리키는 물리주소로 매핑합니다. <br> 
  6) 외부 단편화는 발생하지 않으나, 내부 단편화는 발생합니다. <br> 
</details>

-----------------------

### 메모리 액세스 제어의 핵심은 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 메모리 관리 유닛(MMU)를 통한 가상 주소 방식(virtual addressing)과 페이지 테이블입니다. <br>
  이는 한 프로세스가 소유한 메모리 영역을 다른 프로세스가 함부로 훼손하지 못하게 합니다. 
</details>

-----------------------

### 프로세스 스케줄러의 역할은 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ 프로세스 스케줄러는 CPU 액세스를 통제합니다. 이 때, 실행 큐(run queue)라는 큐를 이용합니다. <br> 
  최신 시스템은 거의 항상 가능한 수준보다 더 많은 스레드/프로세스로 가득하기 때문에 <br> 
  CPU 경합을 해소할 장치가 절실합니다. <br> 
   
  스케줄러는 인터럽트에 응답하고 CPU 코어 액세스를 관리합니다. 
</details>

-----------------------

### CPU 코어란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://library.gabia.com/contents/infrahosting/1227/]
   
+ CPU 코어는 연산 작업을 수행하는 핵심적인 부분이며, CPU의 성능을 판단하는 기준 중 <br> 
  하나가 바로 '코어의 수'입니다. CPU에 코어가 많아지면 연산을 여러 개의 코어가 처리하기 때문에 <br>
  훨씬 빠른 일 처리가 가능해집니다. <br> 
</details>

-----------------------

### 컨텍스트 교환이란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ OS 스케줄러가 현재 실행중인 스레드/태스크를 없애고, 대기 중인 다른 스레드/태스크로 대체하는 프로세스입니다. <br>
  종류는 다양하지만, 뭉뚱그려 말하면, 컨텍스트 교환은 스레드 실행 명령과 스택 상태를 교체하는 모든 일에 연관되어 있습니다. <br> 
  
  유저 스레드 사이에 발생하든, 유저 모드에서 커널 모드로 바뀌면서 일어나든 컨텍스트 교환은 비싼 작업입니다.
  특히, 후자가 그렇습니다. <br>
  유저 스레드가 타임 슬라이스 도중 커널 모드로 바꾸어 어떤 기능을 실행해야 할 때가 있습니다. <br> 
  하지만 유저 공간에 있는 코드가 액세스하는 메모리 영역은 커널 코드와 거의 공유할 부분이 없기 때문에 <br> 
  모드가 바뀌면 명령어와 다른 캐시를 어쩔 수 없이 강제로 비워야 합니다. <br> 
</details>

-----------------------

### CPU 사용률이란 무엇입니까? 

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 최적화]
   
+ CPU 사용률은 애플리케이션 성능을 나타내는 핵심 지표입니다. <br> 
  CPU 사이클은 애플리케이션이 가장 갈증을 느끼는 리소스라서 CPU의 효율적 사용은 성능 향상의 지름길입니다. <br> 
  또 부하가 집중되는 도중에는 사용률이 가능한 한 100%에 가까워야 합니다. 
</details>

-----------------------
