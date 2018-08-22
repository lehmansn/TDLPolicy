# TDLPolicy
Confirmed and allowed Policies for the Topic Description Language (TDL)

To add new Policies into the TDL make a new file inside directory **policy**

## Structure of a Policy file

* policy_type: The name of this Policy type
* description: Descripe the use of your new Policy
* policy_category: [topic, message] Policy for the topic or Policy for the messaging, choose your category
* url(optional): An icon for this Policy type
* input: Values a topic provider can define by itself
* example: One example to explain your Policy

Example: 
```
{
  "policy_type": "accuracy",
  "description": "Describes the accuracy of all published values of the topic",
  "policy_category": "message",
  "input": [
    {
      "value": "name",
      "datatype": "string",
      "description": "Unique name of this policy"
    },
    {
      "value": "accuracy",
      "datatype": "number",
      "description": "Accuracy of the sensor publishing values to the topic"
    }
  ],
  "example": {
    "name": "accuracy",
    "accuracy": 0.001
  }
}
```
