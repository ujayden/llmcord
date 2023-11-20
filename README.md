# gpt-discord (by jakobdylanc)
The best ChatGPT experience for your Discord server.
![](https://github.com/jakobdylanc/gpt-discord/assets/38699060/e496bb18-616a-40ac-93f4-42fe09488747)

# Features
### REPLY-BASED CHAT HISTORY
Mention (@) the bot and it will reply to you. Reply to any message to continue the conversation from that point. The chat history is built from reply chains.

### STREAMED RESPONSES
The bot's replies start generating instantly rather than having to wait longer for one big chunk.

### VISION SUPPORT
The bot can see image attachments when set to the ***gpt-4-turbo-vision*** model.

### AND MORE...
- Easily set a custom personality
- User identity aware
- Fully asynchronous
- 1 Python file, <100 lines of code

# Instructions
> Before you start, install Python and clone this git repo.
1. Install Python requirements:
```bash
pip install -r requirements.txt
```

2. Create _.env_ from _.env.example_ and set it up:

| Setting | Instructions |
| --- | --- |
| DISCORD\_BOT_TOKEN | Create a new Discord application at [discord.com/developers/applications](https://discord.com/developers/applications) and generate a token under the ***Bot*** tab. Also enable ***MESSAGE CONTENT INTENT***. |
| OPENAI\_API_KEY | Generate an OpenAI API key at [platform.openai.com/account/api-keys](https://platform.openai.com/account/api-keys). You must also add a payment method to your OpenAI account at [platform.openai.com/account/billing/payment-methods](https://platform.openai.com/account/billing/payment-methods).|
| GPT_MODEL | Choose ***gpt-3.5-turbo***, ***gpt-4-turbo*** or ***gpt-4-turbo-vision***. More info on OpenAI models: [platform.openai.com/docs/models](https://platform.openai.com/docs/models) |
| CUSTOM\_SYSTEM_PROMPT | Write practically anything you want to customize the bot's behavior! |

3. Invite the bot to your Discord server with this URL (replace <CLIENT_ID> with your Discord application's client ID found under the ***OAuth2*** tab):
```plaintext
https://discord.com/api/oauth2/authorize?client_id=<CLIENT_ID>&permissions=412317273088&scope=bot
```

4. Run the bot:
```bash
python gpt-discord.py
```
