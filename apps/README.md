
## API Reference

#### Get all server applications
```http
  GET /apps
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token. |
| `server_id`     | `integer` | **Required**. Numeric id of the server.|

##### Response
```json
  {
    "apps": [
        {
            "application": "phpstack",
            "id": "4280717",
            "master_user": "master_wupxgujtga",
            "server_id": "1205641",
            "server_ip": "157.245.117.13",
            "sys_user": "kdqpvenvft"
        },
        {
            "application": "phpstack",
            "id": "4381141",
            "master_user": "master_wupxgujtga",
            "server_id": "1205641",
            "server_ip": "157.245.117.13",
            "sys_user": "cvxedyradc"
        },
        {
            "application": "phpstack",
            "id": "4381149",
            "master_user": "master_wupxgujtga",
            "server_id": "1208649",
            "server_ip": "157.245.117.146",
            "sys_user": "bgapwqvwnr"
        }
    ]
}
```


#### Get all project applications
```http
  GET /apps
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token. |
| `project_id`    | `integer` | **Required**. Numeric id of the project    |

##### Response
```json
{
    "apps": [
        {
            "application": "wordpress",
            "id": "4147577",
            "master_user": "master_xwtjjroaqu",
            "server_id": "1131021",
            "server_ip": "178.102.10.11",
            "sys_user": "axtxgplmrc"
        },
        {
            "application": "phpstack",
            "id": "4380777",
            "master_user": "master_euaxgpjtgv",
            "server_id": "7202642",
            "server_ip": "178.102.10.101",
            "sys_user": "ydqpvenvqt"
        }
    ]
}
```