# IoTHubClient_LL_UploadToBlob()

This API uploads to Azure Storage the content pointed to by source having the size under the blob name devicename/.

## Syntax

\#include "[azure-iot-sdk-c/iothub_client/inc/iothub_client_ll.h](../iot-c-ref-iothub-client-ll-h.md)"  
```C
IOTHUB_CLIENT_RESULT IoTHubClient_LL_UploadToBlob(
  IOTHUB_CLIENT_LL_HANDLE  iotHubClientHandle,
  const char *             destinationFileName,
  const unsigned char *    source,
  size_t                   size
);
```

## Parameters
* `iotHubClientHandle` The handle created by a call to the create function. 

* `destinationFileName` name of the file. 

* `source` pointer to the source for file content (can be NULL) 

* `size` the size of the source in memory (if source is NULL then size needs to be 0).

## Return Value
IOTHUB_CLIENT_OK upon success or an error code upon failure.

