---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodelssecurity "github.com/microsoftgraph/msgraph-sdk-go/models/security"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodelssecurity.NewUserSource()
email := "admin@contoso.com"
requestBody.SetEmail(&email)
includedSources := graphmodels.MAILBOX, SITE_SOURCETYPE
requestBody.SetIncludedSources(&includedSources)

userSources, err := graphClient.Security().Cases().EdiscoveryCases().ByEdiscoveryCaseId("ediscoveryCase-id").Custodians().ByEdiscoveryCustodianId("ediscoveryCustodian-id").UserSources().Post(context.Background(), requestBody, nil)


```