# 네이버Z
https://v6xcareer.notion.site/2f61a1b40c81495eaf564cde9efc6089

<br>


### 네트워크 TCP, UDP 차이?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
[참고: https://base64.guru/]
   
+  
</details>


-----------------------

### HTTP?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
[참고: HTTP 완벽 가이드 p.287]
   
+    
</details>
 
-----------------------

### MySQL과 MongoDB의 차이점은?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
[참고: ]
   
+    
</details>

-----------------------

### System Call이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
[참고: 쉽게 배우는 운영체제 p.51] 

+ 시스템 호출은 커널이 자신을 보호하기 위해 만든 인터페이스입니다. <br> 
  커널은 사용자나 응용 프로그램으로부터 컴퓨터 자원을 보호하기 위해 자원에 직접 접근하는 것을 차단합니다. <br> 
  따라서 자원을 이용하려면 시스템 호출이라는 인터페이스를 이용하여 접근해야 합니다. <br> 
   
  그렇다면 자원에 직접 접근하는 것과 시스템 호출을 통해 접근하는 것은 어떤 차이가 있을까? <br> 
  이를 쉽게 이해할 수 있도록 커피를 마시고 싶을 때, 직접 만들어 먹는 경우와 <br>
  다른 사람에게 만들어달라고 부탁하는 경우를 생각해보자. <br> 
   
  (1) 직접 접근
  - 사용자가 직접 컴퓨터 자원에 접근하여 작업하는 방식으로, 사용자가 모든 것을 처리해야 합니다. <br> 
    [그림 1-21]에서 보듯이, 사용자는 커피와 설탕이 어디에 있는지, 커피 머신을 어떻게 작동해야 하는지 등을 모두 알아야 합니다. <br> 
    이 경우는 자기 입맛에 맞는 커필르 만들 수는 있지만, 사용자의 부주의로 커피머신을 망가뜨리거나 주변을 더럽힐 수도 있습니다. <br> 
    즉, 커피 머신을 보호하기 어렵다는 단점이 있습니다. <br> 
  (2) 시스템 호출을 통한 접근
  - 누군가에게 요청하여 작업의 결과만 받는 방식입니다. [그림 1-21]에서 보듯이 사용자는 어떤 커피머신을 쓰는지, 어떻게 커피를 만드는지 등을 <br>
    신경쓸 필요 없이 결과만 받으면 됩니다. 이 경우는 사용자의 오작동이나 악의에 의해 커피머신이 망가지는 일도 막을 수 있습니다. <br> 
    이와 마찬가지로 운영체제는 사용자나 응용 프로그램이 하드웨어에 직접 접근하지 못하도록 막음으로써 컴퓨터 자원을 보호합니다. <br> 
    그리고 대신 하드웨어와 같은 시스템 자원을 사용할 수 있도록 인터페이스를 제공하는데 이것이 바로 시스템 호출입니다. <br> 
   
  이번에는 응용 프로그램의 입장에서 시스템 호출을 살펴봅니다. <br> 
  어떤 응용 프로그램은 숫자 14를, 또 어떤 응용 프로그램은 숫자 21을 하드디스크에 저장하려 한다고 가정합니다. <br> 
  
  (1) 직접 접근
  - 두 응용 프로그램이 자기 마음에 드는 위치에 데이터를 저장하려 할 것입니다. 이 경우 다른 사람의 데이터를 지울 수도 있고, <br> 
    내 데이터가 다른 사람에 의해 지워질 수도 있습니다. <br> 
   
  (2) 시스템 호출을 통합 접근
  - 응용 프로그램이 직접 하드디스크에 데이터를 저장하지 않고, 커널이 제공하는 write() 함수를 사용하여 데이터를 저장해달라고 요청합니다. <br> 
    응용 프로그램은 데이터가 하드디스크의 어느 위치에 어떤 방식으로 저장되는지 알 수 없습니다. <br> 
    만약 자신이 저장한 데이터를 읽고 싶다면 read() 함수로 시스템 호출을 이용하면 가져오면 됩니다. <br> 
    시스템 호출을 이용하면 커널이 데이터를 가져오거나 저장하는 것을 전적으로 책임지기 때문에 <br> 
    컴퓨터 자원을 관리하기가 수월합니다. 
   
</details>


-----------------------


### Docker와 Virtual Machine의 차이점은?

<details>
   <summary> 답안 보기 (👈 Click)</summary>

+ 
</details>


-----------------------

### FireWall의 동작 원리는?

<details>
   <summary> 답안 보기 (👈 Click)</summary>

+ 
</details>


-----------------------






네트워크 TCP, UDP 차이

HTTP 설명

RESTFUL API 설명

HTTP 자원은 어떻게 사용되는 것이며 HTTP 메소드는 어떻게 사용되는 것인지

RDB index 설명

속도를 최대한 높이기 위해 모든 컬럼에 index를 걸어놓는 게 좋을까?

JPA n+1 문제 설명

n+1 문제 해결 방법

리스트와 어레이의 차이점

어레이리스트와 링크드리스트의 차이

set, map 차이

hash map, tree map 차이

set과 map에서 넣은 데이터의 순서가 보장되는지

인터페이스와 추상클래스의 차이

멤버도, 상수도 없고 추상메소드만 있을 때 인터페이스와 추상클래스의 차이

자바의 equals와 hashcode에 대해 설명

등호(=)와 다른 점은?

등호(=)와 hashcode랑 다를까요?

박싱과 언박싱 설명

왜 primitive 타입과 reference 타입이 나눠져있을까

자바에서 접근제어자 설명

접근제어자 예약어는 다 그대로 쓰면 되는지? 생략이 가능한지?

스레드와 프로세스의 차이

 

 

입코딩으로 "캐시"를 구현해 보세요.

조건: 데이터를 최대 n개까지 저장할 수 있으며. 캐시가 꽉 찼을 경우 LRU 방식으로 기존 데이터 제거 / 새 데이터를 추가할 수 있어야 한다.

코드리뷰를 해본 적 있는지, 또는 오픈소스에 기여해본 적 있는지. 누군가의 코드를 리뷰한다면, 중요하게 생각하는 게 무엇인지

기본적인 내용을 확실히 알고 있는지 확인하려는 목적의 꼬리질문이 매우 많았다. 예컨대 캐시 구현을 위해 해시테이블 자료구조를 언급하고 시간복잡도 O(1)을 언급하면 "Open Addressing 방식에서 테이블 크기를 늘릴 때에는 O(n) 아니냐, 항상 O(1)이 맞는가?" 라던가.

올바른 답변을 할 수 있도록 유도해주기도 했다. 캐시 문제를 풀기 위해서는 해시테이블과 Double linked List 두 개의 자료구조를 활용해야 하는데, Double linked List를 떠올리지 못해서 헤메고 있으니 면접관이 먼저 자료구조를 언급하고, 자료구조의 특징을 설명해보라고 했었다.

코드리뷰 관련해서 '프로그래밍 철학'을 물어본 점이 인상적이었음.

"좋은 코드란 무엇인가"를 고민해봤어야 깊이있는 답변을 할 수 있었겠다

JDBC / ORM 개념을 알고 있는지

로드밸런싱의 개념 (L4 / L7)

HTTP / HTTPS의 차이

Public / Private 클라우드의 차이, IaaS의 의미

REST API의 정의

Relational DB / NoSQL의 차이점

아키텍처란 무엇인가, 대용량 트래픽을 견뎌낼 만한 아키텍처는 무엇이라고 생각하는가
