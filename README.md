# cloudformation-newrelic-metricstream
CloudFormation template used for instantiating New Relic Metric Stream integrations

This template configures New Relic IAM Roles, CloudWatch metric stream and Kinesis Data Firehose to send metrics to New Relic with a scalable naming scheme to support multi-account/region scaling via StackSets. 

Note: The NewRelicInfrastrucutre-Integrations role used for Billing will only be deployed in us-east-1 region, so modify as needed if that region is not within scope.

This template is based on the template provided by New Relic, referenced and well documented at the following location:

https://docs.newrelic.com/docs/infrastructure/amazon-integrations/connect/aws-metric-stream-setup/
