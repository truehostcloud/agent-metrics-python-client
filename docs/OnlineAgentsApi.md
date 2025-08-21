# openapi_client.OnlineAgentsApi

All URIs are relative to *http://localhost:8000*

Method | HTTP request | Description
------------- | ------------- | -------------
[**online_agents_list**](OnlineAgentsApi.md#online_agents_list) | **GET** /online-agents/ | 


# **online_agents_list**
> List[ShiftAgent] online_agents_list()

### Example

* Api Key Authentication (TokenAuth):

```python
import openapi_client
from openapi_client.models.shift_agent import ShiftAgent
from openapi_client.rest import ApiException
from pprint import pprint

# Defining the host is optional and defaults to http://localhost:8000
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost:8000"
)

# The client must configure the authentication and authorization parameters
# in accordance with the API server security policy.
# Examples for each auth method are provided below, use the example that
# satisfies your auth use case.

# Configure API key authorization: TokenAuth
configuration.api_key['TokenAuth'] = os.environ["API_KEY"]

# Uncomment below to setup prefix (e.g. Bearer) for API key, if needed
# configuration.api_key_prefix['TokenAuth'] = 'Bearer'

# Enter a context with an instance of the API client
with openapi_client.ApiClient(configuration) as api_client:
    # Create an instance of the API class
    api_instance = openapi_client.OnlineAgentsApi(api_client)

    try:
        api_response = api_instance.online_agents_list()
        print("The response of OnlineAgentsApi->online_agents_list:\n")
        pprint(api_response)
    except Exception as e:
        print("Exception when calling OnlineAgentsApi->online_agents_list: %s\n" % e)
```



### Parameters

This endpoint does not need any parameter.

### Return type

[**List[ShiftAgent]**](ShiftAgent.md)

### Authorization

[TokenAuth](../README.md#TokenAuth)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

### HTTP response details

| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** |  |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

