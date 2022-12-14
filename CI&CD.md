# CI&CD
<br>


### 젠킨스 파이프라인이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: Jenkins Official Website(https://www.jenkins.io/doc/book/pipeline/)] 
   
+ 젠킨스 파이프라인은 지속적 배포를 위한 파이프라인을 구축하는 플러그인들의 집합을 의미합니다. <br>
  CD 파이프라인은 사용자 혹은 고객에게 버전 컨트롤에 의한 소프트웨어를 자동으로 표현하는 프로세스입니다. <br>
  
  모든 소프트웨어에 대한 변화는 출시되기까지의 복잡한 프로세스를 겪습니다. <br> 
  이 프로세스는 소프트웨어를 신뢰할 수 있고 반복적인 방식으로 빌드하고, <br>
  빌드된 소프트웨어를 여러 단계의 테스팅과 배포로 발전시키는 것을 의미합니다. <br> 
  
[참고: https://www.jenkins.io/doc/book/pipeline/] 

+ 젠킨스 파이프라인이란 Jenkins에 지속적 배포 파이프라인을 구현하고 통합하는 것을 <br>
  지원하는 플러그인들의 집합을 의미합니다. <br>
   
  지속적 배포 파이프라인이란 자동화된 프로세스의 표현으로써, <br>
  그것은 소프트웨어를 버전 컨트롤부터 바로 당신의 사용자와 고객에게 전달합니다. <br> 
  당신의 소프트웨어에 대한 모든 변화(소스 컨트롤에 커밋된)는 릴리즈되기까지 <br> 
  복잡한 프로세스를 경험합니다. <br> 
  
  이 프로세스는 소프트웨어를 신뢰할만하고, 반복적인 방법으로 빌드하고, <br> 
  빌드된 소프트웨어를 여러 단계의 테스팅과 배포 스테이지를 진행시키는 것을 의미합니다. <br> 
   
  파이프라인은 간단한 것부터 복잡한 단계의 배포 파이프라인을 모델링하기 위한 다양한 셋의 툴을 <br> 
  코드로 수행할 수 있도록 제공하는데, 그것은 파이프라인 DSL 문법으로 가능합니다. <br> 
   
  젠킨스 파이프라인의 정의는 텍스트 파일(Jenkins 파일이라고 부르는)에 적혀져 있고, <br> 
  그것은 프로젝트의 소스 컨트롤 저장소에 커밋될 수 있습니다. <br> 
   
  이것이 "코드로써의 파이프라인"의 기초이며, CD 파이프라인을 애플리케이션의 파트로써 다루고, <br> 
  다른 코드와 마찬가지로 버전화되고 리뷰될 수 있습니다. <br> 
   
  Jenkins 파일을 생성하고, 소스 컨트롤에 커밋하는 것은 즉각적으로 다양한 혜택을 제공합니다. <br> 
  
  1) 자동적으로 모든 브랜치와 PR에 대한 파이프라인 빌드 프로세스를 제공합니다. <br> 
  2) 파이프라인에서 코드 리뷰와 이터레이션이 가능합니다. <br> 
  3) 파이프라인에 대한 감사용 기록이 가능합니다. <br> 
  4) 파이프라인에 대한 single source of truth를 제공하며, 그것은 프로젝트에 참여한 여러 멤버들에 <br>
     의해 보여지고 편집될 수 있습니다. <br> 
   
  파이프라인을 정의하기 위한 문법은 web UI든 Jenkinsfile 이든 같지만, <br> 
  일반적으로 JenkinsFile로 파이프라인을 정의하는 것이 최선의 프랙티스로 간주되고, <br> 
  그것을 source control에 check 해야 합니다. <br>  
</details>

-----------------------

### 젠킨스의 DSL(Domain-Specific Language)는 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 젠킨스 시작하기2] 
   
+ DSL은 그루비에 기반을 두었고, 젠킨스에 특화된 용어와 기능어를 포함한다. <br> 
  예를 들어, node 키워드는 이전에 '마스터' 혹은 '슬레이브'로 불렸던 노드를 선택해 <br>
  프로그램의 일부를 수행하기 위해 사용됩니다. <br> 
   
  젠킨스는 오랜 시간 동안 그루비 엔진을 포함해왔습니다. <br>
  이는 웹 인터페이스에서 불가능한 접근 및 기능과 깊은 수준의 스크립트 작업을 지원하기 위해 사용됩니다. <br>
  
  DSL은 젠킨스 2의 핵심 요소입니다. DSL은 사용자에게 공개된 기능을 활성화시키는 역할을 합니다. <br> 
  
  
</details>

-----------------------

### Jenkinsfile이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 젠킨스 시작하기2] 
   
+ 젠킨스 2에서는 파이프라인을 정의하는 부분이 젠킨스와 분리될 수 있습니다. <br>
  과거 버전에서는 잡을 정의하는 내용이 젠킨스의 홈 폴더 경로에 저장됐습니다. <br>
  이는 젠킨스가 이 내용을 보고, 이해하고 수정해야 한다는 의미입니다. <br>
   
  젠킨스2에서는 DSL 스크립트를 이용해 웹 인터페이스에서 파이프라인을 정의할 수도 있습니다. <br>
  하지만 DSL을 소스 코드와 함께 텍스트 파일로 저장하는 것도 가능합니다. <br>
  따라서 일반 소스 코드를 다루는 것과 같이 파일을 이용해 젠킨스 잡을 실행시킬 수 있고, <br>
  변경 추적과 분석도 가능해집니다. 

  젠킨스 2에서는 잡 혹은 파이프라인을 정의하는 파일의 명칭은 Jenkinsfile입니다. <br>
  여러 개의 Jenkinsfile을 가질 수 있으며, 프로젝트나 브랜치마다 다를 수 있습니다. <br>
  빌드에 관여하는 모든 코드를 Jenkinsfile에 저장하는 것도 가능하고, <br>
  일부를 공유 라이브러리를 통해 빼내는 것도 가능합니다. <br>
  또한, DSL 코드를 통해 외부 스크립트를 읽어들이는 것도 가능합니다. 
  
[참고: https://www.jenkins.io/doc/book/pipeline/jenkinsfile/] 
 
+ 이 섹션은 Getting Started with Pipeline(https://www.jenkins.io/doc/book/pipeline/getting-started/)의 정보에 기반해서 구성되었고, <br> 
  더 유용한 스텝들, 일반적인 패턴들, 그리고 몇몇 사소하지 않은 Jenkinsfile 예시를 설명합니다. <br> 
  
  Jenkinsfile을 만드는 것은 source control에 체크인 되는데, <br>
  다양한 즉각적인 혜택을 가져다줍니다. <br> 
  (1) 파이프라인에 대한 코드 리뷰와 iteration <br> 
  (2) 파이프라인에 대한 감사 추적 <br> 
  (3) 파이프라인에 대한 Single Source of truth, <br> 
      그것은 프로젝트의 여러 멤버들에 의해 보여지고 편집될 수 있음 <br> 
   
  파이프라인은 두 가지 문법을 지원합니다. <br> 
  선언적, 그리고 스크립트 파이프라인입니다. <br> 
  둘 다 지속적 배포 파이프라인을 구성하는 것을 지원합니다. <br> 
  둘 다 파이프라인을 Web UI 혹은 Jenkinsfile로 정의하는데 사용될 수 있지만, <br>
  일반적으로는 Jenkinsfile을 생성하고, 그것을 source control repository에 <br> 
  포함시키는 것이 최선으로 여겨집니다. <br> 
  
</details>

-----------------------

### Jenkinsfile은 어떻게 생성하는가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
  
[참고: https://www.jenkins.io/doc/book/pipeline/jenkinsfile/] 
 
+ SCM으로 파이프라인 정의하기(https://www.jenkins.io/doc/book/pipeline/jenkinsfile/)에서 논의되었듯이 <br> 
  Jenkinsfile은 Jenkins 파이프라인에 대한 정의를 포함한 텍스트 파일로서, source control에 포함됩니다. <br> 
  기본적인 세 단계의 지속적 배포 파이프라인을 구현한 아래 파이프라인을 봐봅시다. <br> 

  ```
   Jenkinsfile (Declarative Pipeline)
      pipeline {
          agent any

          stages {
              stage('Build') {
                  steps {
                      echo 'Building..'
                  }
              }
              stage('Test') {
                  steps {
                      echo 'Testing..'
                  }
              }
              stage('Deploy') {
                  steps {
                      echo 'Deploying....'
                  }
              }
          }
      }
  ```
  
  모든 파이프라인이 이 세 가지 스테이지를 갖고 있는 것은 아니지만, <br> 
  이것은 대부분의 프로젝트에서 그것들을 정의하는데 있어서 좋은 시작점입니다. <br> 
  이 섹션은 Jenkins의 테스트 설치 과정에서의 간단한 파이프라인의 생성과 실행을 보여줍니다. <br>
   
  이 때, source control 저장소가 이미 프로젝트를 위해 셋업되어 있고, <br> 
  파이프라인이 Jenkins로 정의되어 있다는 것을 가정합니다. <br>  
   
  이상적으로는 그루비 문법 하이라이팅을 지원하는 텍스트 에디터를 활용해서 <br> 
  프로젝트의 루트 디렉토리에 새로운 Jenkinsfile을 생성합니다. <br> 
   
  위의 선언적 파이프라인 예시는 지속적인 배포 파이프라인을 구현하기 위한 최소한의 필요한 구조만을 포함합니다. <br>
  필요한 agent directive는 Jenkins가 파이프라인을 위한 executor와 workspace를 배치하도록 지시합니다. <br> 
  Agent Directive 없이는 선언적 파잉프라인이 유효하지 않을 뿐만 아니라, 어떠한 작업도 할 수 없습니다. <br> 
  기본적으로 Agent Directive는 source 저장소가 체크 아웃되고, 이후 스테이지를 위한 준비가 되도록 합니다. <br>   
   
  Stages Directive와 Steps Directive가 또한 유효한 선언적 파이프라인을 위해 필요하며, <br>
  그 이유는 그것들이 Jenkins에게 무엇을 실행하고, 어떤 stage에서 그것이 실행되어야 하는지 알려주기 때문입니다. <br> 
   
</details>

-----------------------

### 빌드한다는 것이 무엇인가?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.jenkins.io/doc/book/pipeline/jenkinsfile/] 
   
+ 많은 프로젝트에서 파이프라인에서 '작업'의 시작은 '빌드' 단계입니다. <br> 
  일반적으로 파이프라인의 이 단계는 소스 코드가 합쳐지고, 컴파일되고 혹은 패키징됩니다. <br> 
  Jenkinsfile은 현재의 빌드 툴인 GNU/Make, Maven, Gradle, 등에 대한 대체재가 아닙니다. <br> 
  오히려 프로젝트의 개발 라이프사이클(빌드, 테스트, 배포 등)의 여러 단계를 묶는 <br> 
  glue layer로 볼 수 있습니다. <br> 
   
  Jenkins는 일반적인 사용을 위해 어떤 빌드 툴이든 실용적으로 호출하는 여러 플러그인을 갖고 있지만, <br> 
  이 예시에서는 단순히 쉘 단계에서 make를 호출하겠습니다. <br> 
  sh 스텝은 시스템이 Unix/Linux에 기반함을 가정하며, 윈도우에 기반한 시스템에서는 bat가 대신 사용될 수 있습니다. <br> 
   
  ```
    Jenkinsfile (Declarative Pipeline)
      pipeline {
          agent any

          stages {
              stage('Build') {
                  steps {
                      sh 'make' 
                      archiveArtifacts artifacts: '**/target/*.jar', fingerprint: true 
                  }
              }
          }
     }
  ``` 
  - sh 스텝은 make 명령을 호출하고, 명령에 의해 zero exit code가 리턴될때만 계속합니다. <br>
    어떤 non-zero exit code도 파이프라인을 실패합니다. <br> 
   
  - archiveArtifacts는 포함 패턴(**/target/*.jar)과 일치하는 빌드된 파일을 캡처하고, <br>
    나중에 검색할 수 있도록 Jenkins 컨트롤러에 저장합니다. <br> 
   
</details>


-----------------------


### 서술적 파이프라인이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 젠킨스 시작하기2] 
   
+ 젠킨스에서 pipelines-as-code 이전의 예제 코드는 젠킨스에 특화된 DSL 스텝이 추가된 그루비 스크립트였습니다. <br>
  젠킨스 관련 구조는 아주 조금이고, 프로그램의 흐름은 그루비에 의해 관리됐습니다. <br>
  에러 보고와 확인 부분도 젠킨스와 관련 없이 그루비 프로그램 실행에 기반하고 있습니다. <br>
   
  이러한 모델을 앞으로 스크립트 방식의 파이프라인이라고 지칭합니다. <br>
  하지만 파이프라인용 DSL은 이 책에서 점차 변경되고 발전됩니다. 
</details>

-----------------------

### 젠킨스란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: 자바 프로젝트 필수 유틸리티] 
   
+ 젠킨스는 자바로 작성된 오픈 소스 소프트웨어로 지속적 통합(CI)과 지속적 배포(CD)를 제공합니다. <br> 
  웹 어플리케이션 형태로 제공되고 있어서, 어떠한 환경에서도 손쉽게 설치할 수 있으며, <br> 
  도커를 사용해 설치할 수도 있습니다. <br> 
  또한, 천 개 이상의 플러그인으로 다양한 시스템과 연동할 수 있습니다. <br> 
   
  젠킨스의 주요 기능은 아래와 같습니다. <br> 
  1) 형상관리 도구와의 연동 <br>
  2) 소스 코드 체크아웃 <br> 
  3) 웹 인터페이스 <br> 
  4) 테스트 보고서 생성 <br> 
  5) 빌드 및 테스트 자동화 <br> 
  6) 실행 결과 통보 <br>
  7) 코드 품질 감시 <br> 
  8) 다양한 인증 기반과 결합한 인증 및 권한 관리 <br> 
  9) 배포 관리 자동화 <br> 
  10) 분산 빌드(마스터 슬레이브) <br> 
  11) 그루비 스크립트를 이용한 자유로운 잡 스케줄링 <br> 
   
  젠킨스는 개발자가 소스를 추가, 수정한 뒤 형상관리 도구에 저장하면 자동으로 읽어 빌드 및 테스트를 실행합니다. <br> 
  통합 프로세스를 거쳐 검증하여 코드의 문제를 감지하고 빠른 피드백을 제공합니다. <br> 
   
   
   
</details>

-----------------------

### 젠킨스 설치란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.jenkins.io/doc/book/installing/] 
   
+ 젠킨스는 일반적으로 자기 자신의 프로세스에 따라서 독립적인 어플리케이션으로 동작합니다. <br> 
  젠킨스 WAR 파일은 Winstone, Jetty 서블릿 컨테이너 wrapper를 묶고, <br> 
  Jenkins가 지원하는 자바 버전에 따라서, 어떤 OS 혹은 플랫폼에서도 실행될 수 있습니다. <br> 
   
  이론적으로, 젠킨스는 전통적인 서블릿 컨테이너인 Apache Tomcat 혹은 WildFly와 같은 것으로 서블릿으로 실행될 수 있으나, <br>
  실제로 이것은 대체로 테스트되지 않았고, 많은 결함이 있습니다. <br> 
   
  특별히, WebSocket agents에 대한 지원은 오직 Jetty Servlet Container에서 실행됩니다. <br>  
   
</details>

-----------------------

### 서블릿이란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.jenkins.io/doc/book/installing/] 
   
+  
   
</details>

-----------------------

### Jetty란?

<details>
   <summary> 답안 보기 (👈 Click)</summary>
<br />
[참고: https://www.eclipse.org/jetty/] 
   
+ Jetty는 웹 서버와 서블릿 컨테이너를 제공하고, 추가적으로 HTTP/2, WebSocket, OSGi, JMX, JNDI, <br>
  JAAS 그리고 다른 많은 integration을 위한 서포트를 제공합니다. <br> 
  이러한 요소들은 오픈 소스이고, 상업적인 사용과 배포를 위해 자유롭게 사용될 수 있습니다. <br> 
   
  Jetty는 다양한 프로젝트와 제품에 사용되고, 개발과 프로덕션 둘 다에 사용됩니다. <br> 
  Jetty는 쉽게 기기, 툴, 프레임워크, 어플리케이션 서버, 그리고 현대 클라우드 서비스에 내장될 수 있다는 점으로 인해<br>
  오랫동안 개발자들에 의해 사랑받아 왔습니다. <br>
   
  특징 <br>
  - 
</details>

-----------------------

