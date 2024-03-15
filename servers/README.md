
## API Reference

#### Get IDs of all running servers 
```http
  GET /servers/ids
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |

##### Response
```json
{
    "id": [
        "158925",
        "7202642",
        "1131021"
    ]
}
```
#### Get public IPs of all running servers
```http
  GET /servers/ips
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |

##### Response
```json
{
    "public_ip": [
        "143.110.192.11",
        "178.102.10.11",
        "178.102.10.101"
    ]
}
```

#### Get SSH master usernames of all running servers
```http
  GET /servers/users
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |

##### Response
```json
{
    "master_user": [
        "master_xwtjjrxavu",
        "master_wupxgujtga"
    ]
}
```