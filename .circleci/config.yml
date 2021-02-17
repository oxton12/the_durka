# -*- coding: utf-8 -*-
import telebot

bot = telebot.TeleBot('1664022830:AAEOnq9AKeE1MpplF-D8ml1nUWGy__CoStI')
from telebot import types

@bot.message_handler(content_types=['text','sticker'])
def get_text_messages(message):
    if message.text.lower() == "привет" or message.text.lower() == "здорова" or message.text.lower() == "здравствуйте" or message.text.lower() == "хай" or message.text.lower() == "приветствую смотрящих" or message.text.lower() == "здравствуй карта":
        bot.send_message(message.from_user.id, "Привет, шизоид.")
        bot.send_sticker(message.from_user.id,'CAACAgIAAxkBAAEB469gLBIwvdgcjc948cH-TFLoNbOK0AACdRoAAowt_Qe4FPPkfFTeYR4E')

        keyboard = types.InlineKeyboardMarkup()
        # По очереди готовим текст и обработчик для каждого знака зодиака
        key_shiza = types.InlineKeyboardButton(text='шизофрения', callback_data='shiza')
        # И добавляем кнопку на экран
        keyboard.add(key_shiza)
        key_bipol = types.InlineKeyboardButton(text='биполярное расстройство', callback_data='bipol')
        keyboard.add(key_bipol)
        key_hearthstone = types.InlineKeyboardButton(text='слабоумие', callback_data='hearthstone')
        keyboard.add(key_hearthstone)
        key_okr = types.InlineKeyboardButton(text='обсессивно-компульсивное расстройство', callback_data='okr')
        keyboard.add(key_okr)
        key_hellblade = types.InlineKeyboardButton(text='психоз', callback_data='hellblade')
        keyboard.add(key_hellblade)
        bot.send_message(message.from_user.id, text='Что лечим сегодня?', reply_markup=keyboard)

    else:
        bot.send_message(message.from_user.id, "Ты как смирительную рубашку снял? Напиши \"Привет\", или позову санитаров.")
        bot.send_sticker(message.from_user.id,'CAACAgIAAxkBAAEB48NgLBKMopz3BouhnyuWSRlj2x0O3AACdhAAAowt_QfASpYK8SYhYh4E')

@bot.callback_query_handler(func=lambda call: True)
def callback_worker(call):
    if call.data == "shiza":
        bot.send_message(call.message.chat.id, "Относится к разряду психозов. Болезнь затрагивает несколько составляющих психики: мыслительную, эмоциональную, поведенческую и всю совокупность психических функций. Встречаются разные формы шизофрении (кататоническая, простая, параноидная). Соответственно, и симптомы могут разниться, тем не менее, самые частые это галлюцинации, негативизм, замкнутость, апатия.")
        bot.send_sticker(call.message.chat.id, 'CAACAgIAAxkBAAEB47tgLBJahAGEIEyx-eWRu0rCJTwKHQACcRAAAowt_Qe5lZYdJoni7B4E')

    if call.data == "bipol":
        bot.send_message(call.message.chat.id, "Болезнь также известна под названием маниакально-депрессивный психоз. Довольно распространенное заболевание с чередующимися депрессивными и маниакальными фазами. Этим заболеванием страдали некоторые известные актеры и певцы. Распознать болезнь можно по сначала повышенному настроению, усиленной двигательной и речевой активности больного, люди этого типа много говорят, шутят, смеются, берутся за множество дел... А потом так же резко \"сникают\". Не могут сосредоточиться. И в итоге много их начинаний ничем не заканчиваются.")
        bot.send_sticker(call.message.chat.id, 'CAACAgIAAxkBAAEB49FgLBO1GOOkE_Oh4nvq4k4Cl5RCGAAChRAAAowt_QeeCMkx3Vs8Gh4E')

    if call.data == "hearthstone":
        bot.send_message(call.message.chat.id, "Под этим термином подразумевается снижение интеллекта по разным причинам. Течение болезни обычно постепенное, и крайне редко – внезапное. Характеризуется усталостью, слабостью, снижением работоспособности, рассеянностью, нарушениями памяти. Наиболее частые заболевания этой группы – болезни Альцгеймера, Пика, Паркинсона, Вильсона. Лечение таких заболеваний мозга в настоящее время сталкивается с целым рядом осложнений. И в первую очередь не из-за того, что сложно лечить, а потому, что тяжело диагностировать.")
        bot.send_sticker(call.message.chat.id, 'CAACAgIAAxkBAAEB48xgLBKrljPEHFL1ik4AAfhDvH-ARi4AAoAQAAKMLf0HcTptx5rZ0DAeBA')

    if call.data == "okr":
        bot.send_message(call.message.chat.id, "Обсессивно-компульсивное расстройство, а проще говоря - нежелательные мысли и навязчивые действия. Такие люди часто бывают неуверены, заперли ли они двери, выключили свет, постоянно что-то проверяют, стучат по дереву, поддаются суевериям, боятся наступать на крышку канализационного люка. Часто встречаются преувеличенные страхи загрязниться от контакта с людьми или бытовыми предметами. Такие мысли (медики называют их обсессивными) вызывают тревогу, повторяются и начинают восприниматься как реальность. Жизнь человека становится кошмаром. Можно привести пример, когда больной до обеда 60 раз мыл руки, чтобы не заразиться инфекцией, и все равно боялся. Другой больной не мог доехать до работы, потому что постоянно возвращался домой проверить, не включен ли газ.")
        bot.send_sticker(call.message.chat.id, 'CAACAgIAAxkBAAEB471gLBJovffGyBSX5QaoqEWaxucFxgACdxAAAowt_QeBK5ZxqJA0yB4E')

    if call.data == "hellblade":
        bot.send_message(call.message.chat.id, "Психоз – это форма расстройства, при котором психические реакции больного сильно противоречат реальности. Это состояние может быть как самостоятельным заболеванием, так и частью другой болезни психики. Психоз развивается постепенно, и сначала симптомы бывает трудно заметить. Болезнь начинается с небольших перемен в характере и поведении, далее появляется всё больше признаков вплоть до галлюцинаций.")
        bot.send_sticker(call.message.chat.id, 'CAACAgIAAxkBAAEB48VgLBKcCLOLcswP2d3pLu8CFTVwlwACfxAAAowt_QdOrMDsth4lcx4E')

    bot.send_message(call.message.chat.id, "На сегодня лечение окончено, но санитаров я все равно уже вызвал, возвращайся в палату.")

bot.polling(none_stop=True, interval=0)
