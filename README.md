def check_sign():
    chislo = float(input("Напишите число: "))
    if chislo > 0:
        print("Вы ввели положительное число")
    elif chislo < 0:
        print("Вы ввели отрицательное число")
    else:
        print("Вы ввели ноль")
        
        
def calculator():
    num1 = input("Введите первое число: ")
    num2 = input("Введите второе число: ")
    operation = input("Какое действие вам нужно? (+, -, *, /): ")

    try:
        num1 = float(num1)
        num2 = float(num2)

        if operation == "+":
            print("Результат:", num1 + num2)
        elif operation == "-":
            print("Результат:", num1 - num2)
        elif operation == "*":
            print("Результат:", num1 * num2)
        elif operation == "/":
            if operation != 0:
                print("Результат:", num1 / num2)
            else:
                print("На ноль делить нельзя")
        else:
            print("Неизвестная операция.")
    except ValueError:
        print("Ошибка: введите числа правильно!")
        

def main():
    while True:
        print("\nЧто вам нужно?")
        print("1. Определить знак числа")
        print("2. Калькулятор")
        print("3. Выйти")

        vibor = input("Введите номер действия (1/2/3): ").strip()

        if vibor == "1":
            check_sign()
        elif vibor == "2":
            calculator()
        elif vibor == "3":
            print("До новых встреч!")
            break
        else:
            print("Неверный выбор, попробуйте снова!")


main()
#   R e p o s i t o r y 
 
 