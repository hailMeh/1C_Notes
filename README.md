# 1C_Notes
//Найти среднее число
ЧислоА = 14;
ЧислоБ = 15;
ЧислоВ = 13;
Если (ЧислоА > ЧислоБ И ЧислоА < ЧислоВ) ИЛИ (ЧислоА < ЧислоБ И ЧислоА > ЧислоВ) Тогда 
	СреднееЧисло = ЧислоА;
ИначеЕсли (ЧислоБ > ЧислоА И ЧислоБ < ЧислоВ) ИЛИ (ЧислоБ < ЧислоА И ЧислоБ > ЧислоВ) Тогда 
	СреднееЧисло = ЧислоБ;
ИначеЕсли (ЧислоВ > ЧислоА И ЧислоВ < ЧислоБ) ИЛИ (ЧислоВ < ЧислоА И ЧислоВ > ЧислоБ) Тогда 
	СреднееЧисло = ЧислоВ;
КонецЕсли;
Сообщить(СреднееЧисло);

//Найти остаток от деления, если он есть
ЧислоА = 15;
ЧислоБ = 14;     
Если ЧислоА % ЧислоБ = 0 Тогда
	Сообщить("Делится без остатка")
ИначеЕсли ЧислоА % ЧислоБ <> 0 Тогда
	Остаток = ЧислоА % ЧислоБ;
	Сообщить("Делится с остатком");
	Сообщить(Остаток);
КонецЕсли;

//Пример на знание условий
Условие1 = Истина;
Условие2 = Ложь;
Условие3 = Ложь;
Условие4 = Истина;
Условие5 = Истина;
Условие6 = Истина;
Результат = (НЕ (Условие1 ИЛИ Условие2) И Условие3) ИЛИ Условие4 И Условие5 ИЛИ НЕ Условие6;
Сообщить(Результат);

//Задача на цикл и приведение типов числа к строке
Дюйм = 2.54;
Результат = 0;
Для Счетчик = 1 По 20 Цикл
	Результат = Результат + Дюйм;
	Сообщить(Строка(Счетчик) + " Дюйм = " + Строка(Результат) + " см");
КонецЦикла;
//Цикл по условию
СуммаЧисел = 0;
Счётчик = 1;
Пока СуммаЧисел <= 1235 Цикл
	СуммаЧисел = СуммаЧисел + Счётчик;
	Счётчик = Счётчик +1;
КонецЦикла;
Сообщить(СуммаЧисел);

//Цикл по счётчику
СуммаЧисел = 0;
Для Счётчик = 1 По 255 Цикл 
	СуммаЧисел = СуммаЧисел + Счётчик;
КонецЦикла;
Сообщить(СуммаЧисел);

//Цикл по коллекции
МассивЧисел = Новый Массив;
Для Счётчик = 1 По 100 Цикл
	МассивЧисел.Добавить(Счётчик);
	Сообщить(МассивЧисел.Количество())
КонецЦикла;
СуммаЧисел = 0;
Для каждого Число Из МассивЧисел Цикл
	СуммаЧисел = СуммаЧисел + Число;
КонецЦикла;
Сообщить(СуммаЧисел);

//Возведение в степень через цикл
ДвухзначноеЧисло = 15;
Степень = 4;
Результат = 1;
Для Счетчик = 1 По Степень Цикл
	Результат = Результат * ДвухзначноеЧисло;
Если Результат > 10000 Тогда
	Сообщить("Результат превышает допустимую норму в 10000, " + Результат);  
КонецЕсли;
КонецЦикла;
Сообщить(Результат);
	
//Умножение через цикл не пользуяюсь знаком умножения *
А = 19;
Б = 10;
Результат = 0;
Для Счетчик = 1 По Б Цикл
	Результат = Результат + А;
КонецЦикла;
Сообщить(Результат);
	
//Задача на цикл и приведение типов числа к строке
Дюйм = 2.54;
Результат = 0;
Для Счетчик = 1 По 20 Цикл
	Результат = Результат + Дюйм;
	Сообщить(Строка(Счетчик) + " Дюйм = " + Строка(Результат) + " см");
КонецЦикла;
