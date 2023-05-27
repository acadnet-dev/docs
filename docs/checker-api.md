# API description for the Checker

## `/submission/create`
#### Query parameters
* `type` - the problem type (see below for available types)
* `bucket` - the bucket where the problem files are

#### Body
File as multipart/form-data (see below for file type based on problem type)

#### Response
```json
{
    "submission_id": "submission_id"
}
```

## `/submission/status`
#### Query parameters
* `submission_id` - the id of the submission

#### Response
```json
{
    "status": "status",
    "message": "message"
}
```

# Callback
The checker will call the configured callback url after checking a submission. The callback will receive a POST request with the following body:
```json
{
    "submission_id": "submission_id",
    "status": "status",
    "message": "message"
}
```

# Problem types
## SimpleAcadnetIS
The submission is represented by a simple .cpp file that will be compiled. Then the tests found in the problem bucket will be run against the compiled file.
