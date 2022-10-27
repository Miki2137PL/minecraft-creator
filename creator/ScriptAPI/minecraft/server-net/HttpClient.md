---
author: jakeshirley
ms.author: jashir
ms.prod: gaming
title: minecraft/server-net.HttpClient Class
description: Contents of the @minecraft/server-net.HttpClient class.
---
# HttpClient Class
>[!IMPORTANT]
>These APIs are experimental as part of the Beta APIs experiment. As with all experiments, you may see changes in functionality in updated Minecraft versions. Check the Minecraft Changelog for details on any changes to Beta APIs. Where possible, this documentation reflects the latest updates to APIs in Minecraft beta versions.

## Methods
- [cancelAll](#cancelall)
- [get](#get)
- [request](#request)
- [testOnly_fulfillRequest](#testonly_fulfillrequest)
- [testOnly_getRequests](#testonly_getrequests)
- [testOnly_rejectRequest](#testonly_rejectrequest)

### **cancelAll**
`
cancelAll(reason: string): void
`

Cancels all pending requests.

#### **Parameters**
- **reason**: *string*

### **get**
`
get(uri: string): Promise<HttpResponse>
`

Performs a simple HTTP get request.

#### **Parameters**
- **uri**: *string*
  
  URL to make an HTTP Request to.

#### **Returns** Promise&lt;[*HttpResponse*](HttpResponse.md)&gt; - An awaitable promise that contains the HTTP response.

### **request**
`
request(config: HttpRequest): Promise<HttpResponse>
`

Performs an HTTP request.

#### **Parameters**
- **config**: [*HttpRequest*](HttpRequest.md)
  
  Contains an HTTP Request object with configuration data on the HTTP request.

#### **Returns** Promise&lt;[*HttpResponse*](HttpResponse.md)&gt; - An awaitable promise that contains the HTTP response.

### **testOnly_fulfillRequest**
`
testOnly_fulfillRequest(requestId: number, headers: HttpHeader[], body: string, status: number): void
`

#### **Parameters**
- **requestId**: *number*
- **headers**: [*HttpHeader*](HttpHeader.md)[]
- **body**: *string*
- **status**: *number*

### **testOnly_getRequests**
`
testOnly_getRequests(): number[]
`

#### **Returns** *number*[]

### **testOnly_rejectRequest**
`
testOnly_rejectRequest(requestId: number, reason: string): void
`

#### **Parameters**
- **requestId**: *number*
- **reason**: *string*