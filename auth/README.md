
## API Reference

#### Set up SSH key on all running servers
```http
  POST /auth
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |
| `pub_key`     | `string` | **Required**. SSH Public Key (RSA)|

##### Response
```json
{
    "task_id": "xQbB37gt85UHQfjApbju"
}
```


#### Set up SSH key on all servers in a project
```http
  POST /auth
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |
| `pub_key`     | `string` | **Required**. SSH Public Key (RSA)|
| `project_id`    | `integer` | **Required**. Numeric id of the project    |

##### Response
```json
{
    "task_id": "a2PQ8NLoLIRypvzf7X3e"
}
```

#### Set up SSH key on a single server
```http
  POST /auth
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |
| `pub_key`     | `string` | **Required**. SSH Public Key (RSA)|
| `server_id`    | `integer` | **Required**. Numeric id of the server    |

##### Response
```json
{
    "task_id": "cPOQ8NLRLIRypcezf7X3e"
}
```