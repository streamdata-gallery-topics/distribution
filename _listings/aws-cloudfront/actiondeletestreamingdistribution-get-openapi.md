---
swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 0
info:
  title: AWS CloudFront API Delete Streaming Distribution
  version: 1.0.0
  description: Delete a streaming distribution.
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
  /?Action=CreateDistributionWithTags:
    get:
      summary: Create Distribution With Tags
      description: Create a new distribution with tags.
      operationId: createDistributionWithTags
      x-api-path-slug: actioncreatedistributionwithtags-get
      parameters:
      - in: query
        name: CreateDistributionWithTagsRequest
        description: Root level tag for the CreateDistributionWithTagsRequest parameters
        type: string
      - in: query
        name: DistributionConfigWithTags
        description: The distributions configuration information
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance to unlink from the VPC
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC to which the instance is linked
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
      - Tags
  /?Action=CreateStreamingDistribution:
    get:
      summary: Create Streaming Distribution
      description: Creates a new RMTP distribution.
      operationId: createStreamingDistribution
      x-api-path-slug: actioncreatestreamingdistribution-get
      parameters:
      - in: query
        name: CreateStreamingDistributionRequest
        description: Root level tag for the CreateStreamingDistributionRequest parameters
        type: string
      - in: query
        name: StreamingDistributionConfig
        description: The streaming distributions configuration information
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
  /?Action=CreateStreamingDistributionWithTags:
    get:
      summary: Create Streaming Distribution With Tags
      description: Create a new streaming distribution with tags.
      operationId: createStreamingDistributionWithTags
      x-api-path-slug: actioncreatestreamingdistributionwithtags-get
      parameters:
      - in: query
        name: CreateStreamingDistributionWithTagsRequest
        description: Root level tag for the CreateStreamingDistributionWithTagsRequest
          parameters
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,     and provides an error response
        type: string
      - in: query
        name: StreamingDistributionConfigWithTags
        description: The streaming distributions configuration information
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
      - Distribution
      - Tags
  /?Action=DeleteDistribution:
    get:
      summary: Delete Distribution
      description: Delete a distribution.
      operationId: deleteDistribution
      x-api-path-slug: actiondeletedistribution-get
      parameters:
      - in: query
        name: BgpAsn
        description: For devices that support BGP, the customer gateways BGP ASN
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Id
        description: The distribution ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when you disabled
          the      distribution
        type: string
      - in: query
        name: IpAddress
        description: The Internet-routable IP address for the customer gateways outside
          interface
        type: string
      - in: query
        name: Type
        description: The type of VPN connection that this customer gateway supports
          (ipsec
        type: string
      responses:
        200:
          description: OK
      tags:
      - Distribution
  /?Action=DeleteStreamingDistribution:
    get:
      summary: Delete Streaming Distribution
      description: Delete a streaming distribution.
      operationId: deleteStreamingDistribution
      x-api-path-slug: actiondeletestreamingdistribution-get
      parameters:
      - in: query
        name: CustomerGatewayId
        description: The ID of the customer gateway
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,             and provides an error response
        type: string
      - in: query
        name: Id
        description: The distribution ID
        type: string
      - in: query
        name: If-Match
        description: The value of the ETag header that you received when you disabled
          the      streaming distribution
        type: string
      responses:
        200:
          description: OK
      tags:
      - Streaming
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