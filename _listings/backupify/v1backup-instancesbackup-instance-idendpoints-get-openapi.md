---
swagger: "2.0"
x-collection-name: Backupify
x-complete: 0
info:
  title: Backupify Retrieve a list of endpoints for the specified backup_instance
  description: You can only retrieve endpoints for backup_instances you have access
    to. Records are returned in ascending order (by id), with a default of 20 per
    page. Links to the next, previous, first, and last pages can be found in the response
    headers.
  version: 1.0.0
host: api.backupify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/backup_instances/{backup_instance_id}/endpoints:
    get:
      summary: Retrieve a list of endpoints for the specified backup_instance
      description: You can only retrieve endpoints for backup_instances you have access
        to. Records are returned in ascending order (by id), with a default of 20
        per page. Links to the next, previous, first, and last pages can be found
        in the response headers.
      operationId: getV1BackupInstancesBackupInstanceEndpoints
      x-api-path-slug: v1backup-instancesbackup-instance-idendpoints-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer Access Token granted from client credentials authorizing
          vendor to perform action
      - in: path
        name: backup_instance_id
        description: ID of the backup_instance to retrieve an endpoint for
      responses:
        200:
          description: OK
      tags:
      - V1
      - Backup
      - Instances
      - Backup
      - Instance
      - Id
      - Endpoints
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