# HH-api
get info from HH.ru

* Read me will be translated into english later

В репозитории 2 файла: 
1 - создан для получения информации при поиске по вакансиям (см. Поиск по вакансиям https://github.com/hhru/api/blob/master/docs/vacancies.md#search) и отдает файлы со следующей информацией: 
- распределение вакансий по опыту работы
- распределение вакансий по гео
- распределение вакансий по компаниям
- распределение средних значений нижней границы з/п по городам и опыту работы
- распределение средних значений з/п (для вакансий, в которых указана "вилка" зарплат) по городам и опыту работы
- распределение средних значений з/п (для вакансий, в которых указана "вилка" зарплат) по компаниям и опыту работы
- топ-100 слов из требований к вакансиям

2 - создан для получения информации по навыкам из раздела Просмотр вакансии (см. Просмотр вакансии https://github.com/hhru/api/blob/master/docs/vacancies.md#item) и отдает файл, в котором навыки распределены по частоте для каждого опыта работы

Для корректного запроса необходимо правильно указать: 
- наименование искомой вакансии и правильная комбинация нахождения ключевых слов в названии / описании(см. Язык поисковых запросов https://hh.ru/article/1175)
- необходимое гео поиска (по умолчанию в код включены вакансии из России, Украины, Казахстана и Беларуси)
- дополнительно указываемые параметры можно просмотреть в разделе Поиск по вакансиям (https://github.com/hhru/api/blob/master/docs/vacancies.md#search)

Важно! каждый запрос отдает не более 2 000 вакансий. В случае, если искомое количество вакансий превышает 2 000 для каждого уровня опыта, можно продублировать запрос, указав в нем дополнительные принимаемые параметры.
