---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash

// THE CLI IS IN PREVIEW. NON-PRODUCTION USE ONLY
mgc users send-mail post --user-id {user-id} --body '{
\
  "message": {
\
    "subject": "Meet for lunch?",
\
    "body": {
\
      "contentType": "Text",
\
      "content": "The meganb@contoso.com
\
    },
\
    "toRecipients": [
\
      {
\
        "emailAddress": {
\
          "address": "meganb@contoso.com"
\
        }
\
      }
\
    ],
\
    "attachments": [
\
      {
\
        "@odata.type": "#microsoft.graph.fileAttachment",
\
        "name": "attachment.txt",
\
        "contentType": "text/plain",
\
        "contentBytes": "SGVsbG8gV29ybGQh"
\
      }
\
    ]
\
  }
\
}
\
'

```