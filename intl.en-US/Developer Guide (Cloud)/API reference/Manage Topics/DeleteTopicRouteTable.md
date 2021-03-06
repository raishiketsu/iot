# DeleteTopicRouteTable {#reference_vs2_2jd_xdb .reference}

You can call this operation to cancel topic forwarding for specified topics.

## Request parameters {#section_avh_1l5_xdb .section}

|Name|Type|Required|Description|
|:---|:---|:-------|:----------|
|Action|String|Yes|The operation that you want to perform. Set the value to DeleteTopicRouteTable.|
|SrcTopic|String|Yes|The source topic.|
|DstTopic|List|Yes|The list of target topics for the forwarding relationship that you want to cancel.|

## Response parameters {#section_njn_hl5_xdb .section}

|Name|Type|Description |
|:---|:---|:-----------|
|RequestId|String|The GUID generated by Alibaba Cloud for the request.|
|Success|Boolean|Indicates whether the call is successful. A value of true indicates that the call is successful. A value of false indicates that the call has failed. |
|ErrorMessage|String|The error message returned when the call fails.|
|FailureTopics|List|The list of topics for which the forwarding relationship the system has failed to cancel.|

## Examples {#section_mf5_ll5_xdb .section}

**Request example**

```
https://iot.cn-shanghai.aliyuncs.com/?Action=DeleteTopicRouteTable
&SrcTopic=%2Fx7aWKW94bb8%2FtestDataToDataHub%2Fupdate
&DstTopic.1=%2Fx7aWKW94bb8%2FdeviceNameTest1%2Fadd
&DstTopic.2=%2Fx7aWKW94bb8%2FdeviceNameTest2%2Fdelete
&<Common request parameters>
```

**Response example**

```
{
    "RequestId":"FCC27691-9151-4B93-9622-9C90F30542EC",
    "Success":true,
    "FailureTopics":[]
}
```

