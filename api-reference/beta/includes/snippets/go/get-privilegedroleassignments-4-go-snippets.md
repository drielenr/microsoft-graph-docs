---
description: "Automatically generated file. DO NOT MODIFY"
---

```go

//THE GO SDK IS IN PREVIEW. NON-PRODUCTION USE ONLY
graphClient := msgraphsdk.NewGraphServiceClient(requestAdapter)


requestFilter := "isElevated eq true and expirationDateTime ne null or isElevated eq false"

requestParameters := &graphconfig.PrivilegedRoleAssignmentsRequestBuilderGetQueryParameters{
	Filter: &requestFilter,
}
configuration := &graphconfig.PrivilegedRoleAssignmentsRequestBuilderGetRequestConfiguration{
	QueryParameters: requestParameters,
}

result, err := graphClient.PrivilegedRoleAssignments().GetWithRequestConfigurationAndResponseHandler(configuration, nil)


```