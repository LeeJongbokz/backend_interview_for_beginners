# Java OOP
<br>


### 클래스 메서드 vs 인스턴스 메서드?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 
 
+ 변수에서 그랬던 것과 같이, 메서드 앞에 static이 붙어 있으면 클래스 메서드이고, <br> 
  붙어 있지 않으면 인스턴스 메서드입니다. <br> 
  클래스 메서드도 클래스 변수처럼, 객체를 생성하지 않고도 '클래스 이름. 메서드 이름(매개변수)'와 같은 식으로 호출이 가능합니다. <br> 
  반면, 인스턴스 메서드는 반드시 객체를 생성해야만 호출할 수 있습니다. <br> 
  
  그렇다면 클래스를 정의할 때, 어느 경우에 static을 사용해서 클래스 메서드로 정의해야 하는 것일까요? <br> 
  클래스는 '데이터(변수)와 데이터에 관련된 메서드의 집합'이므로, 같은 클래스 내에 있는 메서드와 멤버 변수는 아주 밀접한 관계가 있습니다. <br> 
  
  인스턴스 메서드는 인스턴스 변수와 관련된 작업을 하는, 즉 메서드의 작업을 수행하는데 인스턴스 변수를 필요로 하는 메서드입니다. <br> 
  그런데 인스턴스 변수는 인스턴스(객체)를 생성해야만 만들어지므로, 인스턴스 메서드 역시 인스턴스를 생성해야만 호출될 수 있는 것입니다. <br> 
  
  반면에, 메서드 중에서 인스턴스와 관계없는(인스턴스 변수나 인스턴스 메서드를 사용하지 않는)메서드를 클래스 메서드(static 메서드)로 정의합니다. <br> 
  물론 인스턴스 변수를 사용하지 않는다고 해서 반드시 클래스 메서드로 정의해야 하는 것은 아니지만, 특별한 이유가 없는 한 그렇게 하는 것이 일반적입니다. <br> 
  
</details>

-----------------------

### 상속이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 
 
+ 상속이란, 기존의 클래스를 재사용하여 새로운 클래스를 작성하는 것입니다. <br> 
  상속을 통해서 클래스를 작성하면 보다 적은 양의 코드로 새로운 클래스를 작성할 수 있고, <br> 
  코드를 공통적으로 관리할 수 있기 때문에, 코드의 추가 및 변경이 매우 용이합니다. <br> 
   
  이러한 특징은 코드의 재사용성을 높이고 코드의 중복을 제거하여 프로그램의 생산성과 유지보수에 크게 기여합니다. <br> 
  자바에서 상속을 구현하는 방법은 아주 간단합니다. <br> 
  새로 작성하고자 하는 클래스의 이름 뒤에 상속 받고자 하는 클래스의 이름을 키워드 'extends'와 함께 써주기만 하면 됩니다. <br> 
  
  예를 들어, 새로 작성하려는 클래스의 이름이 Child이고 상속 받고자 하는 기존 클래스의 이름이 Parent라면 다음과 같이 하면 됩니다. <br> 
   
  ```
  class Child extends Parent{
        // ...
  }
  ```
   
  이 두 클래스는 서로 상속 관계에 있다고 하며, 상속해주는 클래스를 '조상 클래스'라 하고, <br>
  상속 받는 클래스를 '자손 클래스'라고 합니다. <br> 
</details>

-----------------------


### 접근 제어자란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 
 
+ 접근 제어자는 멤버 또는 클래스에 사용되어, 해당하는 멤버 또는 클래스를 외부에서 접근하지 못하도록 제한하는 역할을 합니다. <br> 
  접근 제어자가 default임을 알리기 위해 실제로 default를 붙이지는 않습니다. <br> 
  클래스나 멤버변수, 메서드, 생성자에 접근 제어자가 지정되어 있지 않다면, 접근 제어자가 default임을 뜻합니다. <br>
   
  접근 제어자가 사용될 수 있는 곳 - 클래스, 멤버변수, 메서드, 생성자 <br> 
  private: 같은 클래스 내에서만 접근이 가능함 <br> 
  default: 같은 패키지 내에서만 접근이 가능함 <br> 
  protected: 같은 패키지 내에서, 그리고 다른 패키지의 자손클래스에서 접근이 가능함 <br> 
  public: 접근 제한이 전혀 없음 <br> 
   
  접근 범위가 넓은 쪽에서 좁은 쪽의 순으로 왼쪽부터 나열하면 다음과 같습니다. <br> 
  ``` 
     public > protected > (default) > private
  ``` 
  
  public은 접근 제한이 전혀 없는 것이고, private은 같은 클래스 내에서만 사용하도록 제한하는 가장 높은 제한입니다. <br> 
  그리고 default는 같은 패키지내의 클래스에서만 접근이 가능하도록 하는 것입니다. <br> 
  마지막으로 protected는 패키지에 관계없이 상속관계에 있는 자손 클래스에서 접근할 수 있도록 하는 것이 제한목적이지만, <br> 
  같은 패키지 내에서도 접근이 가능합니다. <br> 
  그래서 protected가 default보다 접근 범위가 더 넓습니다. <br> 
</details>

-----------------------

### 접근 제어자를 이용한 캡슐화란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바의 정석] 
 
+ 클래스나 멤버, 주로 멤버에 접근 제어자를 사용하는 이유는 클래스의 내부에 선언된 데이터를 보호하기 위해서입니다. <br> 
  데이터가 유효한 값을 유지하도록, 또는 비밀번호와 같은 데이터를 외부에서 함부로 변경하지 못하도록 하기 위해서는 <br> 
  외부로부터의 접근을 제한하는 것이 필요합니다. <br> 
  이것을 데이터 감추기(data hiding)이라고 하며, 객체지향개념의 캡슐화(encapsulation)에 해당하는 내용입니다. <br> 
   
  또 다른 이유는 클래스 내에서만 사용되는, 내부 작업을 위해 임시로 사용되는 멤버변수나 부분작업을 처리하기 위한 메서드 등의 멤버들을 <br>
  클래스 내부에 감추기 위해서입니다. <br> 
   
  외부에서 접근할 필요가 없는 멤버들을 private으로 지정하여 외부에 노출시키지 않음으로서 복잡성을 줄일 수 있습니다. <br>
  이것 역시 캡슐화에 해당합니다. <br> 
   
  즉, 접근 제어자를 사용하는 이유는 <br>
  (1) 외부로부터 데이터를 보호하기 위해서 <br>
  (2) 외부에는 불필요한, 내부적으로만 사용되는, 부분을 감추기 위해서 입니다. 
  
</details>

-----------------------

