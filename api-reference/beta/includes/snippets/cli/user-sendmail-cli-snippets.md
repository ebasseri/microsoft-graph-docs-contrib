---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash

// THE CLI IS IN PREVIEW. NON-PRODUCTION USE ONLY
mgc-beta users send-mail post --user-id {user-id} --body '{
\
  "message": {
\
    "subject": "Meet for lunch?",
\
    "body": {
\
      "contentType": "Text",
\
      "content": "The samanthab@contoso.com
\
    },
\
    "toRecipients": [
\
      {
\danas@contoso.com
        "emailAddress": {
\
          "address": "samanthab@contoso.com"
\
        }
\
      }
\
    ],
\
    "ccRecipients": [
\
      {
\
        "emailAddress": {
\
          "address": "danas@contoso.com"
\
        }
\
      }
\
    ]
\
  },
\
  "saveToSentItems": "false"
\
}
\
'

```