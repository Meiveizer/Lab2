Державний вищий навчальний заклад Ужгородський національний університет Факультет інформаційних технологій

ЛАБОРАТОРНА РОБОТА №5 Тема: Деплой проекту на AWS EC2

Виконав студент ІIІ курсу Напрям: ІПЗ-2.2 тернинко Василь Васильович

Ужгород-2022 

Хід роботи 
1.Спочатку ми зареєструвалися на AWS. Після чого створюємо інстанс EC2

![1](https://user-images.githubusercontent.com/99879459/225592262-ce8b1530-8418-4414-b350-b4ae337d65f2.png)
![2](https://user-images.githubusercontent.com/99879459/225592451-f5bc1ae8-ea41-42e7-9166-5cf4439c5ec9.png)

Натиснувши на кнопку Connect бачу інструкцію для деплою проекту
![3](https://user-images.githubusercontent.com/99879459/225592567-5039de7e-7b07-4c03-917b-5fb1372b6bcb.png)
Виконуємо команду chmod 400 golf.pem для того щоб запевнитися що наш ключ не є загально доступним Підключаємося до EC2 за допомогою
ssh -i "golf.pem" ec2-user@ec2-3-72-10-164.eu-central-1.compute.amazonaws.com

![4](https://user-images.githubusercontent.com/99879459/225593645-a01de538-bcf7-4436-a7ea-b693d9a6332d.png)
Запускаємо сервіс systemctl start httpd.service

![6](https://user-images.githubusercontent.com/99879459/225594157-62ea1ce1-fa5b-4c84-8f01-56be8e34923c.png)
![5](https://user-images.githubusercontent.com/99879459/225594182-4ab9f216-ea80-4d10-b7be-ee4330044b65.png)
![7](https://user-images.githubusercontent.com/99879459/225594219-a9ef04d5-bdba-42d7-a7a6-497c55a17565.png)

Бачимо результат по ip-адресі 3.72.10.164 

Висновки: на цій лабораторній роботі я навчився створювати інтанси у EC2 , і деплоїти свій проект на AWS EC2.
