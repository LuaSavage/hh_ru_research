# hh_ru_research
Проект реализован в учебных целях анализа рынка труда, в особенности по hh.ru

## Input data
В качестве входных данных используются сериализованные json объекты вакансий, расположенные в json/  
Для их генерации был использован парсер [LuaSavage/hh_ru_parser](https://github.com/LuaSavage/hh_ru_parser)  
Последующие ячейки кода преобразуют эти json объекты в pandas dataframe.  
Dataframe'ы сохраняются в csv/ и могут быть использованы повторно  

## Output data
В качестве выходных данных можно получить следующее:
* Поисковой текст
* Средняя зарплата
* Медианная зарплата
* Среднеквадратичное отклонение зарплаты
* Число вакансий
* Число вакансий с открытой зарплатой
    + в абсолютных значениях
    + в относительных значениях  
* Число вакансий без нижней или верхней границы зарплаты:
    + в абсолютных значениях
    + в относительных значениях      
* Вакансии с максимальной зарплатой  
![Vacancies with max salary](img/max_salary.jpg "Vacancies with max salary")
* Вакансии с минимальной зарплатой  
![Vacancies with min salary](img/min_salary.jpg "Vacancies with min salary")
* Гистограмма распределения зарплат  
![Salary histogram](img/salary_hist.png "Salary histogram")
* Круговые диаграммы графика работы и наличия возможности временного трудоустройства
* Анализ списка технологий по ключевым навыкам
![Key skills](img/key_skills.jpg "Key skills")
* Анализ списка технологий по описанию
![Key skills from description](img/description.jpg "Key skills from description")
