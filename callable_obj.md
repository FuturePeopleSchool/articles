## Как проверить, является ли объект вызываемым?

В Python существуют объекты, которые мы можем вызвать. 

Например, функция или класс. 

Когда мы хотим вызвать объект, то добавляем в конце имени круглые скобки.

```python
a = 10

class Car:
    pass

def hello():
    print('Hello!')

Car()
hello()
```

Если объект не вызываемый, то мы получим исключение *object is not callable*

```python
a = 10

class Car:
    pass

def hello():
    print('Hello!')

a()

print(callable(Car))
print(callable(hello))
print(callable(a))
```

Для проверки возможности вызова объекта существует функция callable. 

Если объект вызываемый - она вернет True.
Если нет false

```python
a = 10

class Car:
    pass

def hello():
    print('Hello!')

print(callable(Car()))
print(callable(hello()))
print(callable(a))
```
