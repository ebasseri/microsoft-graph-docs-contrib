---
description: "Automatically generated file. DO NOT MODIFY"
---

```bash

// THE CLI IS IN PREVIEW. NON-PRODUCTION USE ONLY
mgc-beta users mail-folders message-rules create --user-id {user-id} --mail-folder-id {mailFolder-id} --body '{
\
    "displayName": "From partner",
\
    "sequence": 2,
\
    "isEnabled": true,
\
    "conditions": {
\
        "senderContains": [
\
          "adele"
\
        ]AlexW@contoso.com
\
     },
\
     "actions": {
\
        "forwardTo": [
\
          {
\
             "emailAddress": {
\
                "name": "Alex Wilbur",
\
                "address": "AlexW@contoso.com"
\
              }
\
           }
\
        ],
\
        "stopProcessingRules": true
\
     }
\
}
\

\
'

```