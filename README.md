### Notion Link
[Annotation Processor](https://boklog.notion.site/Annotation-Processor-4b25122370144de88b3c2ea117c1c2c1)

### Using Sample
실제 작동 하는 코드 생성을 보려면 공통 상위 루트에서 두 모듈을 모두 컴파일하거나 processor 모듈을 컴파일 한 다음 user 모듈을 컴파일 해야합니다.
생성된 PersonBuilder 클래스는 annotation-user/target/getnerated-sources/annotations/org/example/annotation/PersonBuilder.java 파일 내에서 찾을 수 있으며 다음과 같아야 합니다.

```java
package org.example.annotation;

public class PersonBuilder {

    private Person object = new Person();

    public Person build() {
        return object;
    }

    public PersonBuilder setName(java.lang.String value) {
        object.setName(value);
        return this;
    }

    public PersonBuilder setAge(int value) {
        object.setAge(value);
        return this;
    }

}
```

![image](https://user-images.githubusercontent.com/45517663/208384616-a7b2ee6a-e85a-41d9-89e0-047415f0f810.png)
