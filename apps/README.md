
## API Reference

#### Get all items

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `server_id`     | `string` | ID of the server to set up SSH keys on.     |
| `project_id`    | `string` | ID of the project to set up SSH keys on.    |
| `pub_key`       | `string` | **Required**. SSH public key for setup.     |
| `email`         | `string` | **Required**. Email address for the user.   |
| `Authorization` | `string` | **Required**. Access token.                 |


#### Get item

```http
  GET /api/items/${id}
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `id`      | `string` | **Required**. Id of item to fetch |



