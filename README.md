# Text-to-Speech-Speech-to-text

def text_to_speech(text, lang='en'):
    tts = gTTS(text=text, lang=lang, slow=False)
    # Save the audio file
    tts.save("output.mp3")
    
    # Play the audio
    return Audio("output.mp3", autoplay=True)

#  Call the function with your text
text = "Hello! Welcome Afra in AI engineering feild"
text_to_speech(text)
