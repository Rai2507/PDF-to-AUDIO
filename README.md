# PDF-to-AUDIO

from gtts import gTTS
import os

#enter your text
my_text= "Hello my name is Rai"

#select the language
language= 'en'

output= gTTS(text= my_text, lang= language, slow= False)

output.save("output.mp3")

os.system("start output.mp3")
