# Actions, resources, and condition keys for AWS Performance Insights<a name="list_awsperformanceinsights"></a>

**Tip**  
This page is moving to a new location on November 16, 2020\. Please update your bookmark to use the new page at [https://docs\.aws\.amazon\.com/service\-authorization/latest/reference/list\_awsperformanceinsights\.html](https://docs.aws.amazon.com/service-authorization/latest/reference/list_awsperformanceinsights.html)\. 

AWS Performance Insights \(service prefix: `pi`\) provides the following service\-specific resources, actions, and condition context keys for use in IAM permission policies\.

**Topics**
+ [Actions defined by AWS Performance Insights](#awsperformanceinsights-actions-as-permissions)
+ [Resource types defined by AWS Performance Insights](#awsperformanceinsights-resources-for-iam-policies)
+ [Condition keys for AWS Performance Insights](#awsperformanceinsights-policy-keys)

## Actions defined by AWS Performance Insights<a name="awsperformanceinsights-actions-as-permissions"></a>

You can specify the following actions in the `Action` element of an IAM policy statement\. Use policies to grant permissions to perform an operation in AWS\. When you use an action in a policy, you usually allow or deny access to the API operation or CLI command with the same name\. However, in some cases, a single action controls access to more than one operation\. Alternatively, some operations require several different actions\.

The **Resource types** column indicates whether each action supports resource\-level permissions\. If there is no value for this column, you must specify all resources \("\*"\) in the `Resource` element of your policy statement\. If the column includes a resource type, then you can specify an ARN of that type in a statement with that action\. Required resources are indicated in the table with an asterisk \(\*\)\. If you specify a resource\-level permission ARN in a statement using this action, then it must be of this type\. Some actions support multiple resource types\. If the resource type is optional \(not indicated as required\), then you can choose to use one but not the other\.

For details about the columns in the following table, see [The actions table](reference_policies_actions-resources-contextkeys.md#actions_table)\.


****  

| Actions | Description | Access level | Resource types \(\*required\) | Condition keys | Dependent actions | 
| --- | --- | --- | --- | --- | --- | 
|   DescribeDimensionKeys  | For a specific time period, retrieve the top N dimension keys for a metric\. | Read |   [ metric\-resource\* ](#awsperformanceinsights-metric-resource)   |  |  | 
|   GetResourceMetrics  | Retrieve PI metrics for a set of data sources, over a time period\. | Read |   [ metric\-resource\* ](#awsperformanceinsights-metric-resource)   |  |  | 

## Resource types defined by AWS Performance Insights<a name="awsperformanceinsights-resources-for-iam-policies"></a>

The following resource types are defined by this service and can be used in the `Resource` element of IAM permission policy statements\. Each action in the [Actions table](#awsperformanceinsights-actions-as-permissions) identifies the resource types that can be specified with that action\. A resource type can also define which condition keys you can include in a policy\. These keys are displayed in the last column of the table\. For details about the columns in the following table, see [The resource types table](reference_policies_actions-resources-contextkeys.md#resources_table)\.


****  

| Resource types | ARN | Condition keys | 
| --- | --- | --- | 
|   metric\-resource  |  arn:$\{Partition\}:pi:$\{Region\}:$\{Account\}:metrics/$\{ServiceType\}/$\{Identifier\}  |  | 

## Condition keys for AWS Performance Insights<a name="awsperformanceinsights-policy-keys"></a>

Performance Insights has no service\-specific context keys that can be used in the `Condition` element of policy statements\. For the list of the global context keys that are available to all services, see [Available keys for conditions](reference_policies_condition-keys.html#AvailableKeys)\.