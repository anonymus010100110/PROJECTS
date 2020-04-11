# PROJECTS
def vvod1():
    b = int(input("Введите число:"))
    return b


def basic1(num, b, a):
    while num <= 3:
        if b < a  and b >= 1:
            print("Больше...")
        elif b <= 10 and b > a :
            print("Меньше...")
        elif b == a:
            print("Отгадали!")
            exit(1)
        else:
            print("Неверный ввод(нужно: от 1 до 10)")
        b = vvod1()
        num += 1


import random
print("Игра 'Угадай число'")
print("Вводите свои предположения")

a = random.randint(0, 10)
num = 1

print("Попытка номер:", num)

b = vvod1()
basic1(num, b, a)

print("Ваши попытки закончились!")
print("Это было число:", a)
input("\n\nНажмите Enter,чтобы выйти\n\n")
