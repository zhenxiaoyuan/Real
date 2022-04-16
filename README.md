# Real
A conversational AI chatbot with Rasa

### Install on Mac
```
# new venv
python3 -m venv venv
# activate venv
source venv/bin/activate

# install rasa and spacy
pip install rasa spacy

# initial rasa
rasa init

# train nlu
rasa train

# test
rasa shell
```