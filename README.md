# Real
A conversational AI chatbot with Rasa

### Use virtual environment
```
# New venv
python3 -m venv venv
# Activate venv
source venv/bin/activate
```
---
### Install Rasa
```
# Install Rasa and SpaCy
pip install rasa spacy
```

### Start Rasa
```
# initial rasa
rasa init

# train nlu
rasa train

# test
rasa shell
```
---
### Install vosk
```
# install vosk
pip install vosk sounddevice
```

### Start vosk
```
# Enter vosk folder
cd vosk
# Run scirpt
./test_microphone.py
```
---
### Models
[SpaCy Models](https://spacy.io/models)  
[vosk Models](https://alphacephei.com/vosk/models)