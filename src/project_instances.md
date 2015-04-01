# Group Project Instances

## Project Instance [/project_instances/{id}]
Get a single project instance

Each Project Instance has the following properties

- **id**: the id of the project instance
- **project**: project the instance is a part of
- **instance** instance that is part of the project

+ Parameters
  + id (number, required) ... id of the Project Instance.

+ Model (application/json)

    JSON representation of Project Resource

    + Body
        {
          "id": 1,
          "url": "https://atmobeta.iplantc.org/api/v2/project_instances/1",
          "project": {
              "id": 1,
              "url": "https://atmobeta.iplantc.org/api/v2/projects/1",
              "name": "project",
              "description": "description",
              "owner": "user",
              "start_date": "2015-03-17T01:50:51.966674Z",
              "end_date": null
          },
          "instance": {
              "id": 1,
              "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
              "url": "https://atmobeta.iplantc.org/api/v2/instances/1",
              "name": "instance",
              "status": "suspended",
              "size": {
                  "id": 23,
                  "url": "https://atmobeta.iplantc.org/api/v2/sizes/23",
                  "alias": "1",
                  "name": "tiny1",
                  "cpu": 1,
                  "disk": 0,
                  "mem": 4096,
                  "active": true,
                  "start_date": "2014-02-04T19:09:07.655411Z",
                  "end_date": null
              },
              "ip_address": "0.0.0.0",
              "shell": false,
              "vnc": false,
              "identity": {
                  "id": 1,
                  "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                  "url": "https://atmobeta.iplantc.org/api/v2/identities/1",
                  "provider": 4
              },
              "user": {
                  "id": 1,
                  "url": "https://atmobeta.iplantc.org/api/v2/users/1",
                  "username": "user",
                  "first_name": "User",
                  "last_name": "User",
                  "email": "user@useremail.com",
                  "is_staff": true,
                  "is_superuser": true,
                  "date_joined": "2015-02-11T22:37:24Z"
              },
              "provider": {
                  "id": 4,
                  "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                  "url": "https://atmobeta.iplantc.org/api/v2/providers/4",
                  "name": "iPlant Cloud - Tucson",
                  "description": "<No Description Provided>",
                  "public": true,
                  "active": true,
                  "start_date": "2014-02-04T19:09:20.713175Z",
                  "end_date": null
              },
              "image": {
                  "id": 868,
                  "url": "https://atmobeta.iplantc.org/api/v2/images/868",
                  "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                  "name": "functional genomics_v1.0",
                  "description": "For practice bioinfomatics data tools",
                  "icon": null,
                  "start_date": "2014-09-05T18:08:12Z",
                  "end_date": null
              },
              "projects": [
                  1
              ],
              "start_date": "2015-03-03T19:08:06Z",
              "end_date": null
        }


### List all project instances [GET]

+ Parameters
    + project__id (number, optional) ... id of the specific project.

+ Response 200(application/json)

     + Body
        {
            "count": 1,
            "next": null,
            "previous": null,
            "results": [
                {
                "id": 1,
                "url": "https://atmobeta.iplantc.org/api/v2/project_instances/1",
                "project": {
                    "id": 1,
                    "url": "https://atmobeta.iplantc.org/api/v2/projects/1",
                    "name": "project",
                    "description": "description",
                    "owner": "user",
                    "start_date": "2015-03-17T01:50:51.966674Z",
                    "end_date": null
                },
                "instance": {
                    "id": 1,
                    "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                    "url": "https://atmobeta.iplantc.org/api/v2/instances/1",
                    "name": "instance",
                    "status": "suspended",
                    "size": {
                        "id": 23,
                        "url": "https://atmobeta.iplantc.org/api/v2/sizes/23",
                        "alias": "1",
                        "name": "tiny1",
                        "cpu": 1,
                        "disk": 0,
                        "mem": 4096,
                        "active": true,
                        "start_date": "2014-02-04T19:09:07.655411Z",
                        "end_date": null
                    },
                    "ip_address": "0.0.0.0",
                    "shell": false,
                    "vnc": false,
                    "identity": {
                        "id": 1,
                        "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                        "url": "https://atmobeta.iplantc.org/api/v2/identities/1",
                        "provider": 4
                    },
                    "user": {
                        "id": 1,
                        "url": "https://atmobeta.iplantc.org/api/v2/users/1",
                        "username": "user",
                        "first_name": "User",
                        "last_name": "User",
                        "email": "user@useremail.com",
                        "is_staff": true,
                        "is_superuser": true,
                        "date_joined": "2015-02-11T22:37:24Z"
                    },
                    "provider": {
                        "id": 4,
                        "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                        "url": "https://atmobeta.iplantc.org/api/v2/providers/4",
                        "name": "iPlant Cloud - Tucson",
                        "description": "<No Description Provided>",
                        "public": true,
                        "active": true,
                        "start_date": "2014-02-04T19:09:20.713175Z",
                        "end_date": null
                    },
                    "image": {
                        "id": 868,
                        "url": "https://atmobeta.iplantc.org/api/v2/images/868",
                        "uuid": "c2b139c4-d8a6-11e4-b9d6-1681e6b88ec1",
                        "name": "functional genomics_v1.0",
                        "description": "For practice bioinfomatics data tools",
                        "icon": null,
                        "start_date": "2014-09-05T18:08:12Z",
                        "end_date": null
                    },
                    "projects": [
                        1
                    ],
                    "start_date": "2015-03-03T19:08:06Z",
                    "end_date": null
                }
            ]
        }

### Add Instance to Project [POST]
Add instance to project. You must specify the following properties:

 - **project**: project id
 - **instance**: instance id

 + Request (application/json)

        {
          "project": 1,
          "instance": 1
        }

+ Response 200 (application/json)

    [Instance][]

### Remove Instance from Project [DELETE]
+ Response 204 (application/json)


## Single Project Instances[/project_instances{?project__id}]
Get instances in a single project.