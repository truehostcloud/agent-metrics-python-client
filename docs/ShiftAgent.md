# ShiftAgent


## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**id** | **int** |  | [optional] [readonly] 
**agent_name** | **str** |  | [optional] 
**agent_id** | **str** |  | [optional] 
**shift_status** | **str** |  | [optional] 
**shift_start_time** | **str** |  | [optional] 
**shift_end_time** | **str** |  | [optional] 
**communication_channels** | **str** | Communication channels this agent handles | [optional] 
**email** | **str** | Agent email address | [optional] 
**operator_id** | **str** | Supportpal Operator ID | [optional] 
**department_ids** | **List[int]** | Departments this operator belongs to | [optional] 

## Example

```python
from agent_metrics_client.models.shift_agent import ShiftAgent

# TODO update the JSON string below
json = "{}"
# create an instance of ShiftAgent from a JSON string
shift_agent_instance = ShiftAgent.from_json(json)
# print the JSON string representation of the object
print(ShiftAgent.to_json())

# convert the object into a dict
shift_agent_dict = shift_agent_instance.to_dict()
# create an instance of ShiftAgent from a dict
shift_agent_from_dict = ShiftAgent.from_dict(shift_agent_dict)
```
[[Back to Model list]](../README.md#documentation-for-models) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to README]](../README.md)


