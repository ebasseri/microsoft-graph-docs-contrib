---
title: "Delete educationModuleResource"
description: "Delete a specific resource attached to a module."
author: "v-rmanda"
ms.localizationpriority: medium
ms.prod: "education"
doc_type: apiPageType
---

# Delete educationModuleResource

Namespace: microsoft.graph

Delete a specific [educationModuleResource](../resources/educationmoduleresource.md) attached to a [module](../resources/educationmodule.md). Only teachers in the class can remove a resource.

[!INCLUDE [national-cloud-support](../../includes/global-only.md)]

## Permissions

Choose the permission or permissions marked as least privileged for this API. Use a higher privileged permission or permissions [only if your app requires it](/graph/permissions-overview#best-practices-for-using-microsoft-graph-permissions). For details about delegated and application permissions, see [Permission types](/graph/permissions-overview#permission-types). To learn more about these permissions, see the [permissions reference](/graph/permissions-reference).

<!-- { "blockType": "permissions", "name": "educationmoduleresource_delete" } -->

[!INCLUDE [permissions-table](../includes/permissions/educationmoduleresource-delete-permissions.md)]

## HTTP request

<!-- { "blockType": "ignored" } -->

```http
DELETE /education/classes/{class-id}/modules/{module-id}/resources/{resource-id}

```

## Request headers

| Header        | Value                     |
| :------------ | :------------------------ |
| Authorization | Bearer {token}. Required. |

## Request body

Don't supply a request body for this method.

## Response

If successful, this method returns a `204 No Content` response code. It doesn't return anything in the response body.

## Example

### Request

The following example shows a request.

<!-- {
  "blockType": "request",
  "name": "delete_educationmoduleresource"
}-->

```http
DELETE https://graph.microsoft.com/v1.0/education/classes/37d99af7-cfc5-4e3b-8566-f7d40e4a2070/modules/24eda3bf-32e5-4c70-a14d-831e606a2e4f/resources/22bd9723-a559-4b57-989b-af3af36cd902
```

### Response

The following example shows the response.

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```
