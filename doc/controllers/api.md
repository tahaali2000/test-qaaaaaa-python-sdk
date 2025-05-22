# API

```python
client_controller = client.client
```

## Class Name

`APIController`

## Methods

* [Getusers](../../doc/controllers/api.md#getusers)
* [Createanewuser](../../doc/controllers/api.md#createanewuser)


# Getusers

Returns a list of users, optionally filtered by search.

```python
def getusers(self,
            search=None,
            limit=None)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `search` | `str` | Query, Optional | Filter users by search term |
| `limit` | `int` | Query, Optional | Limit the number of users returned |

## Response Type

[`List[UsersResponse]`](../../doc/models/users-response.md)

## Example Usage

```python
result = client_controller.getusers()
```


# Createanewuser

Creates a user with default values if not provided.

```python
def createanewuser(self,
                  body)
```

## Parameters

| Parameter | Type | Tags | Description |
|  --- | --- | --- | --- |
| `body` | [`UsersRequest`](../../doc/models/users-request.md) | Body, Required | - |

## Response Type

[`UsersResponse1`](../../doc/models/users-response-1.md)

## Example Usage

```python
body = UsersRequest(
    age=2,
    signup_date=dateutil.parser.parse('2016-03-13').date()
)

result = client_controller.createanewuser(body)
```

