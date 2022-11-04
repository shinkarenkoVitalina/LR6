# LR6

# Лабораторная работа №6

Певым шагом мы создаем копию репозитория https://github.com/Kurtyanik/LR6/ в личном хранилище. 

![1](https://user-images.githubusercontent.com/87824002/200065624-f956e2eb-c260-442a-8209-e93db56d0b59.jpg)

Затем настраиваем клиент git, вводим имя пользователя и email.

Комманды: git config --global user.name <username>; git config --global user.email <email>.

![2](https://user-images.githubusercontent.com/87824002/200066054-6b4c2f74-fe27-471a-a336-451b1215076f.jpg)

Клонируем удалённый репозиторий на компьютер.

Комманда: git clone.

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

Подробно рассмотрим коммиты ветки branch1.
Комманда: git log -p.

![14](https://user-images.githubusercontent.com/87824002/200072434-de5c2176-6aa7-4ea4-9995-31af44b1796b.jpg)

Возвращаемся обратно на ветку master.
Команда: git checkout master.

![15](https://user-images.githubusercontent.com/87824002/200072472-e6a645cd-19ba-443e-b85d-1766547776fc.jpg)

Выполняем слияние ветки branch1 в ветку master.
Комманда: git merge branch1.

![16](https://user-images.githubusercontent.com/87824002/200072526-f52de670-b7c4-41dd-902f-22f5812243ed.jpg)

Разрешаем возникший конфликт: в теории конфликт возник из-за того, что файл mergefile.txt не отслеживается. Проверив это и убедившись, добавляем файл для отслеживания, составляем коммит.
Проверим, есть ли файлы, которые не отслеживаются. Команда: git status.

![17](https://user-images.githubusercontent.com/87824002/200072560-383ba717-3039-478d-a3a6-538ee4109236.jpg)

Добавим файл для отслеживания. Команда: git add mergefile.txt.

![18](https://user-images.githubusercontent.com/87824002/200072602-1b55c7ea-c347-418a-8ba9-30a0b3dd5dc4.jpg)

Проверим, что больше не осталось неотслеживаемых файлов. Команда: git status.

![19](https://user-images.githubusercontent.com/87824002/200072629-869c6a28-9862-45b8-b9b8-801a8c602de3.jpg)

Создаем коммит. Команда: git commit -m "merge conflict of branch1->master resolved".

![20](https://user-images.githubusercontent.com/87824002/200072673-b1577387-ba7e-4b37-a578-245fd256e921.jpg)

Пушим (отправляем) наши локальные изменения в удаленный репозиторий.
Команды: git status; git push.

![21](https://user-images.githubusercontent.com/87824002/200072705-439d5cfa-923e-4683-89e5-aec530742725.jpg)
![22](https://user-images.githubusercontent.com/87824002/200072765-2e794707-2e61-45c1-b668-597c8ebfecd6.jpg)
  
Удаляем (локально) побочную ветку после успешного слияния.
Удаляем ветку branch1 локально. Команда: git branch -d branch1.

![23](https://user-images.githubusercontent.com/87824002/200073601-d00f708c-b79c-407b-82d1-d078cef0f8b3.jpg)

Проверяем, что локальная ветка удалена. Команда: git branch -a

![24](https://user-images.githubusercontent.com/87824002/200073656-3acc75ed-de7b-4e3c-94a4-d8909e5e1191.jpg)

 Добавляем (папку и файлы) изменения и фиксируем их (коммитим). Каждому изменения приписываем комментарий. Создаем папку и переходим в нее. Команды: mkdir changes; cd changes/.
  
![25](https://user-images.githubusercontent.com/87824002/200073844-fe74bb57-4bd8-41fe-8b55-679bbeef8b21.jpg)

Создаем файл, соержащий в себе данные о папке. Команда: echo "package LR6.changes;" > package-info.java.
  
![26](https://user-images.githubusercontent.com/87824002/200073895-8a812195-a7f5-4556-96ab-250abe1314c6.jpg)

Добавляем файл в отслеживаемые. Команда: git add package-info.java.

![27](https://user-images.githubusercontent.com/87824002/200073986-3217dfd2-ed20-4f75-a3f5-ded132c39ddc.jpg)

Создаем коммит. Команда: git commit -m "added new directory plus package-info".

![28](https://user-images.githubusercontent.com/87824002/200074017-4944ad3b-a9c1-4f3c-ad6d-497a96c07a0b.jpg)

Создаем пустой файл. Команда: echo "" > empty.txt.

![29](https://user-images.githubusercontent.com/87824002/200074057-05639768-3fb0-4699-abef-c3b2ff07b5ce.jpg)

Добавляем файл в отслеживаемые. Команда: git add empty.txt.

![30](https://user-images.githubusercontent.com/87824002/200074263-c1afab1b-1b56-415a-ba9a-1b3232e88397.jpg)

Создаем коммит. Команда: git commit -m "empty.txt added"

![31](https://user-images.githubusercontent.com/87824002/200074288-f4fbf93b-2b23-4d8c-a465-92c884bfa76b.jpg)

Сделаем откат последнего коммита.
Найдем идентификатоор последнего коммита. Команда: git log.
  
![32](https://user-images.githubusercontent.com/87824002/200074320-013bf5bd-2cf7-4c81-8b96-053f19bdfea6.jpg)

Скопируем id коммита и откатим его. Команда: git revert.
  
![33](https://user-images.githubusercontent.com/87824002/200074376-274b77bf-92f9-4283-8a7d-d018e2b1b637.jpg)
![34](https://user-images.githubusercontent.com/87824002/200074406-558f2f66-ad3c-4837-8306-ec0f8feb5219.jpg)
![35](https://user-images.githubusercontent.com/87824002/200074446-08a2f63c-7fcf-414c-a3c6-d59e0084f485.jpg)

Отправим (запушим) коммиты в удаленный репозиторий.
Проверка состояния контроля версий. Команда: git status.

![36](https://user-images.githubusercontent.com/87824002/200074523-45c4e97a-ec64-4482-9a70-f9c2413d9750.jpg)

Отправка коммитов. Команда: git push.

![37](https://user-images.githubusercontent.com/87824002/200074547-fea560df-f00e-4206-9032-f4fb6d473d2b.jpg)

Проверяем, что все запушили. Команда: git status.
  
![38](https://user-images.githubusercontent.com/87824002/200074570-3522df80-e200-4da7-885c-4c97dc732d12.jpg)

Создаем ветку для отчёта.
Создаем ветку report. Комманда: git branch report.

![39](https://user-images.githubusercontent.com/87824002/200074741-e5ab4ba2-321c-4c1b-a871-8791c0fa31ae.jpg)

Переходим на ветку report. Команда: git checkout report.

![40](https://user-images.githubusercontent.com/87824002/200074812-b2358911-0814-4b23-b950-1915880d1a36.jpg)

Создаем пустой файл отчета — README.md. Команда: echo "" > READEME.md.

![41](https://user-images.githubusercontent.com/87824002/200074827-c6df9452-5a19-4469-806c-a49b36b5e95e.jpg)

Добавляем отчет в систему контроля версий. Команда: git add README.md.

![42](https://user-images.githubusercontent.com/87824002/200074844-7bd03f3a-7c1d-455e-a20a-8a283c22dabf.jpg)

Создаем коммит с пустым отчетом. Команда: git commit -m "added README.md empty report".

![43](https://user-images.githubusercontent.com/87824002/200074866-6203eea7-4819-439d-962a-b1f43bf1b734.jpg)

Получаем итоговую историю операций в форматированном виде (сокращённый хэш - дата, имя автора : комментарий).
Комманда: git log --pretty=format:"%h - %ar, %an : %s".

![44](https://user-images.githubusercontent.com/87824002/200074950-06716f39-4c1d-4bab-a410-1077520a974b.jpg)

Оформляем отчёт в файле README.md. 
После редактирования отчета, его нужно будет сохранить и закоммитить git commit.
В конце работы необходимо будет запушить все локальные изменения в сетевое хранилище GitHub командой git push.

Все снимки экрана, используемые в этом отчете находятся в папке img.
