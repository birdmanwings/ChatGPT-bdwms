# ChatGPT-MS
This repo is named by ChatGPT for Multi-Session ChatGPT API.

The main code is copied from [PyChatGPT](https://github.com/rawandahmad698/PyChatGPT).

## Multi-Session ChatGPT (`Generated by ChatGPT`)
There are several reasons why separated sessions are better than having everyone in one session when using a language model like GPT-3. 

First, having separate sessions allows for more personalized and focused conversations. In a single session with multiple people, the conversation can quickly become chaotic and difficult to follow. With separate sessions, each person can have their own dedicated conversation with the language model, allowing for more focused and coherent discussions.

Second, separate sessions can improve the performance of the language model. In a single session with multiple people, the language model may have difficulty understanding who is speaking and what they are talking about. With separate sessions, the language model can focus on a single speaker at a time, which can improve its ability to generate relevant and appropriate responses.

Third, separate sessions can improve the overall user experience. In a single session, it can be difficult for users to keep track of the conversation and understand who is speaking. With separate sessions, each user can have their own dedicated space to engage with the language model, which can make the conversation more intuitive and enjoyable.

Overall, separated sessions are generally considered to be better than having everyone in one session when using a language model like GPT-3. They can improve the performance of the model, provide a more personalized and focused conversation, and improve the overall user experience.

# Disclaimer
This is not an official OpenAI product. This is a personal project and is not affiliated with OpenAI in any way. Don't sue me.

# Setup
## Install
```
git clone --recurse-submodules https://github.com/shiyemin/ChatGPT-MS
pip install -r requirements.txt
```

## Configuration
`cp config.json.example config.json`
* Update config.json

## Start API server
`python server.py`

## Use API
```
curl -d '{"message":"Who are you?", "user": "shiyemin"}' -H "Content-Type: application/json" -X POST http://localhost:5000/chat
```