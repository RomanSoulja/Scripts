# Python's Scripts

### Поиск x в f(x):
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

### Калькулятор:
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
