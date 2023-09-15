# Портфолио: инженер по тестированию

## Обо мне 🙋‍♂️

Привет! Меня зовут Андрей, я начинающий тестировщик. <br>
В этом репозитории вы можете найти некоторые из моих проектов, выполненных во время обучения и практики.
<br>

## Навыки и технологии 💻
``Jira``,``qase.io``,``SQL``,`` Postman``,``Fiddler``, ``Swagger``, ``Trello``, <br>
``SoapUI``, ``Android Studio``, ``xCode``, ``Charles``, ``Git``, ``Chrome DevTools``.


## Проекты ✍️

##  Проект : тест веб-приложения для учителей от Skyeng
<p> Описание проекта и задач: Skyeng — это онлайн-школа английского языка, которая помогает людям, поставившим перед собой конкретные жизненные цели, достичь их в процессе обучения. Платформой также пользуются преподаватели, в системе они могут планировать уроки и составлять расписание занятий.</p>
<p>Что нужно было сделать: Проверить новый программный продукт для учителей -  раздел «Личные события» на вкладке «Расписание». Преподаватель может использовать личные события для собственных встреч. Они служат напоминанием, что у преподавателя что-то запланировано на это время.<p>
<ol>
  <li>Задача №1: Проверить функционал "Добавление личного события" </li>
  <li>Задача №2: Проверить функционал "Удаление личного события"</li>
  <li>Задача №3: Проверить функционал "Редактирование личного события"</li>
  <li>Задача №4: Проверить функционал "Совмещение личного события и урока"</li>
</ol>

## Как решал: краткое описание решения:
Решение поставленных задач проходило в 3 этапа:<br>
<br> Этап №1.
<li>Знакомство с требованиями документации, тестирование требований.</li> - (https://skyengpublic.notion.site/6746e543d02c43879de0057cafe196b0)
<li>Составлен тест-план проекта, в котором я отразил главные сведения о тестировании функционала системы, описал основные функции программного продукта, отразил виды и сроки тестирования.</li> - (https://www.notion.so/cc39032b5b1e44cea494fb0df1ef534a?pvs=4)
<li>Составлена декомпозиция системы. Это позволило мне рассмотреть продукт как элемент состоящий из независимых друг от друга нескольких частей, блоков, каждый из которых тестировать гораздо проще и понятнее, чем всю программу сразу. - (https://miro.com/app/board/uXjVMVesfH4=/?share_link_id=876576365617)</li>

<br> Этап №2.
<li>Проведены smoke тесты, что позволило мне понять насколько стабильно работает продукт и увидеть наличие явных ошибок в работе системы (было составлено 3 тест кейса в системе QASE.IO).</li> - (https://app.qase.io/public/report/41f45e99f8cf902da86eefcada264a93ae3fe208)
<li>Проведено приемочное тестирование - оно позволило проверить продукт на соответствие требованиям пользователей (было составлено 3 тест кейса в системе QASE.IO).</li> - (https://app.qase.io/public/report/41f45e99f8cf902da86eefcada264a93ae3fe208)
<li>Проведено функциональное, нефункциональное и регресс-тестирование, тем самым было установлено соответствие системы заданным функциональным требованиям. Для функционального, нефункционального и регресс-тестирования было сформировано по 1 чек-листу (всего 78 тестов). Чек-листы были сформированы в системе Sitechco.</li> - (https://docs.google.com/spreadsheets/d/1b68PV8-pUAJuqzPsLmkKjYHoacK9yM7HMFH7vS8jReY/edit?usp=sharing)

<br> Этап №3.
<li>Изучение документации API.</li> 
<li>Проведение тестирования API. Создание Postman-коллекции. Определение надежности, безопасности и масштабируемости соединений между платформами.</li>  
<li>Отчёт о тестировании. Для удобного предоставления информации о тестировании мною были составлены основные метрики и отчетность по проекту, а также заведены отчеты о найденных ошибках в системе Jira. На основании найденных ошибок были составлены выводы о проделанной работе и написаны рекомендации по устранению основных ошибок в системе.</li> 

## Ссылка на проект:
> <a href="https://www.notion.so/Skyeng-e25f15f1c8a84e8fb414928420513d1d?pvs=4](https://onyx-wok-e34.notion.site/Skyeng-e25f15f1c8a84e8fb414928420513d1d?pvs=4)">Проект SkyEng</a>
 
 ## Выводы (итоги):
<br>
  <p>В результате проведенного тестирования были выявлены следующие баги:<p>
  <li>Баг №1: Нельзя было ввести дату вручную при добавлении личного события. Серьезность этому багу была выставлена S3 (Значительная), Приоритет - Средний. Данная функция не работает, но в целом на функционал системы не влияет.</li>
  <li>Баг №2: Нельзя было ввести дату вручную при добавлении нового урока. Серьезность этому багу была выставлена S3 (Значительная), Приоритет - Средний. Данная функция не работает, но в целом на функционал системы не влияет.</li>
  <li>Баг №3: Нельзя выбрать ученика при добавлении нового урока. Регресс тестирования показало, что функция добавления учащегося не работает. Серьезность была выставлена S2 (Критическая), Приоритет - Наивысший. Ключевая функция перестала работать.</li>
  <li>Баг №4: Во время тестирования API после запроса при введении некорректных значений в тело запроса на создание нового события некорректно отображается код ответа. Приходит код 200 , вместо кода 400. На основании этой ошибки было заведено 5 багов.</li>
  <li>В первую очередь надо исправить баг по добавлению учащегося, это ключевая функция при создании нового урока , данный баг является высоким по приоритету и его надо исправить в первую очередь, после чего данный продукт “Личные события” можно будет выпустить на портал. Баги связанные с добавлением даты вручную (при создании личного события и урока) также рекомендуется исправить, так как со стороны пользователя (учителя) будет удобно вносить дату вручную вместо того чтобы искать её из списка. Также стоит исправить отображение корректного кода ответа на невалидные запросы для отображения достоверной информации о запросе. </li>
</ol>
  <p>Чему я научился:<p>
<li> 1) Составлять отчеты о проведенном тестировании.</li>

<br> 


## Контактная информация 🤙
📫 Email: mr.korobeynikov-90@yandex.ru
