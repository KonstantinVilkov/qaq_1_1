# qaq_1_1
## Задача №1 - CashbackHacker
Вы участвуете в проекте CashbackHacker - небольшой сервис, который сообщает пользователю о том, сколько ему нужно "докупить" в рамках конкретной траты, чтобы получить максимальное количетство кэшбека.

Подробнее: кэшбек начисляется за каждую потраченную полную тысячу рублей, поэтому если вы покупаете что-то на 900 рублей, сервис должен посоветовать вам докупить "ещё чего-нибудь" на 100 рублей.

Код сервиса выглядит следующим образом:
```java
package ru.netology.service;

public class CashbackHackService {
    private final int boundary = 1000;

    public int remain(int amount) {
        return boundary - amount % boundary;
    }
}
```
Вам нужно создать проект на базе Gradle (как на лекции), добавить в него JUnit 5 (прописать их в build.gradle) и написать авто-тесты, которые тестируют функциональность этого сервиса (как минимум, два).

В сервисе точно есть ошибка, поэтому один из ваших авто-тестов должен падать.
