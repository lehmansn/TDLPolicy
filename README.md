# TDLPolicy
Confirmed and allowed Policies for the Topic Description Language (TDL)

To add new Policies into the TDL make a new file inside directory **policy**

## Structure of a Policy file

* name: The name of this Policy
* description: Descripe the use of your new Policy
* policytype: [topic, message] Policy for the topic or Policy for the messaging, choose your category
* input: Values a topic provider can define by itself
* example: One example to explain your Policy

Example: 
```
{
  "name": "accuracy",
  "description": "Describes to accuracy of all published values of the topic",
  "policytype": "message",
  "input": {
    "name": "string",
    "accuracy": "number"
  },
  "example": {
    "name": "accuracy",
    "accuracy": 0.001
  }
}
```