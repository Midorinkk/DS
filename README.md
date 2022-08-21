# Time-Series-Forecasting
Time series forecast for Sberbank virtual internship


## Задание

В файле `data.csv` представлены подневные данные объема расчетных счетов физических лиц. В отличие от депозита, клиент может снять всю сумму с расчетного счета 
в любой момент времени без каких-либо «штрафов». Такой продукт называют Undefined Maturity Product – UMP. 
Однако маловероятно, что все клиенты разом закроют свои счета в Банке. Всегда кто-то снимает деньги, а кто-то пополняет счет – есть некоторый стабильный уровень, 
ниже которого не опустится суммарный обьем расчетных счетов.

Для временного ряда в файле `data.csv` необходимо построить модель, которая оценивает обьем стабильной части средств на дату.

**Например**:

model_forecast

(2019-02-01, ‘1М’, История_до_2019-02-01) = стабильная часть на 1М

**Возможные горизонты**: 1М, 2М, 3М, 4М, 5М, 6М, 7М, 8М, 9М, 10М, 11М, 12М

**Критерии качества модели**:

Нужно одновременно минимизировать величины:

- максимальный объем пробития стабильный части на валидационной выборке
- фактическая стабильная часть – модельная стабильная часть



Всё необходимое для решения задачи и соответствующие комментарии находятся в файле `TS.ipynb`
