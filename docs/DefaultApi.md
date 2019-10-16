# openapi_client.DefaultApi

All URIs are relative to *http://api.mathjs.org/v4*

Method | HTTP request | Description
------------- | ------------- | -------------
[**root_get**](DefaultApi.md#root_get) | **GET** / | Evaluating math.


# **root_get**
> root_get(expr, precision=precision)

Evaluating math.

### Example

```python
from __future__ import print_function
import time
import openapi_client
from openapi_client.rest import ApiException
from pprint import pprint

# Create an instance of the API class
api_instance = openapi_client.DefaultApi()
expr = 'expr_example' # str | The expression to be evaluated. The expression must be url encoded.
precision = 3.4 # float | Number of significant digits in formatted output. Undefined by default. (optional)

try:
    # Evaluating math.
    api_instance.root_get(expr, precision=precision)
except ApiException as e:
    print("Exception when calling DefaultApi->root_get: %s\n" % e)
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **expr** | **str**| The expression to be evaluated. The expression must be url encoded. | 
 **precision** | **float**| Number of significant digits in formatted output. Undefined by default. | [optional] 

### Return type

void (empty response body)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Body contains the result of the expression |  -  |
**400** | Error message in the body |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

