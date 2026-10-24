# VideoCallTranslator for Cursor

Set up live translated video calls without leaving Cursor. Ask the agent for a
call with someone who speaks another language: it creates a room on your
[VideoCallTranslator](https://videocalltranslator.com) account and gives you
two links, one that starts the call for you and one to send to the other
person. They open it in any browser, with no app and no account, and each of
you hears the other in your own language. 41 languages.

## What it can do

| Tool                  | What it does                                                                  |
| --------------------- | ----------------------------------------------------------------------------- |
| `list_call_languages` | The languages a call can use.                                                 |
| `create_call_room`    | Creates a room in your language and, if you say it, the other person's. Free. |
| `list_my_rooms`       | Your open rooms, with their languages, last call date and links.              |
| `get_minutes_balance` | Translation minutes left, and where to buy more.                              |

It cannot start, join or listen to a call, buy or spend minutes, or send
messages. The call itself happens on videocalltranslator.com.

## Setup

1. Install the plugin from the Cursor Marketplace.
2. You need a VideoCallTranslator account: [create one](https://videocalltranslator.com/signup)
   if you have not. New accounts start with 30 free minutes.
3. The first time the agent uses a tool, Cursor opens our sign-in page. Sign
   in, then press **Allow** on the approval page. To connect read-only (list
   rooms and check minutes, but not create rooms), untick **Create new rooms on
   your account** first.

No API key or token goes in this plugin or your settings: sign-in is OAuth 2.1
with PKCE, against `https://videocalltranslator.com/mcp`.

## Try it

- "Which languages can a VideoCallTranslator call use?"
- "Set up a translated call with my grandmother, she speaks Spanish."
- "Create a room called Weekly client call. I speak English and my client speaks Japanese."
- "Show my VideoCallTranslator rooms."
- "How many translation minutes do I have left?"

## Privacy and disconnecting

The agent receives the call languages, your rooms' names, languages, dates and
links, and your minutes balance. Never your email, your guests' names, your
call history, anything said on a call, or payment details. Calls are not
recorded. To disconnect, go to **Account → Settings → Connected assistants** on
videocalltranslator.com and press **Disconnect**.

- Documentation: [connector reference](https://videocalltranslator.com/blog/videocalltranslator-connector-reference)
- [Privacy policy](https://videocalltranslator.com/privacy) · [Terms](https://videocalltranslator.com/terms)
- Support: contact@videocalltranslator.com

VideoCallTranslator is operated by Sevenfires AI LLC.
