
## API Reference

#### Delete SSH key(s)
```http
  DELETE /cleanup
```

| Parameter       | Type     | Description                                 |
| :-------------- | :------- | :------------------------------------------ |
| `Authorization` | `string` | **Required**. Access token |
| `task_id`     | `string` | **Required**. Task ID returned by auth endpoint|

##### Response
```json
{
    "success": "Keys deleted successfully"
}
```