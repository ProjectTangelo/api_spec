FORMAT: 1A

# Tangelo API Documentation

##Basics

Response to any request is either an error or the corresponding data.

######Error syntax:
```json
{
  "error": {
    "message": "Your error message"
  }
}
```

## Home Page [/]

### New Node [POST]
Not yet implemented

### Update Node [PUT]
Not yet implemented

### Delete Node [DELETE]
Not yet implemented

## Node [/nodes/{nodeid}]
### Get Node [GET]
Not yet implemented

### Update Node [PUT]
Not yet implemented

### Delete Node [DELETE]
Not yet implemented

## Node Containers [/nodes/{nodeid}/containers]
### Get Node Containers [GET]
Not yet implemented

## Node Container [/nodes/{nodeid}/containers/{containerid}]
### Get Container [GET]
Not yet implemented

### New Container [POST]
Not yet implemented

### Update Container [PUT]
Not yet implemented

### Delete Container [DELETE]
Not yet implemented

## Lesson Plans [/lessons]

### Get Lesson [GET]
Not yet implemented

### New Lesson [POST]
Not yet implemented

### Update Lesson [PUT]
Not yet implemented

### Delete Lesson [DELETE]
Not yet implemented

## Lesson Plan Documents [/lessons/{docid}]

### Get Document [GET]
Not yet implemented

### New Document [POST]
Not yet implemented

### Update Document [PUT]
Not yet implemented

### Delete Document [DELETE]
Not yet implemented

## Users [/user]

### Get Users [GET /user/:id]
Get a user's data by ID. Accepts requests from Admin users or users who are logged in with the same ID.

Response is either the user or an error.
+ as Admin
```json
  {
    "_id": "5509b80c87d6a08b1cf4ac83",
    "username": "tyler",
    "password": "$2a$10$CPUzSlqtXjNxA.oSkJnyhuTFr66yI0CqomejRGbvVDdgalUN0zbdy",
    "__v": 0,
    "type": "user",
    "email": "tyler@tyler.rylet"
  }
```
+ as "tyler"
```json
  {
    "_id": "5509b80c87d6a08b1cf4ac83",
    "username": "tyler",
    "email": "tyler@tyler.rylet"
  }
```


### New Users [POST /user]
Creates a new user. Requires Admin.
#####Fields:
- Username
  - required
- Password
  - required
- Email
  - optional
  - default: ""
- Type
  - optional
  - default: "user"
  - accepted inputs include
    - "admin"
    - "user"

Response is the new user or an error:
```json
{
  "_id": "5509b80c87d6a08b1cf4ac83",
  "username": "tyler",
  "password": "$2a$10$CPUzSlqtXjNxA.oSkJnyhuTFr66yI0CqomejRGbvVDdgalUN0zbdy",
  "__v": 0,
  "type": "user",
  "email": "tyler@tyler.rylet"
}
```

### Update Users [PUT /user/:id]
#####Fields:
Any field accessible to your user level

Response is the updated user or an error:
```json
{
  "_id": "5509b80c87d6a08b1cf4ac83",
  "username": "tyler",
  "password": "$2a$10$CPUzSlqtXjNxA.oSkJnyhuTFr66yI0CqomejRGbvVDdgalUN0zbdy",
  "__v": 0,
  "type": "user",
  "email": "bob@bob.bob"
}
```

### Delete Users [DELETE]
Not yet implemented

## Authentication
## Login [/login]
