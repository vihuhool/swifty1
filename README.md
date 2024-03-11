```
// Массив с количеством дней в месяцах
let daysInMonths = [31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31]

// Массив с названиями месяцев
let monthNames = ["Январь", "Февраль", "Март", "Апрель", "Май", "Июнь", "Июль", "Август", "Сентябрь", "Октябрь", "Ноябрь", "Декабрь"]

// Используя цикл for, выведем количество дней в каждом месяце (без имен месяцев)
for days in daysInMonths {
    print(days)
}

// Используем массив с именами месяцев, чтобы вывести название месяца + количество дней
for (index, days) in daysInMonths.enumerated() {
    print("\(monthNames[index]): \(days)")
}

// Создадим массив кортежей (имя месяца, количество дней)
let monthDaysTupleArray = zip(monthNames, daysInMonths)

// Выведем кортежи
for tuple in monthDaysTupleArray {
    print("\(tuple.0): \(tuple.1)")
}

// Выведем количество дней в обратном порядке, не изменяя порядок в массиве
for days in daysInMonths.reversed() {
    print(days)
}

// Произвольная выбранная дата (месяц и день)
let chosenMonth = 3 // Март
let chosenDay = 11

// Посчитаем количество дней до этой даты от начала года
var totalDays = 0
for i in 0..<chosenMonth - 1 {
    totalDays += daysInMonths[i]
}
totalDays += chosenDay
print("Количество дней до \(chosenDay) марта от начала года: \(totalDays)")

```

![изображение](https://github.com/vihuhool/swifty1/assets/69204363/96c05e61-2391-4286-9ff1-40ab9f78f247)
![изображение](https://github.com/vihuhool/swifty1/assets/69204363/17fde561-80cd-4993-83e0-1f7ad6632783)

