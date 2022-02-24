---
parent: SEE integration top
title: /masterdata endpoints for HIS integrations
has_children: true
nav_order: 1
---

# Overview

# Authentication

# POST /masterdata: create new dictation metadata
Sample code:


```csharp
// Insert a new, hard-defined MasterData record to the SEEMASTERDATA SQL DB
    internal static async Task InsertNewMasterDataRecordInTask()
    {
        // Attach the POST /masterdata/dataitems REST endpoint to the root url
        var masterDataPostEndPointUri = new Uri(new Uri(SEEAppInterfaceServiceUrl), "/SEEAppInterface/masterdata/dataitems");
        // Create an 'InsertMasterDataRequest' json request object
        var request = CreateTestMasterDataRecord();

        HttpClient httpClient = new HttpClient();
        // Set the API key in the request header for authentication
        httpClient.DefaultRequestHeaders.Add("x-sps-api-key", "AdminApiKey_TestGroup_678e1f10-53b0-4b8d-af36-7067b52466ea");
        // Call the POST /masterdata/dataitems endpoint with the predefined json request
        var result = await httpClient.PostAsJsonAsync(masterDataPostEndPointUri, request);
        result.EnsureSuccessStatusCode();
    }
```
