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
print("Сколько вам лет?")
age = int(input())
if 22 <= age < 25:
    print("14 лет: К 30 годам я объезжу всю Европу и примусь за Азию. 30 лет: Если сейчас реструктурировать кредит под 14%, то смогу взять гречу по акции")
if 40 > age >= 20:
    print("Раньше со словами Мне как обычно я заходил в бар. Теперь с такими словами я захожу в аптеку")
else:
    print("Повзрослел — это когда боишься стоматологов, не потому что больно, а потому что дорого.")

# 1-lessons-6
name = "Маргарита"
print (name[1], name[::-1], name[-3], name[:5], end="\n", sep="\n")

# 1-lessons-7
print("Как вас зовут?")
user_name_str = input()
print("Сколько вам лет?")
age = int(input())
summa = 0
proizv = 1
for i in range(2):
    summa=summa+int(str(age)[i])
    proizv=proizv*int(str(age)[i])
print(len(user_name_str), summa, proizv)

# 1-lessons-8
name = "Маргарита"
name = name.upper()
print(name.upper(), name.lower(), name.capitalize(), name[0].upper()+name.lower(), sep="\n", end="\n")

# 1-lessons-9
name = input('Введите имя: ')
age = int(input("Введите возраст: "))
name_letters = list(name)
not_space = True
for i in range(len(name_letters)):                  
    if name_letters[i] == ' ':
        not_space = False
        print("Рада познакомиться!")
else:
    print('Введенные данные не соответствуют условиям!')

# 1-lessons-10
print("Какой будет ответ у задачи:3+(8*32/2)?")
otvet = int(input())
if otvet == 131:
    print("Правильно")
else:
    print("Неправильно. Подумай ещё своей головушкой.")

#телеграм бот
import(telegram)
bot=telebot.Telebot(5317785622:AAEBeSL514cNnvSW-Q_JZ1YPMfpBHbdBzWk)
@bot.messege_handler(commands=["start"])
def start(message, res=False):
    chat_id= message.chat.id
    bot.send_message(chat.id, text="Привет, {0.first_name}! Я тестовый бот.".format(message.from_user))

@bot.message_handler(content_types=["text"])
def ger_text_messages(message):
    chat_id=message.chat.id
    ms_text=message.text
    bot.send_message(chat_id, text="Да слышу я тебя. Твоё сообщение:" + ms_text)

bot.polling(none_stop=True, interval=0)
