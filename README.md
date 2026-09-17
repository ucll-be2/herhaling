# Backend 2 - Herhaling

Dit project frist de belangrijkste basisconcepten uit **Backend 1** op:
- RESTful API's bouwen met Spring Boot
- Data ophalen en bewaren met Spring Data JPA
- Businesslogica implementeren in service classes
- Exceptions afhandelen in controllers
- Unit testen van service classes met mocking

De applicatie bevat een eenvoudige API rond acteurs en films. Ze gebruikt een in-memory **H2-database**. Voor de service classes zijn er unit tests voorzien met **JUnit 5** en **Mockito**.

## Projectstructuur

- [`src/main/java/.../controller`](./src/main/java/be/ucll/backend2/controller): REST-controllers voor actors en movies
- [`src/main/java/.../service`](./src/main/java/be/ucll/backend2/service): businesslogica
- [`src/main/java/.../repository`](./src/main/java/be/ucll/backend2/repository): JPA-repositories en initiële data
- [`src/main/java/.../model`](./src/main/java/be/ucll/backend2/model): domeinmodellen
- [`src/main/resources/application.properties`](./src/main/resources/application.properties): configuratie van de applicatie
- [`src/main/resources/schema.sql`](./src/main/resources/schema.sql): SQL-script om de database te initialiseren
- [`src/test/java/.../unit`](./src/test/java/be/ucll/backend2/unit): unit tests van de service classes
- [`bruno/`](./bruno): Bruno-collectie om de API te testen

## API testen met Bruno

In de map `bruno/` staat een collectie met requests om de applicatie manueel te testen. Je kan deze collectie openen in [Bruno](https://www.usebruno.com/).
