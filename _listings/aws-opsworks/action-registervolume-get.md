---
swagger: "2.0"
info:
  title: AWS OpsWorks API Register Volume
  version: 1.0.0
  description: Registers an Amazon EBS volume with a specified stack.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=RegisterVolume:
    get:
      summary: ' Register Volume '
      description: Registers an Amazon EBS volume with a specified stack
      operationId: registerVolume
      parameters:
      - in: query
        name: Ec2VolumeId
        description: The Amazon EBS volume ID
        type: string
      - in: query
        name: StackId
        description: The stack ID
        type: string
      responses:
        200:
          description: OK
      tags:
      - volumes
definitions: []
x-collection-name: AWS OpsWorks
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---