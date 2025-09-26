# Матвей Тимофеев ✨  

## Обо мне  
Студент 1 курса ИРИТ-РТФ по направлению «Прикладная информатика» (09.03.03). 🎓  
Увлекаюсь компьютерными играми, разработкой собственных проектов и TG-ботов.  
Интересуюсь машинным обучением и компьютерным зрением. 🤖  

## Мои интересы  
- Компьютерные игры 🎮  
- Программирование (собственные проекты, GitHub) 💻  
- TG-боты 🤖  
- Машинное обучение и машинное зрение 🔬  

## Мои навыки  
1. **Python** 🐍  
   - TG user-bot на **Pyrogram**  
   - Боты на **Telebot**  
   - Парсеры **HTML-таблиц**  

2. **C++**  
   - Программирование микроконтроллеров  

3. **C#**  
   - Запуск кастомной LM с применением «вайб-кодинга»  

4. **JavaScript**  
   - Первый язык, базовые знания  

5. **Lua** 🦎  
   - Опыт написания скриптов и небольших программ  
   - Использовался для автоматизации и игр  

## Расписание на неделю  

| Дата       | День недели | Занятие                                   | Время         |
|------------|-------------|-------------------------------------------|---------------|
| 29.09.2025 | Понедельник | Архитектура вычислительных систем        | 14:15–15:45   |
|            |             | Разработка WEB-приложений                | 16:00–17:30   |
| 30.09.2025 | Вторник     | Физ-ра                                   | 12:00–13:30   |
|            |             | АГиТДУ                                   | 14:15–15:45   |
|            |             | Программирование (повышенный уровень)    | 17:40–19:10   |
|            |             | Программирование (повышенный уровень)    | 19:15–20:45   |
| 01.10.2025 | Среда       | Математика (повышенный уровень)          | 8:30–10:00    |
|            |             | ОРГ                                      | 10:15–11:45   |
|            |             | Архитектура вычислительных систем        | 19:15–20:45   |
| 02.10.2025 | Четверг     | АГиТДУ                                   | 8:30–10:00    |
|            |             | Физ-ра                                   | 12:00–13:30   |
|            |             | Математика (повышенный уровень)          | 14:15–15:45   |
|            |             | Математика (повышенный уровень)          | 16:00–17:30   |
| 03.10.2025 | Пятница     | Информационные технологии и сервисы      | 10:15–11:45   |
|            |             | Английский язык B1                       | 12:00–13:30   |

## Дополнительно  
- 📎 https://github.com/TrollFace324  
- Я  
  ![Markdown Logo](https://cdn.discordapp.com/attachments/1041075762142384312/1421017210259902474/image.png?ex=68d780e8&is=68d62f68&hm=f4d43b202b553c3653b07e0590bbca551f0f4e8dd56938f03691eb292c97b8da&)  
- Пример кода из https://github.com/TrollFace324/User_bot_for_tg:  

```python
# Start message
@bot.on_message()
async def echo_handler(client: Client, message: Message):
    defualt_user = Defualt_user(message)
    admin = Admin(message)
    eris_tg_bot = Eris_tg_bot(message)
    eris_me = Eris_me(message)

    if message.text and message.chat.id == CHAT_ERIS_BOT:
        if message.from_user.id == ME:
            await eris_me.requestMoreTime()
            await eris_me.getAllTime()
            await eris_me.clearAllTime()
            await eris_me.addTime()
            await eris_me.helpEris()

        if message.from_user.id == CHAT_ERIS_BOT:
            eris_tg_bot.setTimeIn()
            await eris_tg_bot.setTimeOut()
            await eris_tg_bot.autoTimeOut()
            await eris_tg_bot.deleteUselessMessage()
    
    if message.text and message.from_user and message.from_user.id == ME:
        await admin.useEval()
        await admin.useEvalMe()
        await admin.getErrInEval()
        await admin.helpAdmin()
    
    defualt_user.setDarkMode()
    await defualt_user.requestToGPT()
    await defualt_user.getPolaroid()
    await defualt_user.helpUser()

    if message.reply_to_message:
        await defualt_user.try_write_poll()
        await defualt_user.try_remove_poll()
        await defualt_user.get_visual_poll_data()
