# Сервис логирования для использования в spring-boot приложениях
##  Maven
```xml
<repositories>
        <repository>
            <id>github</id>
            <url>https://maven.pkg.github.com/vyacheslavchernov/logger-spring-boot-starter</url>
        </repository>
</repositories>
```

Актуальную версию [см. здесь](https://github.com/vyacheslavchernov?tab=packages&repo_name=logger-spring-boot-starter)
```xml
<dependency>
    <groupId>ru.vych</groupId>
    <artifactId>logger-spring-boot-starter</artifactId>
    <version>0.0.1-RELEASE</version>
</dependency>
```

## Конфигурация application.yaml
Без конфигурации будет активно только логирование в консоль.

Пример минимального конфига с другими методами записи лога
```yaml
logger:
  console:
    enabled: true # По умолчанию true
    level: DEBUG # По умолчанию INFO
```
Все проперти можно посмотреть в [LogProperties.java](src/main/java/ru/vych/logger/config/LogProperties.java)