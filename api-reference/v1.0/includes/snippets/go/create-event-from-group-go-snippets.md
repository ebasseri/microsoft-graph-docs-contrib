---
description: "Automatically generated file. DO NOT MODIFY"
---

```go


import (
	  "context"
	  msgraphsdk "github.com/microsoftgraph/msgraph-sdk-go"
	  graphmodels "github.com/microsoftgraph/msgraph-sdk-go/models"
	  //other-imports
)

graphClient := msgraphsdk.NewGraphServiceClientWithCredentials(cred, scopes)


requestBody := graphmodels.NewEvent()
subject := "Let's go for lunch"
requestBody.SetSubject(&subject)
body := graphmodels.NewItemBody()
contentType := graphmodels.HTML_BODYTYPE
body.SetContentType(&contentType)
content := "Does late morning work for you?"
body.SetContent(&content)
requestBody.SetBody(body)
start := graphmodels.NewDateTimeTimeZone()
dateTime := "2019-06-16T12:00:00"
start.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
start.SetTimeZone(&timeZone)
requestBody.SetStart(start)
end := graphmodels.NewDateTimeTimeZone()
dateTime := "2019-06-16T14:00:00"
end.SetDateTime(&dateTime)
timeZone := "Pacific Standard Time"
end.SetTimeZone(&timeZone)
requestBody.SetEnd(end)
location := graphmodels.NewLocation()
displayName := "Harry's Bar"
location.SetDisplayName(&displayName)
requestBody.SetLocation(location)


attendee := graphmodels.NewAttendee()
emailAddress := graphmodels.NewEmailAddress()
address := "adelev@contoso.com"
emailAddress.SetAddress(&address)
name := "Adele Vance"
emailAddress.SetName(&name)
attendee.SetEmailAddress(emailAddress)
type := graphmodels.REQUIRED_ATTENDEETYPE
attendee.SetType(&type)

attendees := []graphmodels.Attendeeable {
	attendee,
}
requestBody.SetAttendees(attendees)

events, err := graphClient.Groups().ByGroupId("group-id").Events().Post(context.Background(), requestBody, nil)


```