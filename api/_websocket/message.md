---
title: Messages
position: 10
parameters:
  - name:
    content:
content_markdown: |-
  Following is supported message category.

  | category | 
  | --- | 
  | SIGNAL_KEY | 
  | SIGNAL_TEXT | 
  | SIGNAL_IMAGE | 
  | SIGNAL_VIDEO | 
  | SIGNAL_DATA | 
  | SIGNAL_STICKER | 
  | SIGNAL_CONTACT | 
  | PLAIN_TEXT | 
  | PLAIN_IMAGE | 
  | PLAIN_VIDEO | 
  | PLAIN_DATA | 
  | PLAIN_STICKER | 
  | PLAIN_CONTACT | 
  | PLAIN_JSON | 
  | SYSTEM_CONVERSATION | 
  | SYSTEM_ACCOUNT_SNAPSHOT | 
  | APP_BUTTON_GROUP | 
  | APP_CARD | 

  PLAIN_TEXT 
  ```json
    {
      "id": "UUID // generated by client", 
      "action":  "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID",
        "category": "PLAIN_TEXT",
        "status": "SENT",
        "message_id": "UUID // generated by client",
        "data": "Base64 encoded data" ,
      }
    }
  ```

  PLAIN_IMAGE
  ```json
    {
      "id": "UUID",
      "action": "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID"
        "category": "PLAIN_IMAGE"
        "status": "SENT",
        "message_id": "UUID",
        "data": "Base64 encoded data"
      }
    }
   ```

  Date Format
  ```json
    {"attachment_id": "Read From POST /attachments", "mine_type": "", "width": "100", "height": "100", "size": "1000byte", "thumbnail": "base64 encoded"}
  ```

  PLAIN_DATA
  ```json
    {
      "id":  "UUID",
      "action":  "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID",
        "category": "PLAIN_DATA",
        "status": "SENT",
        "message_id": "UUID",
        "data": "Base64 encoded data",
      }
    }
  ```
  Data Format
  ```json
    {"attachment_id": "Read From POST /attachments", "mine_type": "", "size": "1000byte", "name": "Share"}
  ```

  PLAIN_STICKER
  ```json
    {
      "id":  "UUID",
      "action":  "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID",
        "category": "PLAIN_STICKER",
        "status": "SENT",
        "message_id":  "UUID",
        "data": "Base64 encoded data"
      }
    }
  ```
  Data Format
  ```json
    {"name": "hello", "album_id": "UUID"}
  ```

  PLAIN_CONTACT
  ```json
    {
      "id": "UUID",
      "action": "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID",
        "category": "PLAIN_CONTACT"
        "status": "SENT",
        "message_id": "UUID",
        "data":  "Base64 encoded data"
      }
    }
  ```
  Data Format
  ```json
   { "user_id": "UUID"}
  ```

  PLAIN_VIDEO
  ```json
    {
      "id": "UUID",
      "action": "CREATE_MESSAGE",
      "params": {
        "conversation_id": "UUID",
        "category": "PLAIN_VIDEO",
        "status": "SENT",
        "message_id": "UUID",
        "data": "Base64 encoded data"
      }
    }
  ```
  Data Format
  ```json
   {"attachment_id": "Read From POST /attachments", "mine_type": "", "width": "100", "height": "100", "size": "1000byte", "duration": "1000s", "thumbnail": "base64 encoded"}
  ```

  ACKNOWLEDGE_MESSAGE_RECEIPT ack server received message
  ```json
    {
      "id": "UUID",
      "action": "ACKNOWLEDGE_MESSAGE_RECEIPT",
      "params": {
        "message_id": "UUID // message_id is you received message's message_id",
        "status": "READ"
      }
    }
  ```


left_code_blocks:
  - code_block: |-
    title: 
    language: 
right_code_blocks:
  - code_block: |-
      {
        "id": "89e0bdee-c355-47f2-945a-be48be875606",
        "action": "",
        "params": "mRm5rm9bkQztvpsaTyz1Rib0BEM0S1FKl",
        "data": "eyJhbGciOiJSUzUxMiIsInR5cCI6IkpXVCJ9",
      }
    title: Response
    language: json
---
