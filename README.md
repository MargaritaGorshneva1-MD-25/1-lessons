# 1-lessons-1
print("Как вас зовут?")
user_name_str = input()
print("Ваше имя,", user_name_str, "?")
user_otvet_str = input()
if user_otvet_str == "Да" or "Yes":
    print("Приятно познакомиться!:)")
else:
    print("Хм...зачем тогда вы написали это имя?")

№ 1-lessons-2
print("Сколько вам лет?")
user_name_str = input()
print("Вам", user_name_str, "?")
user_otvet_str = input()
if user_otvet_str == "Да" or "Yes":
    print("Прекрасно.")
else:
    print("Хм...зачем тогда вы написали не свой возраст?")

# 1-lessons-3
print("Как вас зовут?")
user_name_str = input()
print(user_name_str*4+user_name_str)

# 1-lessons-4
print("Как вас зовут?")
user_name_str = input()
print("Сколько вам лет?")
age = int(input())
print("Привет,", user_name_str , "!")
if age<=14:
    print("Говорят, что если девушке меньше 16, то она прекрасна. Но только если ей реально меньше 16, а не под 25")
else:
    print("Моей бабушке 50, но у неё тело болит меньше, чем у тебя.")
    
# 1-lessons-5

# 1-lessons-6

# 1-lessons-7

# 1-lessons-8

# 1-lessons-9

# 1-lessons-10
print("Какой будет ответ у задачи:3+(8*32/2)?")
otvet = int(input())
if otvet == 131:
    print("Правильно")
else:
    print("Неправильно. Подумай ещё своей головушкой.")
