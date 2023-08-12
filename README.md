# Embedchain WhatsApp Bot Template
This is a replit template to create your own WhatsApp bot using the embedchain package.

## Template Setup
- Fork this replit template.
- Set your `OPENAI_API_KEY` in Secrets.
- Register for a free account on [Twilio](https://www.twilio.com/try-twilio) and create a new Whatsapp Sandbox.
- You can find it in the left Sidebar under `Develop` by navigating to `Messaging>Try it out>Send a WhatsApp Message`.
- To connect a phone number and allow it to chat with the bot, follow the on screen instructions.
- Click on `Run` in the replit container and a URL will get generated for your bot.
- Copy the URL, append `/chat` at the end and paste it under `When a message comes in` under the `Sandbox settings` for Whatsapp in Twilio. Save your settings.

## Usage Instructions
- To allow a new number or reconnect an old number with the Sandbox, follow the instructions in your Twilio account.
- To add data sources to the bot, use the command:
```text
add <data_type> <url_or_text>
```
- To ask queries from the bot, use the command:
```text
<question>
```