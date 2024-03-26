---
description: >-
  클라우드 컴퓨팅은 인터넷으로 가상화된 IT 리소스를 서비스로 제공하는 것을 의미합니다. 그리고 클라우드 컴퓨팅에서 가상화하여 서비스로
  제공하는 대상은 서버, 플랫폼, 소프트웨어
---

# 클라우드란

AWS, Azure,GCP가 대중화되면서 클라우드를 인프라스트럭처의 가상화 개념으로만 이해하기도 하지만 클라우드는 인프라스트럭처 뿐만이 아니라 플랫폼과 소프트까지 포함하는 온라인의 모든 영역을 다루는 꽤 광범위한 개념입니다. 그렇기 때문에 클라우드는 분야별 특성별로 나누어서 이해가 필요하다.

클라우드는 그 형태에 따라서 아래와 같은 몇가지 형태로 나뉘어 진다.&#x20;

* Infrastructure as a Service(IaaS, 아이아스, 이에스)서비스로 제공되는 인프라스트럭처입니다. 개발사에 제공되는 물리적 자원을 가상화합니다.
* Platform as a Service(PaaS, 파스)서비스로 제공되는 플랫폼입니다. 개발사에 제공되는 플랫폼을 가상화합니다.
* Software as a Service(SaaS, 사스)서비스로 제공되는 소프트웨어입니다. 고객에게 제공되는 소프트웨어를 가상화합니다.

일반적인 시스템 개발자 입장에서는 가장 많이 사용하는 부분이 Saas형태의 서비스이나 Saas를 Cloud환경에 적용하면서 자동으로 Iaas 및 Paas환경을 사용하게 된다.

<figure><img src=".gitbook/assets/image (6).png" alt=""><figcaption></figcaption></figure>

1.  IaaS : 물리적 자원 제공

    IaaS는 고객에게 서버, 네트워크, OS, 스토리지를 가상화하여 제공하고 관리합니다. IaaS는 가상화된 물리적인 자산을 UI 형태의 대시보드 또는 API로 제공합니다. IaaS의 고객들은 서버와 스토리지를 접근할 수 있지만 사실상 클라우드에 있는 가상 데이터 센터를 통해 리소스를 전달받는 형태입니다. IaaS는 기존의 데이터센터에서 제공받던 물리적인 자산을 완벽하게 가상화하여 제공하기 때문에 서버 사양의 변경 등 물리적 자산의 수정이 필요한 경우 기존의 방식에 비해 훨씬 빠른 대응이 가능합니다.

    IaaS의 제공업체는 서버, 하드 드라이브, 네트워킹, 가상화 및 스토리지를 관리하며 고객은 OS, 미들웨어, 애플리케이션 및 데이터와 같은 자원들을 관리해야 합니다.
2.  PaaS : 소프트웨어 개발을 돕는 플랫폼 제공

    PaaS는 고객에게 OS, 미들웨어, 런타임과 같은 소프트웨어 작성을 위한 플랫폼을 가상화하여 제공하고 관리합니다. 이 가상화된 플랫폼은 웹을 통해 제공되며 개발자는 운영체제, 소프트웨어 업데이트, 저장소 또는 인프라에 대한 관리없이 소프트웨어 개발에 집중할 수 있습니다.

    PaaS를 사용하면 기업에서는 특수 소프트웨어 구성 요소를 사용하여 PaaS에 내장된 응용 프로스램을 설계하고 만들 수 있습니다. 이러한 응용 프로그램 또는 미들웨어는 특정 클라우드 특성을 채택할 때 확장 가능하고 가용성이 높습니다.
3.  SaaS : 고객이 사용하는 소프트웨어 제공

    SaaS는 고객을 대신하여 소프트웨어와 데이터를 제공하고 관리합니다. 패키지 또는 On-premise 방식인 기존의 소프트웨어 전달 방식과 다르게 SaaS는 개별 컴퓨터에 응용 프로그램을 다운로드하고 설치할 필요가 없습니다. SaaS를 통해 서비스를 공급하는 업체는 데이터, 미들웨어, 서버 및 스토리지와 같은 모든 잠재적인 기술적 문제를 관리하기 때문에 고객은 유지 보수 및 자원을 간소화하면서 비즈니스에 집중할 수 있습니다.



### 서비리스

클라드우가 발전되면서 위의 3가지 형태를 벗어난 서버리스 형태의 서비스도 나타 났다.

의미는 클라우드 서비스 공급자가 서버를 관리, 실행하며, 요청이나 특정 이벤트가 있을 때 클라우드의 서버를 이용하거나 서비스 할 어플리케이션을 동작시키는 것. 이를 통해 사용자(개발자)는 서버 관리에서 완전히 자유로워지며 실제 구현해야 할 기능에 더 집중할 수 있게 됨.

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption><p>ㅇ <a href="https://www.einfochips.com/blog/serverless-architecture-the-future-of-software-architecture/">https://www.einfochips.com/blog/serverless-architecture-the-future-of-software-architecture/</a></p></figcaption></figure>

서버리스는 보통 '서버리스 컴퓨팅' 또는 '서버리스 아키텍처'로 불린다. 서버리스 개념은 어플리케이션 관점에서 BaaS(Backend as a Service)와 FaaS(Function as a Service)로 나누어 살펴보면 이해가 더 용이하다.

1. **Backend-as-a-Service (BaaS)**

It is more like the SaaS (software-as-a-service) for application development rather than business processing. In BaaS paradigm, an application developer can just focus on writing code or business functionality and do not need to worry about provisioning and maintaining servers to run the code. In this concept, the code will be run on some third party vendor server or infrastructure.

In most cases, the BaaS services run continuously once they are started.  Hence, enterprises need to pay for these services regardless of whether the code is running or not. Backend-as-a-service offers generic components that can be plugged into an application, especially as the generic backend have a custom front-end component. 현재 주된 사용 대상이 모바일 앱과 웹 앱(WebApp)이다 보니 MBaaS(Mobile Backend as a Service)라 불리는 시장이 활성화 되는 추세. 클라우드 데이터베이스 서비스인 Firebase나 클라우드 인증 서비스인 Auth0가 BaaS에 해당됨.

* **예) Authentication:** 많은 애플리케이션에는 가입, 로그인, 비밀번호 관리 및 다른 인증 장치와의 통합과 같은 인증 논리가 필요하다. 대부분의 코드는 여러 애플리케이션에서 매우 유사합니다. Auth0 및 Amazon Cognito와 같은 제품에는 기능이 내장되어 있으므로 이 기능을 직접 개발할 필요 없다.

<figure><img src=".gitbook/assets/image (2).png" alt=""><figcaption><p><a href="https://www.samsungsds.com/kr/insights/1232763_4627.html">https://www.samsungsds.com/kr/insights/1232763_4627.html</a></p></figcaption></figure>

2. **Function-as-a-Service (FaaS)**

FaaS는 사용자가 쓸 기능을 함수 단위로 나누어 구현하고 이를 서비스하는 형태입니다. FaaS는 Event-Driven 아키텍처를 구현하는데 적합하며 사용자가 원하는 기능을 미리 작성해놓고 특정 이벤트(예를 들어 HTTP Request, API 호출, 특정 조건 등)에 의해 실행된다. 이때 서버는 계속 대기하면서 이벤트를 기다리지 않고 이벤트가 발생할 때마다 실행됩니다. 비용은 서버가 실행된 횟수와 시간(밀리세컨드. 1,000분의 1초)에 따라 산정된다. FaaS를 구현한 대표적인 서비스로 AWS의 Lambda, 마이크로소프트의 Azure Functions, 구글의 Google Cloud Functions 등이 있다.\


<figure><img src=".gitbook/assets/image (5).png" alt=""><figcaption></figcaption></figure>

1. Customers leverage your microservices by making HTTP API calls. Ideally, your consumers should have a tightly bound service contract to your API to achieve consistent expectations of service levels and change control.
2. Amazon API Gateway hosts RESTful HTTP requests and responses to customers. In this scenario, API Gateway provides built-in authorization, throttling, security, fault tolerance, request and response mapping, and performance optimizations.
3. AWS Lambda contains the business logic to process incoming API calls and use DynamoDB as a persistent storage.
4. Amazon DynamoDB persistently stores microservices data and scales based on demand. Since microservices are often designed to do one thing well, a schemaless NoSQL data store is regularly incorporated.
