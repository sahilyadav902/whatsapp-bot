# embedchain whatsapp-bot

## Setup
- Register for a free account on [Twilio](https://www.twilio.com/try-twilio) and create a new Whatsapp Sandbox.
- You can find it in the left Sidebar under `Develop` by navigating to `Messaging>Try it out>Send a WhatsApp Message`.
- To connect a phone number to allow it to chat with the bot, follow the on screen instructions.
- Now register for an account on ngrok website [here](https://dashboard.ngrok.com/signup).
- To download and setup ngrok, follow the instructions [here](https://dashboard.ngrok.com/get-started/setup) after logging in.
- Claim the free static domain for tunneling offered by ngrok under `Tunnels` in the left Sidebar.
- Copy the static domain link, add `/chat` at the end of the link and paste it under `When a message comes in` under the `Sandbox settings` for Whatsapp in Twilio. Save your settings.
- Clone the repo, create and activate your virtual environment. Install the packages in `requirements.txt`.
- Rename the `sample.env` to `.env` and add your Open AI API Key in it.
- Run the bot using the command:
```bash
python bot.py
```
- In a new terminal, start your tunneling using ngrok and the static domain you created earlier as follows:
```bash
.\ngrok http --domain=<your_static_domain_link_here> 5000
```
- Now your whatsapp bot is online and running.

## Usage
- To allow a new number or reconnect an old number with the Sandbox, follow the instructions in your Twilio account.
- To add data sources to your bot, use the following command:
```text
Add <data_type> <url_or_text>
```
- To chat with the bot, you can simply ask any question from it.

## Supported Data Types
Please use the following keywords for the data_type argument to add data sources to the bot:
- Youtube Video - youtube_video
- PDF file - pdf_file
- Web Page - web_page
- Site Map - sitemap
- Doc file - docx
- Code documentation website - docs_site
- Text Data - text