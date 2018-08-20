# TDLPolicy
Confirmed and allowed Policies for the Topic Description Language (TDL)

To add new policies into the TDL make a new file inside directory **policy**

## Structure of a policy file



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