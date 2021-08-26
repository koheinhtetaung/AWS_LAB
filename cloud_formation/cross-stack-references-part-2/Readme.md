AWS::EC2::Route 
`RouteTableId` 
`Required: Yes`

Creating a VPC comes with `Main` Routing Table. But [AWS::EC2::VPC](https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-ec2-vpc.html) doesn't return `RouteTableId` vaule according to the documentation.
Reference: [https://stackoverflow.com/questions/55024507/how-can-we-get-a-vpcs-default-route-table-id-using-getattr-in-aws-cloudformat](https://stackoverflow.com/questions/55024507/how-can-we-get-a-vpcs-default-route-table-id-using-getattr-in-aws-cloudformat)