# Task0
import random
random_list = [random.randrange(-100,100) for i in range(30)]
print("\nСлучайный список чисел от -100 до 100: ", random_list)
max_element = max(random_list)
position = random_list.index(max_element)
print("\nМаксимальное значение из списка: ", max_element, "\nна позиции: ", position + 1)
new_list=[]
for element in random_list:
    if (element % 2) == 1:
        new_list.append(element)
if len(new_list) == 0:
  print("\nнет ни одного нечетного числа")
else:
  new_list.sort(reverse=True)
  print("\nНовый список: ", new_list)