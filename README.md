# PG-JED
This application utilizes google's speech to text API, open source NLP libraries
and some personal touches to flag if a <1min audio file contains explicit language or not.

## usage:
To envoke the program via the command line, pass in one argument (the path to an audio file) to the listen.py script.
example in linux/bash shell:  $ python listen.py audio_files/Voice_001.m4a

Returns True if explicit language is detected, else False. 

## requirments:
In order to convert audio files into .WAV, you must install ffmpeg and expose that binary to windows PATH ie: C:\Users\Daniel\Downloads\ffmpeg-20190505-e384f6f-win64-static\bin

Must set your own google API key within SpeechToText.py by setting os.environ["GOOGLE_APPLICATION_CREDENTIALS"] = "\<path to json file containing api key\>"

See requirements.txt for environment packages

