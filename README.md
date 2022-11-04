# LR6

# Лабораторная работа №6

Певым шагом мы создаем копию репозитория https://github.com/Kurtyanik/LR6/ в личном хранилище. 

![1](https://user-images.githubusercontent.com/87824002/200065624-f956e2eb-c260-442a-8209-e93db56d0b59.jpg)

Затем настраиваем клиент git, вводим имя пользователя и email.

Комманды: git config --global user.name <username>; git config --global user.email <email>.

![2](https://user-images.githubusercontent.com/87824002/200066054-6b4c2f74-fe27-471a-a336-451b1215076f.jpg)

Клонируем удалённый репозиторий на компьютер.

Комманда: git clone <url>.

![3](https://user-images.githubusercontent.com/87824002/200066364-b3024ffc-d22f-4f0e-91bb-c390dc83c0e5.jpg)

Проверяем, что при клонировании репозитория, все файлы из удаленного репозитория перешли в локальный.

Команда: git pull.

![5](https://user-images.githubusercontent.com/87824002/200066460-744670c7-c9b2-4cd5-8a74-389b23ace5d7.jpg)

Добавляем файл через интерфейс GitHub.

Нажимаем на кнопку Add file, затем на Create new file.

![6](https://user-images.githubusercontent.com/87824002/200066646-2a68cc81-3bc9-4349-bc7a-95b8b4f7d713.jpg)

С помощью появившегося интерфейса вводим название файла и его содержимое.

![7](https://user-images.githubusercontent.com/87824002/200066683-cfac7a51-3f3a-41a5-9972-cc8c3d1f9a40.jpg)

Прописываем комментарий к коммиту и соответственно делаем сам коммит

![8](https://user-images.githubusercontent.com/87824002/200066892-187406b0-5109-4923-9012-e32e1071be0d.jpg)

В итоге файл появляется в репозитории на GitHub

![9](https://user-images.githubusercontent.com/87824002/200066975-408db0e8-4c1c-4ef0-a8cc-8792ddc63a6e.jpg)

Поддтягиваем изменения с удаленного репозитория в локальный.

Комманда: git pull.

![10](https://user-images.githubusercontent.com/87824002/200067033-0d3c0a66-802e-47ee-91f2-aa3c785e6a0f.jpg)

Посмотрим коммиты веток

Коммиты ветки master. Комманда: git log.

![11](https://user-images.githubusercontent.com/87824002/200067078-34b9620a-ae58-4c2e-b347-de0328a4fa42.jpg)

Переходим на вторую ветку branch1. Команда: git checkout branch1

![12](https://user-images.githubusercontent.com/87824002/200067111-c42cae25-6fe6-4afe-b12c-9aaaea5a0b1b.jpg)

Коммиты ветки branch1. Комманда: git log

![13](https://user-images.githubusercontent.com/87824002/200067167-84fcadbf-65a2-4d46-bdb5-58da882a1191.jpg)
