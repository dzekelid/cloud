---
swagger: "2.0"
x-collection-name: AWS CloudFormation
x-complete: 1
info:
  title: AWS CloudFormation API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=DescribeAccountLimits:
    get:
      summary: Describe Account Limits
      description: Retrieves your account's AWS CloudFormation limits, such as the
        maximum number of stacks that you can create in your account.
      operationId: describeAccountLimits
      x-api-path-slug: actiondescribeaccountlimits-get
      parameters:
      - in: query
        name: NextToken
        description: A string that identifies the next page of limits that you want
          to retrieve
        type: string
      responses:
        200:
          description: OK
      tags:
      - Account Limits
  /?Action=DescribeChangeSet:
    get:
      summary: Describe Change Set
      description: Returns the inputs for the change set and a list of changes that
        AWS CloudFormation will make if you execute the change set.
      operationId: describeChangeSet
      x-api-path-slug: actiondescribechangeset-get
      parameters:
      - in: query
        name: ChangeSetName
        description: The name or Amazon Resource Name (ARN) of the change set that
          you want to describe
        type: string
      - in: query
        name: NextToken
        description: A string (provided by the DescribeChangeSet response output)
          that identifies the next page of information that you want to retrieve
        type: string
      - in: query
        name: StackName
        description: If you specified the name of a change set, specify the stack
          name or ID (ARN) of the change set you want to describe
        type: string
      responses:
        200:
          description: OK
      tags:
      - Change Sets
---