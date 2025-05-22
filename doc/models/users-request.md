
# Users Request

## Structure

`UsersRequest`

## Fields

| Name | Type | Tags | Description |
|  --- | --- | --- | --- |
| `username` | `str` | Optional | User's username |
| `age` | `int` | Required | User's age |
| `is_active` | `bool` | Optional | Whether the user is active |
| `rating` | `float` | Optional | User's rating |
| `signup_date` | `date` | Required | Signup date |

## Example (as JSON)

```json
{
  "username": "username4",
  "age": 140,
  "isActive": false,
  "rating": 194.34,
  "signupDate": "2016-03-13"
}
```

