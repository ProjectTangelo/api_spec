FORMAT: 1A

# Tangelo API Documentation

## Home Page [/]
### Get Index [GET]
+ Response (application/json)

	{
		"hello": "world"
	}


## Nodes [/nodes]
### Get Nodes [GET]
Get a response from a server
+ Response (application/json)
    [{
        "name" : "node01",
        "size" : "small",
        "memory": {
            "free" : 300, 
            "total" : 1024
        }
    },{
        "name" : "node02",
        "size" : "small",
        "memory": {
            "free" : 120, 
            "total" : 1024
        }
      }]



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

## Users [/users]

### Get Users [GET]
Not yet implemented

### New Users [POST]
Not yet implemented

### Update Users [PUT]
Not yet implemented

### Delete Users [DELETE]
Not yet implemented

## Authencitation
## Login [/login]


