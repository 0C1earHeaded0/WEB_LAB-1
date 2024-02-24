<p align = "center">МИНИСТЕРСТВО НАУКИ И ВЫСШЕГО ОБРАЗОВАНИЯ<br>
РОССИЙСКОЙ ФЕДЕРАЦИИ<br>
ФЕДЕРАЛЬНОЕ ГОСУДАРСТВЕННОЕ БЮДЖЕТНОЕ<br>
ОБРАЗОВАТЕЛЬНОЕ УЧРЕЖДЕНИЕ ВЫСШЕГО ОБРАЗОВАНИЯ<br>
«САХАЛИНСКИЙ ГОСУДАРСТВЕННЫЙ УНИВЕРСИТЕТ»</p>
<br><br><br><br><br><br>
<p align = "center">Институт естественных наук и техносферной безопасности<br>Кафедра информатики<br>Шинкаренко Кирилл Константинович</p>
<br><br><br>
<p align = "center"><br><strong>Лабораторная работа №1.</strong><br>01.03.02 Прикладная математика и информатика</p>
<br><br><br><br><br><br><br><br><br><br><br><br>
<p align = "right">Научный руководитель<br>
Соболев Евгений Игоревич</p>
<br><br><br>
<p align = "center">г. Южно-Сахалинск<br>2024 г.</p>
<br><br><br><br><br><br><br><br><br><br><br><br>

<h1 align = "center">Введение</h1>

<p><b>HTML</b>(от англ. HyperText Markup Language — «язык гипертекстовой разметки») — стандартизированный язык гипертекстовой разметки документов для просмотра веб-страниц в браузере.</p>
<p>Попробуем написать страницу о себе.</p>

<br>
<h1 align = "center">Цели и задачи</h1>


<p>Требуется сверстать простую страницу о себе.</p>
<p>Необходимо: </p>
<ol>
	<li>Изучить основы HTML/CSS</li>
	<li>Продумать дизайн сайта.</li>
	<li>Определить необходимые классы и блоки.</li>
	<li>ВЁРСТКА!</li>
</ol>

<h1 align="center">Решение</h1>
<h2 align="center">Файл index.html</h2>

```
<!DOCTYPE html>

<html lang="ru">

<head>

  <link rel="preconnect" href="https://fonts.googleapis.com">

  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&display=swap" rel="stylesheet">

  <link rel="preconnect" href="https://fonts.googleapis.com">

  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:ital,wght@0,300..800;1,300..800&family=Sansita:ital,wght@0,400;0,700;0,800;0,900;1,400;1,700;1,800;1,900&display=swap" rel="stylesheet">

  <link rel="preconnect" href="https://fonts.googleapis.com">

  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

  <link href="https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,300;0,400;0,500;0,700;1,300;1,400;1,500;1,700&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="style.css">

  <meta charset="UTF-8">

  <meta name="viewport" content="width=device-width, initial-scale=1.0">

  <title>MyPersonalPage</title>

</head>

<body>

    <header>

      <div class="container">  

        <div class="nav_items">

            <a class="item" href="#">ГЛАВНАЯ</a>

            <a class="item" href="#achive">ДОСТИЖЕНИЯ</a>

            <a class="item" href="#about">ОБО МНЕ</a>

        </div>

      </div>

    </header>

  

    <div class="content">

  

      <div class="main_line">

  

        <div class="main_block">

          <h1>Всем привет!  <br> Меня зовут Кирилл &#128075;</h1>

          <p>

            Это мой первый сайт. И, по совместительству, первая лабораторная работа по вебам... <br>

            Не судите строго :)<p style="font-size: x-small;">Ps. И да, сайт ни капли не Адаптивный&#9996;</p>

          </p>

        </div>

  

        <div class="photo">

          <img src="/assets/photo.jpg" alt="">

        </div>

      </div>

      <a id="about" class="anchor"></a>

      <div class="section">

        <div class="paragraph_header">

          <h2>Обо мне</h2>

        </div>

  

        <div class="paragraph_text">

          <p>

            На данный момент я являюсь студентом Сахалинского Государственного Университета.

            Обучаюсь на 2-м курсе направления "Прикладная математика и информатика (Системное программирование и администрирование)".

            Увлекаюсь всем подряд (люблю пробовать новое). Сейчас начал изучать Web-разработку (Frontend в частности). Разбираюсь с HTML и CSS.

            Впереди цель - обуздать JavaScript.

          </p>

        </div>

      </div>

  

      <a id="achive" class="anchor"></a>

      <div class="section">

        <div class="paragraph_header">

          <h2>Мои достижения</h2>

        </div>

  

        <div class="paragraph_text">

          <p>

            Из достижений могу отметить две статьи по искусственному интеллекту на темы:

            "Исследование влияния формата представления обучающей выборки на точность классификаторов, построенных методами машинного обучения"

            и

            "Введение в принципы декомпозиции обучающей выборки на обучающее и тестовое множество в задачах машинного обучения".

            За них получил два диплома первой степени.

          </p>

          <div class="dips">

            <div class="dip">

              <img src="assets/dip1.png" alt="">

            </div>

            <div class="dip">

              <img src="assets/dip2.png" alt="">

            </div>

          </div>

        </div>

      </div>

    </div>

  

    <footer>

      <div class="contacts">

        <p><a>Telegram</a></p> <p><a>GitHub</a></p> <p><a>Discord</a></p>

      </div>

    </footer>

</body>

</html>
```


<h2 align="center">Файл style.css</h2>

```
body {

    margin: 0;

    background-color: #07142b;

    background-repeat: no-repeat;

}

  

header {

    font-family: "Open Sans";

    font-size: 16px;

    background-color: #173c4c;

    padding: 20px;

    font-weight: 700;

    position: fixed;

    top: 0;

    width: 100%;

}

  

.nav_items {

    text-align: center;

}

  

.nav_items a {

    color: #ffffff;

    text-decoration: none;

    padding: 20px 40px 20px 40px;

    margin: -2px;

    transition: background-color 400ms linear;

}

  

.nav_items a:hover {

    background-color: #07142b;

}

  

.content {

    font-weight: 500;

    display: block;

    margin-top: 130px;

    font-family: ubuntu;

}

  

.content .photo img {

    border-radius: 300px;

    margin-right: 300px;

    width: 450px;

    height: 450px;

}

  

.main_line {

    display: flex;

    align-items: center;

}

  

.main_block p {

    color: #ffffff;

    font-weight: lighter;

    text-align: inherit;

    font-size: 40px;

    line-height: 60px;

    margin: 0;

    padding: 0;

}

  

.main_block {

    background-color: #326d6c;

    background-size: 100% 50%;

    margin-right: 100px;

    border-top-right-radius: 150px;

    border-bottom-right-radius: 10px;

    font-size: 30px;

    font-family: ubuntu;

    padding: 25px 25px 25px 40px;

}

  

.main_block h1 {

    text-align: left;

    color: #ffffff;

    font-size: 60px;

    font-weight: 200;

    padding: 0;

    margin: 0;

    margin-top: 5px;

}

  

.section {

    margin-top: 74px;

    padding: 0;

}

  

.section h2 {

    color: #173c4c;

    font-size: 55px;

    text-align: center;

    margin: 0;

    padding: 0;

}

  

.paragraph_header {

    background-color: #ffffff;

}

  

.paragraph_text {

    color: white;

    text-align: justify;

    text-indent: 80px;

    font-size: 30px;

    margin: 0 10% 0 10%;

    padding-top: 25px;

    line-height: 60px;

}

  

.dip img {

    width: 700px;

    height: 500px;

    margin-left: -55px;

}

  

.dips {

    display: flex;

}

  

.anchor {

    display: flex;

    width: 1px;

    height: 1px;

}

  

footer {

    background-color: #173c4c;

    margin-top: 60px;

    justify-content: center;

    display: flex;

}

  

footer p {

    font-size: 20px;

    padding-right: 25px;

    padding-left: 25px;

    line-height: 5px;

    font-family: ubuntu;

    font-weight: 100;

}

  

.contacts {

    display: flex;

}

  

.contacts a {

    color: #ffffff;

    text-decoration: none;

    transition: color 250ms linear;

    border-right: 1px solid;

    border-left: 1px solid;

    border-color: #07142b;

    padding-right: 10px;

    padding-left: 10px;

}

  

.contacts a:hover {

    color: #07142b;

    cursor: pointer;

}
```
<h1 align = "center">Результат</h1>


<h1 align = "center">Вывод</h1>
<p align="justify">По итогу проделанной лабораторной работы, я больше узнал о селекторах, свойствах и параметрах CSS, научился реализовывать "задуманное" на "чистом листе", сделал свой первый web-сайт.</p>
