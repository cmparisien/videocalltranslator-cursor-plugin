---
name: translated-video-calls
description: Set up a live translated video call with someone who speaks another language, using VideoCallTranslator. Use when the user wants to call, meet or interview someone in another language, asks for a translated call or room, or asks about their VideoCallTranslator rooms or translation minutes.
---

# Translated video calls

VideoCallTranslator runs one-to-one video calls in the browser with live
spoken translation both ways. Its MCP server gives you four tools:

- `list_call_languages`: the languages a call can use.
- `create_call_room`: a room on the user's account. Returns a host link (the user
  opens it to start the call) and a guest link (the user sends it to the other
  person, who needs no app or account).
- `list_my_rooms`: the user's open rooms, their languages and links.
- `get_minutes_balance`: translation minutes left, and where to buy more.

## When the user asks for a call

1. If they named the other person's language, pass it; otherwise leave it out
   and the guest picks it before joining. Their own language defaults to the
   one on their account.
2. Create the room and give both links, saying clearly which is which. Never
   send the guest link anywhere yourself: the user shares it.
3. Creating a room is free. Minutes are only used while both people are
   connected, so mention the balance only if it is low or the user asks.

You cannot start, join or listen to a call, buy minutes, or send messages.
