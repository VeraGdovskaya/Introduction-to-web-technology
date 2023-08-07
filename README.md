# Introduction-to-web-technology (seminar4)

<!-- Задача №1: сформировать массив с данными для блока «Опыт работы».
Вывести данные массива в HTML-шаблоне.
Задача №2: создать БД, состоящую из одной таблицы (информация об одногруппниках) с четырьмя полями (добавить поле «Адрес»): id, name, age, address -->

1 <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <?php
    <?php
    $job = [
    'job_name' => ['Easy English', 'Зебра', 'Цветочный Мир'],
    'job_data' => ['2015-настоящее время', '2012-2015', '2010-2012'],
    'job_desc' => ['Учитель английского', 'Фитнес тренер', 'Флорист']
    ]
    ?>
    
    <h1>Опыт работы:</h1>
    <?php echo $job['job_name'][0]; ?>
    <?php echo " :  "; ?>
    <?php echo $job['job_data'][0]; ?>
    <?php echo ", "; ?>
    <?php echo $job['job_desc'][0]; ?>
    <h2>  </h2>
    <?php echo $job['job_name'][1]; ?>
    <?php echo " :  "; ?>
    <?php echo $job['job_data'][1]; ?>
    <?php echo ", "; ?>
    <?php echo $job['job_desc'][1]; ?>
    <h3>  </h3>
    <?php echo $job['job_name'][2]; ?>
    <?php echo " :  "; ?>
    <?php echo $job['job_data'][2]; ?>
    <?php echo ", "; ?>
    <?php echo $job['job_desc'][2]; ?>
    
</body>
</html>

--create
create table GROUP_MATE  (
    student_ID INTEGER PRIMARY KEY,
    name TEXT NOT NULL,
    age TEXT NOT NULL,
    address TEXT NOT NULL
);
--insert
INSERT INTO GROUP_MATE VALUES(0001, 'Татьяна Иванова', 21, 'Воронеж');
INSERT INTO GROUP_MATE VALUES(0002, 'Сергей Петров', 25, 'Кемерово');
INSERT INTO GROUP_MATE VALUES(0003, 'Еленеа Смит', 21, 'Москва');
INSERT INTO GROUP_MATE VALUES(0004, 'Иван Иванов', 22, 'Сочи');
INSERT INTO GROUP_MATE VALUES(0005, 'Роман Петров', 23, 'Санкт-Петербург');
