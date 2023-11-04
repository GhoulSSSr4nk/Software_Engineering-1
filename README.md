# Тема 5. Базовые коллекции: множества, списки
Отчет по Теме #5 выполнил(а):
- Глушков Михамл Сергеевич
- ПИЭ-21-1

| Задание | Лаб_раб | Сам_раб |
| ------ | ------ | ------ |
| Задание 1 | + | + |
| Задание 2 | + | + |
| Задание 3 | + | + |
| Задание 4 | + | + |
| Задание 5 | + | + |
| Задание 6 | + | |
| Задание 7 | + | |
| Задание 8 | + |  |
| Задание 9 | + |  |
| Задание 10 | + |  |

# Лабараторные работы 
   ## Лабараторная работа 1
Друзья предложили вам поиграть в игру “найди отличия и убери повторения (версия для программистов)”. Суть игры состоит в том, что на вход программы поступает два множества, а ваша задача вывести все элементы первого, которых нет во втором. А вы как раз недавно прошли множества и знаете их возможности, поэтому это не составит для вас труда.

  ```python
set_1={'White','Black','Red','Pink'}
set_2={'Red','Green','Blue','Red'}
print(set_1 - set_2 )
```
  ### Результат
  ![1](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%201.png)

 
## Краткий вывод:
Исходные множества:

set_1: {'White', 'Black', 'Red', 'Pink'}
set_2: {'Red', 'Green', 'Blue', 'Red'}
Результат операции set_1 - set_2:

В set_1 есть 'White', 'Black', 'Pink'
'Red' есть в обоих множествах, поэтому он не включается в результат.
Таким образом, на экран будет выведено множество {'White', 'Black', 'Pink'}.


   ## Лабараторная работа 2
Напишите две одинаковые программы, только одна будет использовать set(), а вторая frozenset() и попробуйте к исходному множеству добавить несколько элементов, например, через цикл. 

  ```python
a = set('abcdefg')
print(a)
for i in range(1, 5):
    a.add(1)
print(a)

```
  ### Результат
  ![2](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%202.png)

 
## Краткий вывод:
В этом коде создается множество a, содержащее элементы 'a', 'b', 'c', 'd', 'e', 'f', 'g'. Затем в цикле добавляется элемент '1' в это множество несколько раз.


   ## Лабараторная работа 3
На вход в программу поступает список (минимальной длиной 2 символа). Напишите программу, которая будет менять первый и последний элемент списка

  ```python
def replace(input_list):
    memory = input_list[0]
    input_list[0]=input_list[-1]
    
    return input_list 

print(replace([1,2,3,4,5]))
```
  ### Результат
  ![3](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%203.png)

 
## Краткий вывод:
Этот код определяет функцию replace, которая принимает на вход список (input_list). Внутри функции первый элемент списка (input_list[0]) сохраняется в переменной memory. Затем первый элемент списка заменяется последним (input_list[0] = input_list[-1]). Функция возвращает измененный список.


   ## Лабараторная работа 4
На вход в программу поступает список (минимальной длиной 10 символов). Напишите программу, которая выводит элементы с индексами от 2 до 6. В программе необходимо использовать “срез”

  ```python
a =[12,54,32,843,2346,765,75,25,234,756,23]
print(a[2:6])

```
  ### Результат
  ![5](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%204.png)

 
## Краткий вывод:
В данном коде создается список a, и затем выводится подсписок этого списка, начиная с элемента с индексом 2 и заканчивая элементом с индексом 5 (не включая элемент с индексом 6).


   ## Лабараторная работа 5
Иван задумался о поиске «бесполезного» числа, полученного из списка. Суть поиска в следующем: он берет произвольный список чисел, находит самое большое из них, а затем делит его на длину списка. Студент пока не придумал, где может пригодиться подобное значение, но ищет у вас помощи в реализации такой функции useless()

  ```python
ef useless(lst):
    return max(lst) / len(lst)
print(useless([3,5,7,3,33]))
print(useless([-12.5,54,77.3,0,-36,98.2,-63,21.7,47,-89.6]))
print(useless([-25.8,86,12.5,-56,73.2,0,43,-91.5,65.9,-7]))
```
  ### Результат
  ![5](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%205.png)

 
## Краткий вывод:

Этот код определяет функцию useless, которая принимает на вход список (lst). Функция возвращает результат деления максимального значения в списке на его длину.

   ## Лабараторная работа 6
 Ребята не могут определится каким супергероем они хотят стать. У них есть случайно составленный список супергероев, и вы должны определить кто из ребят будет каким супергероем. Необходимо использовать разделение списков

  ```python
superheroes =['superman','spiderman','batman']
nikolay,vasiliy,ivan = superheroes

print('Николай -', nikolay)
print('Василий -', vasiliy)
print('Иван -', ivan)
```
  ### Результат
  ![6](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%206.png)

 
## Краткий вывод:
В данном коде создается список superheroes с тремя строковыми элементами. Затем эти элементы распаковываются в три переменные: nikolay, vasiliy, и ivan. И, наконец, значения этих переменных выводятся на экран.

   ## Лабараторная работа 7
Вовочка, насмотревшись передачи “Слабое звено” решил написать программу, которая также будет находить самое слабое звено (минимальный элемент) и удалять его, только делать он это хочет не с людьми, а со списком. Помогите Вовочке с реализацией программы. Подсказка: для этого вам необходимо отсортировать список и удалить значение при помощи pop()

  ```python
a =[-25.8,86,12.5,-56,73.2,0,43,-91.5,65.9,-7]
a.sort()
print("Отсортированный список:\n",a)
a.pop(0)
print("Отсортированный список без наименьшого элемента:
```
 
# Результат
  ![7](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%207.png)

 
## Краткий вывод:
a = [-25.8, 86, 12.5, -56, 73.2, 0, 43, -91.5, 65.9, -7]: Создается список a с десятью числовыми элементами.

a.sort(): Список a сортируется в порядке возрастания. После этой операции a будет [ -91.5, -56, -25.8, -7, 0, 12.5, 43, 65.9, 73.2, 86].

print("Отсортированный список:\n", a): Выводится отсортированный список.

a.pop(0): Удаляется первый элемент списка. Теперь a будет [ -56, -25.8, -7, 0, 12.5, 43, 65.9, 73.2, 86].

print("Отсортированный список без наименьшего элемента: \n", a): Выводится отсортированный список без удаленного элемента.


   ## Лабараторная работа 8
Михаил решил создать большой n-мерный список, для этого он случайным образом создал несколько списков, состоящих минимум из 3, а максимум из 10 элементов и поместил их в один большой список. Он также как и Иван не знает зачем ему это сейчас нужно, но надеется на то, что это пригодится ему в будущем.

  ```python
from random import  randint

def list_maker():
    a =[randint(1,100)]*randint(3,10)
    return a
if __name__ =='__main__':
    result = []
    for i in range(randint(1,5)):
        result.append(list_maker())

    print(result)

```
  ### Результат
  ![8](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%208.png)

 
## Краткий вывод:
В этом коде определена функция list_maker(), которая создает список случайной длины от 3 до 10 элементов, где каждый элемент - случайное число от 1 до 100. Затем в основной части программы создается список result, в который добавляются результаты вызова функции list_maker() несколько раз (от 1 до 5 раз).


   ## Лабараторная работа 9
Вы работаете в ресторане и отвечает за статистику покупок, ваша задача сравнить между собой заказы покупателей, которые указаны в разном порядке. Реализуйте функцию superset(), которая принимает 2 множества. Результат работы функции: вывод в консоль одного из сообщений в зависимости от ситуации: 1 - «Супермножество не обнаружено»
2 – «Объект {X} является чистым супермножеством» 
3 – «Множества равны

  ```python
def superset(set_1,set_2):
    if set_1 > set_2:
        print(f'Объект {set_1} вляется чистым супермножством')
    elif set_1==set_2:
        print(f"Множества равны")
    elif set_1<set_2:
        print(f'Объект {set_2} является чистым супермножеством')
    else:
        print("Супермножество не обнаружено")

if __name__ == '__main__':
    superset({1,8,3,5},{3,5})
    superset({1, 8, 3, 5}, {5, 3,8,1})
    superset({3,5}, {5,3,8,1})
    superset({90,100}, {3, 5})
```
  ### Результат
  ![9](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%209.png)

 
## Краткий вывод:
def superset(set_1, set_2):: Определяется функция superset, которая сравнивает два множества и выводит информацию о том, является ли одно из них супермножеством другого.

if set_1 > set_2:: Если set_1 является супермножеством set_2 (все элементы set_2 также присутствуют в set_1), то выводится сообщение о том, что set_1 является чистым супермножеством.

elif set_1 == set_2:: Если множества равны, выводится сообщение об этом.

elif set_1 < set_2:: Если set_2 является супермножеством set_1, выводится сообщение о том, что set_2 является чистым супермножеством.

else:: Если ни одно из вышеперечисленного не выполняется, выводится сообщение о том, что супермножество не обнаружено.

if __name__ == '__main__':: Проверяется, запущен ли скрипт напрямую (а не импортирован как модуль).

Вызывается функция superset несколько раз с разными множествами.


   ## Лабараторная работа 10
Предположим, что вам нужно разобрать стопку бумаг, но нужно начать работу с нижней, “переверните стопку”. Вам дан произвольный список. Представьте его в обратном порядке. Программа должна занимать не более двух строк в редакторе кода.

  ```python
my_list=[2,5,8,3]
print(my_list[::-1])
```
  ### Результат
  ![10](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Lab%2010.png)

 
## Краткий вывод:
my_list = [2, 5, 8, 3]: Создается список my_list с элементами 2, 5, 8, 3.

my_list[::-1]: Используется срез для создания нового списка, который является обратным порядком элементов из списка my_list. [::-1] означает "взять все элементы с шагом -1", что приводит к обратному порядку.

print(my_list[::-1]): Выводится новый список, который является обратным порядком исходного списка.

# Самостоятельные работы
   ## Самотоятельная работа 1
Ресторан на предприятии ведет учет посещений за неделю при помощи кода работника. У них есть список со всеми посещениями за неделю. Ваша задача почитать: • Сколько было выдано чеков • Сколько разных людей посетило ресторан • Какой работник посетил ресторан больше всех раз Список выданных чеков за неделю: [8734, 2345, 8201, 6621, 9999, 1234, 5678, 8201, 8888, 4321, 3365, 1478, 9865, 5555, 7777, 9998,1111, 2222, 3333, 4444, 5556, 6666, 5410, 7778, 8889, 4445, 1439, 9604, 8201, 3365, 7502, 3016, 4928, 5837, 8201, 2643, 5017, 9682, 8530, 3250, 7193, 9051, 4506, 1987, 3365, 5410, 7168, 7777, 9865, 5678, 8201, 4445, 3016, 4506, 4506] Результатом выполнения задачи будет: листинг кода, и вывод в консоль, в котором будет указана вся необходимая информация.

  ```python
from collections import Counter

# Список выданных чеков за неделю
checks = [8734, 2345, 8201, 6621, 9999, 1234, 5678, 8201, 8888, 4321, 3365, 1478, 9865, 5555, 7777, 9998,
          1111, 2222, 3333, 4444, 5556, 6666, 5410, 7778, 8889, 4445, 1439, 9604, 8201, 3365, 7502, 3016,
          4928, 5837, 8201, 2643, 5017, 9682, 8530, 3250, 7193, 9051, 4506, 1987, 3365, 5410, 7168, 7777,
          9865, 5678, 8201, 4445, 3016, 4506, 4506]

# Сколько было выдано чеков
num_checks = len(checks)

# Сколько разных людей посетило ресторан
num_unique_visitors = len(set(checks))

# Какой работник посетил ресторан больше всех раз
most_visited_employee = Counter(checks).most_common(1)[0][0]

# Вывод результатов
print("Сколько было выдано чеков:", num_checks)
print("Сколько разных людей посетило ресторан:", num_unique_visitors)
print("Какой работник посетил ресторан больше всех раз:", most_visited_employee)


```
  ### Результат
  ![11](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Sam%201.png)

 
## Краткий вывод:
Этот код использует модуль collections для создания объекта Counter, который помогает подсчитать количество посещений для каждого кода работника. Затем мы используем эти данные для вывода необходимой информации в консоль.

  ## Самотоятельная работа 2
На физкультуре студенты сдавали бег, у преподавателя физкультуры есть список всех результатов, ему нужно узнать • Три лучшие результата • Три худшие результата • Все результаты начиная с 10 Ваша задача помочь ему в этом. Список результатов бега: [10.2, 14.8, 19.3, 22.7, 12.5, 33.1, 38.9, 21.6, 26.4, 17.1, 30.2, 35.7, 16.9, 27.8, 24.5, 16.3, 18.7, 31.9, 12.9, 37.4] Результатом выполнения задачи будет: листинг кода, и вывод в консоль, в котором будет указана вся необходимая информация.

  ```python
# Список результатов бега
running_results = [10.2, 14.8, 19.3, 22.7, 12.5, 33.1, 38.9, 21.6, 26.4, 17.1, 30.2, 35.7, 16.9, 27.8, 24.5, 16.3, 18.7, 31.9, 12.9, 37.4]

# Три лучших результата
best_results = sorted(running_results)[:3]

# Три худших результата
worst_results = sorted(running_results)[-3:]

# Все результаты начиная с 10
results_from_10 = running_results[9:]

# Вывод результатов
print("Три лучших результата:", best_results)
print("Три худших результата:", worst_results)
print("Все результаты начиная с 10:", results_from_10)

```
  ### Результат
  ![12](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Sam%202.png)

 
## Краткий вывод:
Этот код использует функцию sorted() для сортировки списка результатов бега. Затем мы используем срезы для выбора три лучших и три худших результатов, а также всех результатов начиная с 10-го.

  ## Самотоятельная работа 3
Преподаватель по математике придумал странную задачку. У вас есть три списка с элементами, каждый элемент которых – длина стороны треугольника, ваша задача найти площади двух треугольников, составленные из максимальных и минимальных элементов полученных списков. Результатом выполнения задачи будет: листинг кода, и вывод в консоль, в котором будут указаны два этих значения. Три списка:
one = [12, 25, 3, 48, 71] two = [5, 18, 40, 62, 98] three = [4, 21, 37, 56, 84]

  ```python
import math

# Три списка с элементами
one = [12, 25, 3, 48, 71]
two = [5, 18, 40, 62, 98]
three = [4, 21, 37, 56, 84]

# Функция для вычисления площади треугольника по длинам его сторон
def calculate_triangle_area(a, b, c):
    s = (a + b + c) / 2
    return math.sqrt(s * (s - a) * (s - b) * (s - c))

# Находим минимальные и максимальные значения в каждом списке
min_one, max_one = min(one), max(one)
min_two, max_two = min(two), max(two)
min_three, max_three = min(three), max(three)

# Вычисляем площади треугольников
area_min = calculate_triangle_area(min_one, min_two, min_three)
area_max = calculate_triangle_area(max_one, max_two, max_three)

# Вывод результатов
print("Площадь треугольника, составленного из минимальных элементов:", area_min)
print("Площадь треугольника, составленного из максимальных элементов:", area_max)

```
  ### Результат
  ![13](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Sam%203.png)

 
## Краткий вывод:
Этот код использует формулу Герона для вычисления площади треугольника по длинам его сторон. Затем мы находим минимальные и максимальные значения в каждом из трех списков и вычисляем площади треугольников, составленных из минимальных и максимальных элементов.

  ## Самотоятельная работа 4
  Никто не любит получать плохие оценки, поэтому Борис решил это исправить. Допустим, что все оценки студента за семестр хранятся в одном списке. Ваша задача удалить из этого списка все двойки, а все тройки заменить на четверки. Списки оценок (проверить работу программы на всех трех вариантах): [2, 3, 4, 5, 3, 4, 5, 2, 2, 5, 3, 4, 3, 5, 4] [4, 2, 3, 5, 3, 5, 4, 2, 2, 5, 4, 3, 5, 3, 4] [5, 4, 3, 3, 4, 3, 3, 5, 5, 3, 3, 3, 3, 4, 4] Результатом выполнения задачи будет: листинг кода, и вывод в консоль, в котором будут три обновленных массива


  ```python
# Функция для обновления списка оценок
def update_grades(grades):
    updated_grades = []
    for grade in grades:
        if grade == 2:
            continue  # Пропускаем двойки
        elif grade == 3:
            updated_grades.append(4)  # Заменяем тройки на четверки
        else:
            updated_grades.append(grade)
    return updated_grades

# Три списка оценок
grades1 = [2, 3, 4, 5, 3, 4, 5, 2, 2, 5, 3, 4, 3, 5, 4]
grades2 = [4, 2, 3, 5, 3, 5, 4, 2, 2, 5, 4, 3, 5, 3, 4]
grades3 = [5, 4, 3, 3, 4, 3, 3, 5, 5, 3, 3, 3, 3, 4, 4]

# Обновляем списки оценок
updated_grades1 = update_grades(grades1)
updated_grades2 = update_grades(grades2)
updated_grades3 = update_grades(grades3)

# Вывод результатов
print("Обновленный список оценок 1:", updated_grades1)
print("Обновленный список оценок 2:", updated_grades2)
print("Обновленный список оценок 3:", updated_grades3)

```
  ### Результат
  ![14](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Sam%204.png)

 
## Краткий вывод:
Этот код создает функцию update_grades, которая проходится по каждой оценке в списке и удаляет двойки, а тройки заменяет на четверки. Затем функция вызывается для каждого из трех списков оценок.

  ## Самотоятельная работа 5
Вам предоставлены списки натуральных чисел, из них необходимо сформировать множества. При этом следует соблюдать это правило: если какое-либо число повторяется, то преобразовать его в строку по следующему образцу: например, если число 4 повторяется 3 раза, то в множестве будет следующая запись: само число 4, строка «44», строка «444». Множества для теста: list_1 = [1, 1, 3, 3, 1] list_2 = [5, 5, 5, 5, 5, 5, 5] list_3 = [2, 2, 1, 2, 2, 5, 6, 7, 1, 3, 2, 2] Результаты вывода (порядок может отличаться, поскольку мы работаем с set()): {'11', 1, 3, '33', '111'} {5, '5555', '555555', '55555', '555', '55', '5555555'}  {'11', 1, 3, 2, 5, 6, '222222', '222', 7, '2222', '22222', '22'}
  ```python
def process_list(input_list):
    result_set = set()
    for num in set(input_list):
        count = input_list.count(num)
        if count > 1:
            result_set.add(str(num) * count)
        else:
            result_set.add(num)
    return result_set

# Три списка натуральных чисел
list_1 = [1, 1, 3, 3, 1]
list_2 = [5, 5, 5, 5, 5, 5, 5]
list_3 = [2, 2, 1, 2, 2, 5, 6, 7, 1, 3, 2, 2]

# Обработка списков
result_1 = process_list(list_1)
result_2 = process_list(list_2)
result_3 = process_list(list_3)

# Вывод результатов
print(result_1)
print(result_2)
print(result_3)

```
  ### Результат
  ![15](https://github.com/GhoulSSSr4nk/Software_Eng/blob/Тема-5/pic/Sam%205.png)

 
## Краткий вывод:
Этот код создает функцию process_list, которая обрабатывает список натуральных чисел в соответствии с указанными правилами и возвращает соответствующее множество. Затем эта функция вызывается для каждого из трех списков.

# Общий вывод 
 решении задач по теме множества и операции с ними использовались различные аспекты работы с множествами, такие как операции над множествами, создание множеств, обход элементов множества, сортировка, использование условий и функций для обработки данных.


В некоторых задачах использовались стандартные модули Python, такие как math и collections, для выполнения математических и коллекционных операций.
Циклы и условия:

В коде присутствовали циклы для обработки элементов списка и условия для проверок и принятия решений.
Работа с множествами в Python предоставляет множество удобных инструментов для обработки данных. Операции над множествами, условия, циклы и использование функций помогают решать разнообразные задачи, начиная от простых операций с элементами до сложных математических вычислений.
