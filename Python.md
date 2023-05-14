# Python's Scripts

Обозначения типов данных:
* int - целое число (42);
* float - число с запятой (1.15);
* str - строка ("тут могла быть Ваша реклама");
* bool - булевый тип данных (true или false);
* list - список;
* tuple - кортеж;
* set - множество.

> Все программы являются консольными

## Поиск x в f(x):
```
funct = input('Введите функцию с переменной x: ')

x = input('Введите x: ')

while x.isdigit() or (x.startswith('-') and x[1:].isdigit):
	x = int(x)
	print(f'Ответ: {eval(funct)}')
	x = input('Введите x: ')
	print('Если хотите прекратить впишите любую строку.')

print('Программа завершилась.')
```


## Калькулятор:
```
import math, random


settin = '''Можно использовать математические операции,
рандом и т.д.'''

print(settin)
example = input('Введите пример: ')

while example != 0:
	print(f'Ответ: {eval(example)}')
	print('Если хотите прекратить впишите 0')
	example = input('Введите пример: ')

print('Программа завершилась.')
```


## Поиск координат(x;y) по функции:
```
print('Впишите функцию с переменной x')
print('y =', end=' ')
func = input()
listik = []
cycle = 0


while func != 'Конец':
    cycle += 1

    xStart = int(input('Впишите первую границу: '))
    xEnd = int(input('Впишите вторую границу: '))

    for x in range(xStart, xEnd+1):
        listik.append(f'({x};{eval(func)})')

    print(*listik)
    
    print(f'''
Впишите функцию с переменной x
{cycle} цикл
Или впишите "Конец"''')
    print('y =', end=' ')
    func = input()
```
