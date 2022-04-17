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
### Install tts
```
git submodule update --force --recursive --init --remote
pip install -e .  # this is necessary!
```

### Use tts
```
# Transfer Hanzi to Pinyin
cd examples/aishell3/
python ../../mtts/text/gp2py.py -t "为适应新的网络传播方式和读者阅读习惯"
>> sil wei4 shi4 ying4 xin1 de5 wang3 luo4 chuan2 bo1 fang1 shi4 he2 du2 zhe3 yue4 du2 xi2 guan4 sil|sil 为 适 应 新 的 网 络 传 播 方 式 和 读 者 阅 读 习 惯 sil
# Add to input txt file
# Generate output files
python ../../mtts/synthesize.py  -d cuda -c config.yaml --checkpoint ./checkpoints/checkpoint_1350000.pth.tar -i input.txt
```
---
### Models
[SpaCy Models](https://spacy.io/models)  
[vosk Models](https://alphacephei.com/vosk/models)  
[aishell3 checkpoints](https://zenodo.org/record/4912321#.YMN2-FMzakA)  
[biaobei checkpoints](https://zenodo.org/record/4910507#.YMN29lMzakA)