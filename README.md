# aps-docker-compose

## Install

- [Docker](https://docs.docker.com/engine/install/) 
- [Docker Compose](https://docs.docker.com/compose/install/)

## Start

```
docker-compose up
```

## Run

- http://localhost:8088/activiti-app/
- User admin@app.activiti.com
- Pass admin

## Document

- https://docs.alfresco.com/process-services1.11/concepts/welcome.html
- https://hub.alfresco.com/t5/alfresco-process-services/ct-p/BPM-software


## Send Email

- Script

```
var processId = execution.getProcessInstanceId();
execution.setVariable("processId", processId);
```

- JSON

```
{
    "To": ["phuchiss.su@gmail.com"],
    "CC": [],
    "Subject": "Test",
    "Body": "Test",
    "ProcessInstanceId": "273532",
    "Special": null,
    "Files": ["NoAttachment"]
}
```
