---
swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 0
info:
  title: AWS CloudFront API Create Distribution
  version: 1.0.0
  description: Creates a new web distribution.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=CreateDistribution:
    get:
      summary: Create Distribution
      description: Creates a new web distribution.
      operationId: createDistribution
      x-api-path-slug: actioncreatedistribution-get
      parameters:
      - in: query
        name: CreateDistributionRequest
        description: Root level tag for the CreateDistributionRequest parameters
        type: string
      - in: query
        name: DistributionConfig
        description: The distributions configuration information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this request
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: VpcIds.N
        description: One or more VPC IDs
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
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