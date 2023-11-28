# Отчет по лабораторной работе №7 <br>студента АСБ-3-037 Михеенко М. М.

---
### Задание 1:
Здесь надо заменить *var* на *let*, ну и строчки красиво оформить
```
let FirstPrompt = prompt('var one'),
    SecondPrompt = prompt('var two');
    
if (FirstPrompt === SecondPrompt) {
    console.log('equally');
}
else {
    console.log('no equally');
}

let World = 'world';
FirstPrompt = FirstPrompt + World;
```

### Задание 2:
Проще просто написать новую программу =)
```
let ColourFruits = {
    'apple': 'green',
    'strawberry': 'red',
    'blueberry': 'blue',
    'raspberry': 'light red',
    'lemon': 'yellow'
} 

fruit = Object.keys(ColourFruits)
colour = Object.values(ColourFruits)

for (let key in fruit) {
    console.log(fruit[key]);
}
    
for (let key in fruit) {
    console.log(fruit[key] + ' ' + colour[key]);
}
```

### Задание 3:
Расставил пробелы, табуляции. Оставил пустые строки между разными блоками кода, чтоб читалось проще и понятнее
```
let CountPeople = prompt ('Введите кол-во человек ', undefined);

if (!isNaN(parseFloat(CountPeople))) {
    CountPeople = parseFloat(CountPeople);
}
else {
    CountPeople = 0;
}

while(CountPeople === 0) {
    let CountPeople = prompt ('Введите кол-во человек ', undefined);
    if (!isNaN(parseFloat(CountPeople))) {
        CountPeople = parseFloat(CountPeople);
    }
    else {
        CountPeople = 0;
    }
}

let salary = prompt ('Введите зарплату на человека ', undefined);

if (!isNaN(parseFloat(salary))) {
    salary=parseFloat(salary);
}
else {
    salary = 0;
}

while (CountPeople === 0) {
    let salary = prompt('Введите зарплату на человека ', undefined);
    if (!isNaN(parseFloat(salary))) {
        salary = parseFloat(salary)
    } else {
        salary = 0;
    }
}

alert('Затраты на ЗП: ' + CountPeople * salary);
```

### Задание 4:
Опять заменил *var*-ы на *let*-ы. Написал нормальные названия переменных на английском языке, а не чушь транслитом
```
let ClassStudent = [
    {FIO: 'Петров А.А.', Rating: 5 },
    {FIO: 'Иванов Б.Б.', Rating: 3.4 },
    {FIO: 'Сидоров Г.Г.', Rating: 9 },
    {FIO: 'Немолодой Д.Д', Rating: 2 },
    {FIO: 'Молодой Е.Е', Rating: 3.4 }
];

let MeanRating = 0,
    count = 0,
    BadStudent = [];

for (let indexStudent = 0; indexStudent < ClassStudent.length; indexStudent++) {

    if (ClassStudent[indexStudent].Rating > 5) {
        console.log('Это значение учитываться не будет оно не соответствует допустимым значениям');
    }

    if (ClassStudent[indexStudent].Rating < 0) {
        console.log('Это значение учитываться не будет оно не соответствует допустимым значениям');
    }

    if (! (ClassStudent[indexStudent].Rating <= 5 && ClassStudent[indexStudent].Rating >= 0 )) {
        continue;
    }

    if (ClassStudent[indexStudent].Rating < 4) {
        BadStudent.push(ClassStudent[indexStudent]);
    }

    MeanRating += ClassStudent[indexStudent].Rating;
    count += 1;
}

MeanRating = MeanRating / count;
console.log('Средняя оценка: ' + MeanRating);
console.log('Плохие студенты: ');

if (BadStudent.length === 0) {
    console.log('Таких нет');
}

BadStudent.forEach((index) => { console.log('Фио: ' + index.FIO + '; Оценка: ' + index.Rating) });
```

### Задание 5:
Да там и так всё в порядке))))))
![Да серьёзно. А ты че, не верил?))))](imgs/serious.jpg)