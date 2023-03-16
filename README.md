Державний вищий навчальний заклад Ужгородський національний університет Факультет інформаційних технологій

ЛАБОРАТОРНА РОБОТА №3 Тема: Docker

Виконав студент ІIІ курсу Напрям: ІПЗ-2.2 Тернинко Василь 
Ужгород-2022 Хід роботи

1.Використання готових Docker Images. Спочатку я створив папку Docker з файлом docker-compose.yml
![3](https://user-images.githubusercontent.com/99879459/225441672-9109e801-6c24-4c3b-811b-be22e765625f.png)
![4](https://user-images.githubusercontent.com/99879459/225441691-e091cb79-1d61-483f-9149-220df35026c9.png)

2.Використання Docker Compose. Docker Compose — інструментальний засіб, що входить до складу Docker. Він призначений для вирішення завдань, пов'язаних із розгортанням проектів: Docker Compose використовується для одночасного керування кількома контейнерами, що входять до складу програми. Цей інструмент пропонує ті ж можливості, що й Docker, але дозволяє працювати з більш складними програмами. Для налаштування служб програми у Docker Compose використовується конфігураційний файл з розширенням .yml. Тобто спочатку створюється файл YAML, де будуть прописані налаштування служб, а після цього за допомогою команди docker compose -d створюються та запускаються всі служби з нього. YAML — зручний для читання людиною формат серіалізації даних, концептуально близький до мов розмітки; у Docker Compose використовується для налаштування служб програм. Переваги YAML: • YAML короткий і зрозумілий, легко читається та пишеться; • YAML використовує структури даних, характерні для мов програмування; • Синтаксис YAML мінімальний у порівнянні з XML; • Підтримує коментарі на відмінно від JSON; • Підтримує рядки без лапок.

Недоліки YAML: • Строгість у відступах: якщо ви неправильно вставите один пробіл під час відступу, код може перестати працювати. • Легше знайти підтримку XML, JSON замість YAML. • JSON і XML мають кращу продуктивність, ніж YAML. Приклад створення та збирання образа за допомогою Docker Compose - виконання завдання 1. 3. Створення HTML сторінки та занесення її в Docker Image. Залити даний Docker Image на Docker Hub. 

Спочатку ми залогінилися до DockerHub
![5](https://user-images.githubusercontent.com/99879459/225442042-b864277d-2154-43b2-922d-01e361ccbaea.png)
Потім я за допомогою build створив docker image і за допомогою docker run перевірив на працездатність мій контейнер
![6](https://user-images.githubusercontent.com/99879459/225442127-3c5571fb-fad4-4064-be6d-362bf1360c20.png)
![7](https://user-images.githubusercontent.com/99879459/225442253-ec1fb791-2681-4334-8627-cb69c4142b6a.png)
![8](https://user-images.githubusercontent.com/99879459/225442284-5dbfad30-ba52-475b-b201-edc9d4ad41aa.png)
Я перейменував свій локальний репозиторій за допомогою docker tag lab3:latest 
meiveizer/lab3:latest і запушив за допомогою docker push meiveizer/lab3:latest
![10](https://user-images.githubusercontent.com/99879459/225588344-6f51785b-d71c-4da3-921f-ace5c92488a1.png)
Бачимо залитий репозиторій на DockerHub ( https://hub.docker.com/repository/docker/meiveizer/lab3/general ) 

4. Скачати Docker Image когось із групи і розвернути в себе контейнер з HTML сторінкою на порті 8086 ззовні. Для виконання цього завдання я скачаю Docker Image мого однокурсника Русина Олександра (https://hub.docker.com/r/sasharusyn/docker_lab3).
![11](https://user-images.githubusercontent.com/99879459/225589171-eae50ec5-4dab-4022-8291-ceb51af2bd01.png)
![12](https://user-images.githubusercontent.com/99879459/225589215-b8e09ee2-e3e4-4cbd-a6fb-f35b36a6c4a2.png)

Висновки: на цій лабораторній роботі я навчився працювати з Docker, використовувати готові DockerImage та працювати з DockerCompose, створювати теги, робити push та стягувати готові DockerImage.
