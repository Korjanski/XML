# XML
 1. Создать внешний репозиторий c названием XML.
зайти на сайт https://github.com
войти под своей учетной записью
нажать на вкладку Repositories
нажать на зеленую кнопку NEW
в поле Repository name ввести Xml
выбрать  Public
поставиь галочку Add a README file
нажать create repository


 2. Клонировать репозиторий XML на локальный компьютер.
нажать Code выбрать пункт Https
далее скопировать ссылку,зайти в папку,куда будет скопирован репозиторий
git clone https://github.com/Korjanski/XML.git

 3. Внутри локального XML создать файл “new.xml”.
git touch new.xml
git status файл new.xml не отслеживается(горит красным)


 4. Добавить файл под гит.
Добавить файл под гит.
git add new.xml (добавляем файл под гит)
git status new.xml отслеживается(горит зеленым)

5. Закоммитить файл.
git commit -m "add new.xml"

 6. Отправить файл на внешний GitHub репозиторий.
git push

 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.
vim new.xml
i

		<?xml version="1.0" encoding="UTF-8"?>
       <about_me>
                <name>Dergachev Sergey</name>
		<age>34</age>
		<home_pets>no</home_pets>
		<future_desire_salary>700$</future_desire_salary>
      </about_me>
esc
:wq

 8. Отправить изменения на внешний репозиторий.
git commit -am new.xml
git push

 9. Создать файл preferences.xml
touch preference.xml

 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.
   vim preferences.xml
   i
     <?xml version="1.0" encoding="UTF-8"?>
<preference>
        <favorite_movie>pulp fiction</favorite_movie>
	<favorite_serial>brassic</favorite_serial>
	<favorite_food>sushi</favorite_food>
	<favorite_time_of_the_year>summer</favorite_time_of_the_year>
	<country_i_would_like_to_visit>Great Britain</country_i_would_like_to_visit>
</preference>
esc
:wq

 11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML
cat>skills.xml
<skills>json,xml,txt,github,gitbash</skills>

Enter
Ctrl+D

 12. Сделать коммит в одну строку.
 git add .;git commit -m"add skills.xml,preference.xml"

 13. Отправить сразу 2 файла на внешний репозиторий.
 git push

 14. На веб интерфейсе создать файл bug_report.xml.
нажать add file
выбрать create new file
в поле name new file ввести bug_report.xml

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
нажать кнопку commit new file

 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.
открыть файл bug_report.xml
{"hello Kitty"}

 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.
нажать commit change


 18. Синхронизировать внешний и локальный репозиторий XML
git pull ввести в терминале
