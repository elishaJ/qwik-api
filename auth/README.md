
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


#### Set up SSH key on all project servers
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
<!-- 
#### Get item

```http
  GET /api/items/${id}
```
| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `server_id`     | `string` | ID of the server to set up SSH keys on.     |
| `project_id`    | `string` | ID of the project to set up SSH keys on.    |
| `pub_key`       | `string` | **Required**. SSH public key for setup.     |
| `email`         | `string` | **Required**. Email address for the user.   |
| `Authorization` | `string` | **Required**. Access token.                 | -->
