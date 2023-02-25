# Spring-FrameWork-study

Spring Framework

IoC 컨테이너
  - IoC (Inversion of Control) : 제어 역전
  - 일반적으로 프로그래밍을 작성할 때 프로그램이 흘러가는 흐름이나 생성되는 객체에 대한 제어권을 개발자가 만드는
    개발자가 가지는 것과 달리 프레임워크가 가지는 것을 의미한다.
  - 개발자가 코드의 흐름이나 객체 생성에 관련된 코드를 프로그래밍 코드에 직접 작성하는 것이 아닌 프레임워크가 사용하는 
    파일에 작성하면 이를 토대로 프레임워크가 객체를 생성하여 반환하고 코드가 동작하는 순서를 결정하게 된다는 의미이다.

IoC 컨테이너 종류
  - BeanFactory
	클래스를 통해 객체를 생성하고 이를 전달한다.
	상속 등 객체 간의 관계를 형성하고 관리한다.
	Bean에 관련된 설정을 위한 xml 파일은 즉시 로딩하지만 객체는 개발자가 요구할 때 생성한다.
	XmlBeanFactory
  - ApplicationContext
	클래스를 통해 객체를 생성하고 이를 전달한다.
	상속 등 객체 간의 관계를 형성하고 관리한다.
	국제화 지원 등 문자열에 관련된 다양한 기능을 제공한다.
	리스너로 등록되어 있는 Bean에 이벤트를 발생시킬 수 있다.
	Bean에 관련된 설정을 위한 xml 파일은 즉시 로딩하면서 객체를 미리 생성해서 가지고 있다.
	ClassPathXmlApplicationContext
	FileSystemXmlApplicationContext
	XmlWebApplicationContext

☆ 스프링 프레임워크는 IoC 컨테이너를 이용해 Bean 객체들을 관리한다.

POJO Class
  - POJO (Plain Old Java Object) : 자바 모델이나, 기능, 프레임워크 등에 따르지 않고 홀로 독립적이며 단순한 기능만을 가진
    객체들을 의미한다. (VO 나 DAO 같은 MVC 에서 Model 을 의미)
  - Java 에서는 이러한 객체들을 Bean이라고 부른다
  - POPO(PHP), POCO(닷넷 프레임워크), PODS(C++), POD(Perl) 등
