# translator-task
from deep_translator import GoogleTranslator

msg = input("Enter a sentence you want to translate: ")
lang = input('''Enter the language to translate: 
             (English => en, Arabic => ar, French => fr, German => de, Russian => ru
              Turkish => tr ): ''')

result = GoogleTranslator(source='auto', target= lang ).translate(msg)
print(f"Translated message: {result}") 
