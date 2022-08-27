# Flask Blog App

A Simple blog app using flask and mysql

## API Reference

#### Get all posts

```http
  GET /
```

### Get Slug

```http
  GET /post/<string:post_slug>
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `post_slug`      | `string` | **Required**. filters slug to fetch |

### Admin Dashboard

```http
  GET /dashboard
```
```http
  POST /dashboard
```
No Parameters.

### Edit Post

```http
  GET /edit/<string:sno>
```
```http
  POST /edit/<string:sno>
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `sno`      | `string` | **Required**. filters post to be edit |

### Delete Post

```http
  GET /delete/<string:sno>
```
```http
  POST /delete/<string:sno>
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `sno`      | `string` | **Required**. filters post to be delete |

### Logout

```http
  GET /logout
```
Simply pops the user session.

### About

```http
  GET /about
```

Gets about page.

### Upload Post

```http
  GET /uploader
```
Uploads file.

### Contact Post

```http
  GET /contact
```
Posts contact.
