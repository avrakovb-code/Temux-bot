# Temux-bot
Telegram bot
import telebot

TOKEN = "SENING_BOT_TOKENING"  # bu yerga o'z bot tokeningni yoz!

bot = telebot.TeleBot(TOKEN)

@bot.message_handler(commands=['start'])
def start(message):
    bot.reply_to(message, "Salom! Men Render’da 24/7 ishlaydigan botman 🤖")

bot.infinity_polling()
