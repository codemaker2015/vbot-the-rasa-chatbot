# VBot - Rasa Chatbot

![](demo/demo.gif)

VBot is live on AWS. [Click here](http://54.193.138.236/) to test it

## Installation
First, clone this repo using `git clone https://github.com/codemaker2015/vbot-the-rasa-chatbot`

- Create a virtual environment
```
python -m venv venv
```
- Activate the virtual environment  
Windows : `venv/Scripts/activate`    
Linux : `source venv/bin/activate`
- Upgrade pip
```
python -m pip install --upgrade pip
```
- Install Rasa into the virtual environment 
```
pip install rasa
```
- Initialize rasa chatbot
```
rasa init
```
- Run the rasa server 
```
rasa run -m models --enable-api --cors "*"
```
- For training the model
```
rasa train --config config.yml --domain domain.yml --data data/
```

