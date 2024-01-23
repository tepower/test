---
title: 高级应用
language_tabs:
  - shell: Shell
  - http: HTTP
  - javascript: JavaScript
  - ruby: Ruby
  - python: Python
  - php: PHP
  - java: Java
  - go: Go
toc_footers: []
includes: []
search: true
code_clipboard: true
highlight_theme: darkula
headingLevel: 2
generator: "@tarslib/widdershins v4.0.20"

---

# 高级应用

Base URLs:

# Authentication

# 外部接口

<a id="opIdqueryRealDataUsingPOST"></a>

## POST 获取 实时数据

POST /zfpt-pdyzz-web/advance/d5000api/getRealDate

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|sensorId|query|string| yes |sensorId|
|addr|query|string| yes |addr|
|token|header|string| no |none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "timestamp": "string",
    "value": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetSensorUsingPOST"></a>

## POST 获取 传感器

POST /zfpt-pdyzz-web/advance/d5000api/getSensor

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|stationId|query|string| yes |stationId|
|sensorType|query|string| yes |sensorType|
|token|header|string| no |none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "assetCode": "string",
      "cityId": 0,
      "cityName": "string",
      "code": "string",
      "createPer": "string",
      "describes": "string",
      "deviceId": 0,
      "deviceTemplateId": 0,
      "deviceTypeId": 0,
      "durationTime": 0,
      "durationTimes": 0,
      "gatewayId": 0,
      "id": 0,
      "manufacturerId": 0,
      "manufacturerNum": "string",
      "monthTime": 0,
      "monthTimes": 0,
      "name": "string",
      "offlineTimes": 0,
      "onlineTime": 0,
      "operationDept": 0,
      "pinYin": "string",
      "pmsId": "string",
      "posX": 0,
      "postion": "string",
      "psrId": "string",
      "remark": "string",
      "samplingFrequency": 0,
      "sensorControType": 0,
      "sensorType": "string",
      "signState": "string",
      "stationId": 0,
      "stationName": "string",
      "synStatus": "string",
      "updatePer": "string",
      "useYears": 0,
      "weekTime": 0,
      "weekTimes": 0,
      "yearTime": 0,
      "yearTimes": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetSensorTestUsingPOST"></a>

## POST 获取 传感器

POST /zfpt-pdyzz-web/advance/d5000api/getSensorTest

### Params

|Name|Location|Type|Required|Description|
|---|---|---|---|---|
|token|header|string| no |none|

> Response Examples

> 200 Response

```json
{
  "property1": {},
  "property2": {}
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

HTTP Status Code **200**

|Name|Type|Required|Restrictions|Title|description|
|---|---|---|---|---|---|
|» **additionalProperties**|object|false|none||none|

<a id="opIdgetStationByNameUsingPOST"></a>

## POST 根据站房名称模糊查询站房名称列表接口

POST /zfpt-pdyzz-web/advance/d5000api/getStationByName

> Body Parameters

```json
{
  "objId": "string",
  "stationName": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[StationQuery](#schemastationquery)| no | StationQuery|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetStationTreeUsingPOST"></a>

## POST 获取 站点树

POST /zfpt-pdyzz-web/advance/d5000api/getStationTree

> Body Parameters

```json
{
  "objId": "string",
  "sxtFlag": true,
  "type": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[ViePom](#schemaviepom)| no | ViePom|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetTreeByStationUsingPOST"></a>

## POST 根据站房ID查询树层级ID列表

POST /zfpt-pdyzz-web/advance/d5000api/getTreeByStation

> Body Parameters

```json
{
  "objId": "string",
  "stationName": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[StationQuery](#schemastationquery)| no | StationQuery|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 评估统计

<a id="opIdsourceLevelUsingPOST"></a>

## POST sourceLevel

POST /zfpt-pdyzz-web/advance/evalHome/sourceLevel

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdstationAvgUsingPOST"></a>

## POST stationAvg

POST /zfpt-pdyzz-web/advance/evalHome/stationAvg

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 设备规则关联表

<a id="opIdaddUsingPOST"></a>

## POST add

POST /zfpt-pdyzz-web/advance/evalStation/add

> Body Parameters

```json
{
  "evalId": 0,
  "evalName": "string",
  "stationId": 0,
  "stationName": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdaddBatchUsingPOST"></a>

## POST addBatch

POST /zfpt-pdyzz-web/advance/evalStation/addBatch

> Body Parameters

```json
[
  {
    "evalId": 0,
    "evalName": "string",
    "stationId": 0,
    "stationName": "string"
  }
]
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|array[any]| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingPOST"></a>

## POST getById

POST /zfpt-pdyzz-web/advance/evalStation/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|string| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdlistUsingPOST"></a>

## POST list

POST /zfpt-pdyzz-web/advance/evalStation/list

> Body Parameters

```json
{
  "evalId": 0,
  "evalName": "string",
  "stationId": 0,
  "stationName": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdremoveUsingPOST"></a>

## POST remove

POST /zfpt-pdyzz-web/advance/evalStation/removes

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST"></a>

## POST update

POST /zfpt-pdyzz-web/advance/evalStation/update

> Body Parameters

```json
{
  "evalId": 0,
  "evalName": "string",
  "stationId": 0,
  "stationName": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 评估

<a id="opIdgetDeviceScoreUsingPOST"></a>

## POST getDeviceScore

POST /zfpt-pdyzz-web/advance/evaluate/getDeviceScore

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|deviceId|query|string| no ||deviceId|
|sFlag|query|string| no ||sFlag|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetStationScoreUsingPOST"></a>

## POST getStationScore

POST /zfpt-pdyzz-web/advance/evaluate/getStationScore

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|stationId|query|string| no ||stationId|
|sFlag|query|string| no ||sFlag|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 评估规则

<a id="opIdApplicationRuleUsingPOST"></a>

## POST ApplicationRule

POST /zfpt-pdyzz-web/advance/evaluationRule/ApplicationRule

> Body Parameters

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdaddUsingPOST_1"></a>

## POST add

POST /zfpt-pdyzz-web/advance/evaluationRule/add

> Body Parameters

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingPOST_1"></a>

## POST getById

POST /zfpt-pdyzz-web/advance/evaluationRule/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|string| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdlistUsingPOST_1"></a>

## POST list

POST /zfpt-pdyzz-web/advance/evaluationRule/list

> Body Parameters

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryPageListUsingPOST"></a>

## POST queryPageList

POST /zfpt-pdyzz-web/advance/evaluationRule/queryPageList

> Body Parameters

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdremoveUsingPOST_1"></a>

## POST remove

POST /zfpt-pdyzz-web/advance/evaluationRule/removes

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_1"></a>

## POST update

POST /zfpt-pdyzz-web/advance/evaluationRule/update

> Body Parameters

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 规则详情

<a id="opIdaddUsingPOST_2"></a>

## POST add

POST /zfpt-pdyzz-web/advance/ruleDetails/add

> Body Parameters

```json
{
  "monitorId": "string",
  "monitorType": "string",
  "name": "string",
  "options": "string",
  "parentId": "string",
  "remark": "string",
  "ruleLeft": "string",
  "ruleRight": "string",
  "source": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdaddBatchUsingPOST_1"></a>

## POST addBatch

POST /zfpt-pdyzz-web/advance/ruleDetails/addBatch

> Body Parameters

```json
[
  {
    "monitorId": "string",
    "monitorType": "string",
    "name": "string",
    "options": "string",
    "parentId": "string",
    "remark": "string",
    "ruleLeft": "string",
    "ruleRight": "string",
    "source": "string",
    "tag": "string",
    "type": "string",
    "weight": "string"
  }
]
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|array[any]| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingPOST_2"></a>

## POST getById

POST /zfpt-pdyzz-web/advance/ruleDetails/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|string| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdlistUsingPOST_2"></a>

## POST list

POST /zfpt-pdyzz-web/advance/ruleDetails/list

> Body Parameters

```json
{
  "monitorId": "string",
  "monitorType": "string",
  "name": "string",
  "options": "string",
  "parentId": "string",
  "remark": "string",
  "ruleLeft": "string",
  "ruleRight": "string",
  "source": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryPageListUsingPOST_1"></a>

## POST queryPageList

POST /zfpt-pdyzz-web/advance/ruleDetails/queryPageList

> Body Parameters

```json
{
  "monitorId": "string",
  "monitorType": "string",
  "name": "string",
  "options": "string",
  "parentId": "string",
  "remark": "string",
  "ruleLeft": "string",
  "ruleRight": "string",
  "source": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdremoveUsingPOST_2"></a>

## POST remove

POST /zfpt-pdyzz-web/advance/ruleDetails/removes

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_2"></a>

## POST update

POST /zfpt-pdyzz-web/advance/ruleDetails/update

> Body Parameters

```json
{
  "monitorId": "string",
  "monitorType": "string",
  "name": "string",
  "options": "string",
  "parentId": "string",
  "remark": "string",
  "ruleLeft": "string",
  "ruleRight": "string",
  "source": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateBatchUsingPOST"></a>

## POST updateBatch

POST /zfpt-pdyzz-web/advance/ruleDetails/updateBatch

> Body Parameters

```json
[
  {
    "monitorId": "string",
    "monitorType": "string",
    "name": "string",
    "options": "string",
    "parentId": "string",
    "remark": "string",
    "ruleLeft": "string",
    "ruleRight": "string",
    "source": "string",
    "tag": "string",
    "type": "string",
    "weight": "string"
  }
]
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|array[any]| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 站房评估

<a id="opIdgetDeviceScoreUsingPOST_1"></a>

## POST getDeviceScore

POST /zfpt-pdyzz-web/advance/score/getDeviceScore

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|deviceId|query|string| no ||deviceId|
|sFlag|query|string| no ||sFlag|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetStationScoreUsingPOST_1"></a>

## POST getStationScore

POST /zfpt-pdyzz-web/advance/score/getStationScore

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|stationId|query|string| no ||stationId|
|sFlag|query|string| no ||sFlag|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 站房评估历史查询

<a id="opIdgetListUsingPOST"></a>

## POST getList

POST /zfpt-pdyzz-web/advance/scoreHst/getList

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "current": 0,
  "endTime": "string",
  "id": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "size": 0,
  "spaceId": "string",
  "spaceName": "string",
  "startTime": "string",
  "status": "string",
  "tableName": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptHstScoreDto](#schematzfpthstscoredto)| no | TZfptHstScoreDto|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetPageUsingPOST"></a>

## POST getPage

POST /zfpt-pdyzz-web/advance/scoreHst/getPage

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "current": 0,
  "endTime": "string",
  "id": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "size": 0,
  "spaceId": "string",
  "spaceName": "string",
  "startTime": "string",
  "status": "string",
  "tableName": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptHstScoreDto](#schematzfpthstscoredto)| no | TZfptHstScoreDto|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 传感器规则

<a id="opIdaddUsingPOST_3"></a>

## POST add

POST /zfpt-pdyzz-web/advance/sensorRule/add

> Body Parameters

```json
{
  "name": "string",
  "optionType": "string",
  "parentId": "string",
  "remark": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdaddBatchUsingPOST_2"></a>

## POST addBatch

POST /zfpt-pdyzz-web/advance/sensorRule/addBatch

> Body Parameters

```json
[
  {
    "name": "string",
    "optionType": "string",
    "parentId": "string",
    "remark": "string",
    "tag": "string",
    "type": "string",
    "weight": "string"
  }
]
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|array[any]| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingPOST_3"></a>

## POST getById

POST /zfpt-pdyzz-web/advance/sensorRule/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|string| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdlistUsingPOST_3"></a>

## POST list

POST /zfpt-pdyzz-web/advance/sensorRule/list

> Body Parameters

```json
{
  "name": "string",
  "optionType": "string",
  "parentId": "string",
  "remark": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryPageListUsingPOST_2"></a>

## POST queryPageList

POST /zfpt-pdyzz-web/advance/sensorRule/queryPageList

> Body Parameters

```json
{
  "name": "string",
  "optionType": "string",
  "parentId": "string",
  "remark": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdremoveUsingPOST_3"></a>

## POST remove

POST /zfpt-pdyzz-web/advance/sensorRule/removes

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_3"></a>

## POST update

POST /zfpt-pdyzz-web/advance/sensorRule/update

> Body Parameters

```json
{
  "name": "string",
  "optionType": "string",
  "parentId": "string",
  "remark": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|any| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateBatchUsingPOST_1"></a>

## POST updateBatch

POST /zfpt-pdyzz-web/advance/sensorRule/updateBatch

> Body Parameters

```json
[
  {
    "name": "string",
    "optionType": "string",
    "parentId": "string",
    "remark": "string",
    "tag": "string",
    "type": "string",
    "weight": "string"
  }
]
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|array[any]| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 一次设备表

<a id="opIdaddUsingPOST_4"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZfptAccountmgDevice/add

> Body Parameters

```json
{
  "assetCode": "string",
  "cityId": 0,
  "cityName": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "describes": "string",
  "deviceCode": "string",
  "deviceId": "string",
  "deviceModelId": "string",
  "deviceName": "string",
  "deviceTemplateId": 0,
  "deviceTypeChildrenid": 0,
  "deviceTypeId": 0,
  "dydj": "string",
  "feederId": "string",
  "id": 0,
  "manufacturerDate": "2019-08-24T14:15:22Z",
  "manufacturerId": "string",
  "manufacturerNum": "string",
  "operationDept": 0,
  "pinYin": "string",
  "pmsId": "string",
  "position": "string",
  "putDate": "2019-08-24T14:15:22Z",
  "ratedCur": "string",
  "ratedVolt": "string",
  "remark": "string",
  "retireDate": "2019-08-24T14:15:22Z",
  "stationId": 0,
  "stationName": "string",
  "takeDate": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "useYears": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgDevice](#schematzfptaccountmgdevice)| no | TZfptAccountmgDevice|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZfptAccountmgDevice/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZfptAccountmgDevice/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "assetCode": "string",
    "cityId": 0,
    "cityName": "string",
    "createPer": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "describes": "string",
    "deviceCode": "string",
    "deviceId": "string",
    "deviceModelId": "string",
    "deviceName": "string",
    "deviceTemplateId": 0,
    "deviceTypeChildrenid": 0,
    "deviceTypeId": 0,
    "dydj": "string",
    "feederId": "string",
    "id": 0,
    "manufacturerDate": "2019-08-24T14:15:22Z",
    "manufacturerId": "string",
    "manufacturerNum": "string",
    "operationDept": 0,
    "pinYin": "string",
    "pmsId": "string",
    "position": "string",
    "putDate": "2019-08-24T14:15:22Z",
    "ratedCur": "string",
    "ratedVolt": "string",
    "remark": "string",
    "retireDate": "2019-08-24T14:15:22Z",
    "stationId": 0,
    "stationName": "string",
    "takeDate": "2019-08-24T14:15:22Z",
    "updatePer": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "useYears": 0
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZfptAccountmgDevice/queryList

> Body Parameters

```json
{
  "assetCode": "string",
  "cityId": 0,
  "cityName": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "describes": "string",
  "deviceCode": "string",
  "deviceId": "string",
  "deviceModelId": "string",
  "deviceName": "string",
  "deviceTemplateId": 0,
  "deviceTypeChildrenid": 0,
  "deviceTypeId": 0,
  "dydj": "string",
  "feederId": "string",
  "id": 0,
  "manufacturerDate": "2019-08-24T14:15:22Z",
  "manufacturerId": "string",
  "manufacturerNum": "string",
  "operationDept": 0,
  "pinYin": "string",
  "pmsId": "string",
  "position": "string",
  "putDate": "2019-08-24T14:15:22Z",
  "ratedCur": "string",
  "ratedVolt": "string",
  "remark": "string",
  "retireDate": "2019-08-24T14:15:22Z",
  "stationId": 0,
  "stationName": "string",
  "takeDate": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "useYears": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgDevice](#schematzfptaccountmgdevice)| no | TZfptAccountmgDevice|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "assetCode": "string",
      "cityId": 0,
      "cityName": "string",
      "createPer": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "describes": "string",
      "deviceCode": "string",
      "deviceId": "string",
      "deviceModelId": "string",
      "deviceName": "string",
      "deviceTemplateId": 0,
      "deviceTypeChildrenid": 0,
      "deviceTypeId": 0,
      "dydj": "string",
      "feederId": "string",
      "id": 0,
      "manufacturerDate": "2019-08-24T14:15:22Z",
      "manufacturerId": "string",
      "manufacturerNum": "string",
      "operationDept": 0,
      "pinYin": "string",
      "pmsId": "string",
      "position": "string",
      "putDate": "2019-08-24T14:15:22Z",
      "ratedCur": "string",
      "ratedVolt": "string",
      "remark": "string",
      "retireDate": "2019-08-24T14:15:22Z",
      "stationId": 0,
      "stationName": "string",
      "takeDate": "2019-08-24T14:15:22Z",
      "updatePer": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "useYears": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_4"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZfptAccountmgDevice/update

> Body Parameters

```json
{
  "assetCode": "string",
  "cityId": 0,
  "cityName": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "describes": "string",
  "deviceCode": "string",
  "deviceId": "string",
  "deviceModelId": "string",
  "deviceName": "string",
  "deviceTemplateId": 0,
  "deviceTypeChildrenid": 0,
  "deviceTypeId": 0,
  "dydj": "string",
  "feederId": "string",
  "id": 0,
  "manufacturerDate": "2019-08-24T14:15:22Z",
  "manufacturerId": "string",
  "manufacturerNum": "string",
  "operationDept": 0,
  "pinYin": "string",
  "pmsId": "string",
  "position": "string",
  "putDate": "2019-08-24T14:15:22Z",
  "ratedCur": "string",
  "ratedVolt": "string",
  "remark": "string",
  "retireDate": "2019-08-24T14:15:22Z",
  "stationId": 0,
  "stationName": "string",
  "takeDate": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "useYears": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgDevice](#schematzfptaccountmgdevice)| no | TZfptAccountmgDevice|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# t-zfpt-accountmg-station-controller

<a id="opIdaddUsingPOST_5"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZfptAccountmgStation/add

> Body Parameters

```json
{
  "acceptancePer": "string",
  "acceptanceResult": 0,
  "acceptanceState": 0,
  "acquisitioningStrategy": 0,
  "areaId": "string",
  "areaIds": "string",
  "areaName": "string",
  "cimUuid": "string",
  "consstructionType": 0,
  "coverArea": 0,
  "createDate": "2019-08-24T14:15:22Z",
  "createFactory": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "gatewayId": 0,
  "gatewaySn": "string",
  "gatewayType": "string",
  "height": 0,
  "inspectionStrategy": 0,
  "isCalled": 0,
  "lastAcceptanceTime": "2019-08-24T14:15:22Z",
  "lastOfflineAcceptanceResult": 0,
  "lat": 0,
  "linkageStrategy": 0,
  "lon": 0,
  "operationDept": "string",
  "operationDepts": "string",
  "phone": 0,
  "pinYin": "string",
  "pinYinShouZiMu": "string",
  "pmsId": "string",
  "remark": "string",
  "rulePer": "string",
  "runState": "string",
  "stationAddr": "string",
  "stationCode": "string",
  "stationId": 0,
  "stationLevel": "string",
  "stationLine": "string",
  "stationLines": "string",
  "stationName": "string",
  "stationType": "string",
  "stationVoltId": 0,
  "svgUuid": "string",
  "thresholdStrategy": 0,
  "topicName": "string",
  "tyrq": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "usUp": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgStation](#schematzfptaccountmgstation)| no | TZfptAccountmgStation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_1"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZfptAccountmgStation/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_1"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZfptAccountmgStation/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "acceptancePer": "string",
    "acceptanceResult": 0,
    "acceptanceState": 0,
    "acquisitioningStrategy": 0,
    "areaId": "string",
    "areaIds": "string",
    "areaName": "string",
    "cimUuid": "string",
    "consstructionType": 0,
    "coverArea": 0,
    "createDate": "2019-08-24T14:15:22Z",
    "createFactory": "string",
    "createPer": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "gatewayId": 0,
    "gatewaySn": "string",
    "gatewayType": "string",
    "height": 0,
    "inspectionStrategy": 0,
    "isCalled": 0,
    "lastAcceptanceTime": "2019-08-24T14:15:22Z",
    "lastOfflineAcceptanceResult": 0,
    "lat": 0,
    "linkageStrategy": 0,
    "lon": 0,
    "operationDept": "string",
    "operationDepts": "string",
    "phone": 0,
    "pinYin": "string",
    "pinYinShouZiMu": "string",
    "pmsId": "string",
    "remark": "string",
    "rulePer": "string",
    "runState": "string",
    "stationAddr": "string",
    "stationCode": "string",
    "stationId": 0,
    "stationLevel": "string",
    "stationLine": "string",
    "stationLines": "string",
    "stationName": "string",
    "stationType": "string",
    "stationVoltId": 0,
    "svgUuid": "string",
    "thresholdStrategy": 0,
    "topicName": "string",
    "tyrq": "2019-08-24T14:15:22Z",
    "updatePer": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "usUp": 0
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_1"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZfptAccountmgStation/queryList

> Body Parameters

```json
{
  "acceptancePer": "string",
  "acceptanceResult": 0,
  "acceptanceState": 0,
  "acquisitioningStrategy": 0,
  "areaId": "string",
  "areaIds": "string",
  "areaName": "string",
  "cimUuid": "string",
  "consstructionType": 0,
  "coverArea": 0,
  "createDate": "2019-08-24T14:15:22Z",
  "createFactory": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "gatewayId": 0,
  "gatewaySn": "string",
  "gatewayType": "string",
  "height": 0,
  "inspectionStrategy": 0,
  "isCalled": 0,
  "lastAcceptanceTime": "2019-08-24T14:15:22Z",
  "lastOfflineAcceptanceResult": 0,
  "lat": 0,
  "linkageStrategy": 0,
  "lon": 0,
  "operationDept": "string",
  "operationDepts": "string",
  "phone": 0,
  "pinYin": "string",
  "pinYinShouZiMu": "string",
  "pmsId": "string",
  "remark": "string",
  "rulePer": "string",
  "runState": "string",
  "stationAddr": "string",
  "stationCode": "string",
  "stationId": 0,
  "stationLevel": "string",
  "stationLine": "string",
  "stationLines": "string",
  "stationName": "string",
  "stationType": "string",
  "stationVoltId": 0,
  "svgUuid": "string",
  "thresholdStrategy": 0,
  "topicName": "string",
  "tyrq": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "usUp": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgStation](#schematzfptaccountmgstation)| no | TZfptAccountmgStation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "acceptancePer": "string",
      "acceptanceResult": 0,
      "acceptanceState": 0,
      "acquisitioningStrategy": 0,
      "areaId": "string",
      "areaIds": "string",
      "areaName": "string",
      "cimUuid": "string",
      "consstructionType": 0,
      "coverArea": 0,
      "createDate": "2019-08-24T14:15:22Z",
      "createFactory": "string",
      "createPer": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "gatewayId": 0,
      "gatewaySn": "string",
      "gatewayType": "string",
      "height": 0,
      "inspectionStrategy": 0,
      "isCalled": 0,
      "lastAcceptanceTime": "2019-08-24T14:15:22Z",
      "lastOfflineAcceptanceResult": 0,
      "lat": 0,
      "linkageStrategy": 0,
      "lon": 0,
      "operationDept": "string",
      "operationDepts": "string",
      "phone": 0,
      "pinYin": "string",
      "pinYinShouZiMu": "string",
      "pmsId": "string",
      "remark": "string",
      "rulePer": "string",
      "runState": "string",
      "stationAddr": "string",
      "stationCode": "string",
      "stationId": 0,
      "stationLevel": "string",
      "stationLine": "string",
      "stationLines": "string",
      "stationName": "string",
      "stationType": "string",
      "stationVoltId": 0,
      "svgUuid": "string",
      "thresholdStrategy": 0,
      "topicName": "string",
      "tyrq": "2019-08-24T14:15:22Z",
      "updatePer": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "usUp": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_5"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZfptAccountmgStation/update

> Body Parameters

```json
{
  "acceptancePer": "string",
  "acceptanceResult": 0,
  "acceptanceState": 0,
  "acquisitioningStrategy": 0,
  "areaId": "string",
  "areaIds": "string",
  "areaName": "string",
  "cimUuid": "string",
  "consstructionType": 0,
  "coverArea": 0,
  "createDate": "2019-08-24T14:15:22Z",
  "createFactory": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "gatewayId": 0,
  "gatewaySn": "string",
  "gatewayType": "string",
  "height": 0,
  "inspectionStrategy": 0,
  "isCalled": 0,
  "lastAcceptanceTime": "2019-08-24T14:15:22Z",
  "lastOfflineAcceptanceResult": 0,
  "lat": 0,
  "linkageStrategy": 0,
  "lon": 0,
  "operationDept": "string",
  "operationDepts": "string",
  "phone": 0,
  "pinYin": "string",
  "pinYinShouZiMu": "string",
  "pmsId": "string",
  "remark": "string",
  "rulePer": "string",
  "runState": "string",
  "stationAddr": "string",
  "stationCode": "string",
  "stationId": 0,
  "stationLevel": "string",
  "stationLine": "string",
  "stationLines": "string",
  "stationName": "string",
  "stationType": "string",
  "stationVoltId": 0,
  "svgUuid": "string",
  "thresholdStrategy": 0,
  "topicName": "string",
  "tyrq": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "usUp": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAccountmgStation](#schematzfptaccountmgstation)| no | TZfptAccountmgStation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# t-zfpt-alarm-controller

<a id="opIdaddUsingPOST_6"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZfptAlarm/add

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdalarmStatUsingPOST"></a>

## POST alarmStat

POST /zfpt-pdyzz-web/advance/tZfptAlarm/alarmStat

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_2"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZfptAlarm/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_2"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZfptAlarm/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "alarmLastTime": "2019-08-24T14:15:22Z",
    "alarmLevel": "string",
    "alarmNum": 0,
    "alarmSource": "string",
    "alarmState": "string",
    "alarmType": "string",
    "areaId": 0,
    "columnId": 0,
    "confirmStatus": 0,
    "continued": 0,
    "current": 0,
    "dataTime": "string",
    "deviceId": 0,
    "deviceName": "string",
    "deviceType": "string",
    "deviceTypeList": [
      "string"
    ],
    "endTime": "string",
    "evtConfirmRemarks": "string",
    "id": 0,
    "imageUuid": "string",
    "iotId": "string",
    "method": "string",
    "pageNum": 0,
    "pointId": 0,
    "remarks": "string",
    "returnTime": "2019-08-24T14:15:22Z",
    "size": 0,
    "startTime": "string",
    "stationId": 0,
    "stationName": "string",
    "tableName": "string",
    "threshold": "string",
    "timestamp": "2019-08-24T14:15:22Z",
    "value": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryCntListUsingPOST"></a>

## POST queryCntList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryCntList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "deviceType": "string",
      "deviceTypeName": "string",
      "endTime": "2019-08-24T14:15:22Z",
      "imageUuid": "string",
      "method": "string",
      "methodName": "string",
      "remarks": "string",
      "startTime": "2019-08-24T14:15:22Z",
      "stationId": 0,
      "stationName": "string",
      "timestamp": "2019-08-24T14:15:22Z"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryCntPageListUsingPOST"></a>

## POST queryCntPageList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryCntPageList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryDtoListUsingPOST"></a>

## POST queryDtoList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryDtoList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "deviceType": "string",
      "deviceTypeName": "string",
      "endTime": "2019-08-24T14:15:22Z",
      "imageUuid": "string",
      "method": "string",
      "methodName": "string",
      "remarks": "string",
      "startTime": "2019-08-24T14:15:22Z",
      "stationId": 0,
      "stationName": "string",
      "timestamp": "2019-08-24T14:15:22Z"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryDtoPageListUsingPOST"></a>

## POST queryDtoPageList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryDtoPageList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_2"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "alarmSource": "string",
      "alarmState": "string",
      "alarmType": "string",
      "areaId": 0,
      "columnId": 0,
      "confirmStatus": 0,
      "continued": 0,
      "current": 0,
      "dataTime": "string",
      "deviceId": 0,
      "deviceName": "string",
      "deviceType": "string",
      "deviceTypeList": [
        "string"
      ],
      "endTime": "string",
      "evtConfirmRemarks": "string",
      "id": 0,
      "imageUuid": "string",
      "iotId": "string",
      "method": "string",
      "pageNum": 0,
      "pointId": 0,
      "remarks": "string",
      "returnTime": "2019-08-24T14:15:22Z",
      "size": 0,
      "startTime": "string",
      "stationId": 0,
      "stationName": "string",
      "tableName": "string",
      "threshold": "string",
      "timestamp": "2019-08-24T14:15:22Z",
      "value": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryPageListUsingPOST_3"></a>

## POST queryPageList

POST /zfpt-pdyzz-web/advance/tZfptAlarm/queryPageList

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "alarmSource": "string",
      "alarmState": "string",
      "alarmType": "string",
      "areaId": 0,
      "columnId": 0,
      "confirmStatus": 0,
      "continued": 0,
      "current": 0,
      "dataTime": "string",
      "deviceId": 0,
      "deviceName": "string",
      "deviceType": "string",
      "deviceTypeList": [
        "string"
      ],
      "endTime": "string",
      "evtConfirmRemarks": "string",
      "id": 0,
      "imageUuid": "string",
      "iotId": "string",
      "method": "string",
      "pageNum": 0,
      "pointId": 0,
      "remarks": "string",
      "returnTime": "2019-08-24T14:15:22Z",
      "size": 0,
      "startTime": "string",
      "stationId": 0,
      "stationName": "string",
      "tableName": "string",
      "threshold": "string",
      "timestamp": "2019-08-24T14:15:22Z",
      "value": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_6"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZfptAlarm/update

> Body Parameters

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptAlarm](#schematzfptalarm)| no | TZfptAlarm|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# 二次设备与测点关联表

<a id="opIdaddUsingPOST_7"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZfptSensorPointRelation/add

> Body Parameters

```json
{
  "deviceType": "string",
  "dictionaryCode": "string",
  "dictionaryId": 0,
  "dictionaryName": "string",
  "id": 0,
  "paramDef": "string",
  "psrType": "string",
  "tagType": 0,
  "tagTypes": [
    0
  ],
  "unit": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSensorPointRelation](#schematzfptsensorpointrelation)| no | TZfptSensorPointRelation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_3"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZfptSensorPointRelation/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_3"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZfptSensorPointRelation/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "deviceType": "string",
    "dictionaryCode": "string",
    "dictionaryId": 0,
    "dictionaryName": "string",
    "id": 0,
    "paramDef": "string",
    "psrType": "string",
    "tagType": 0,
    "tagTypes": [
      0
    ],
    "unit": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_3"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZfptSensorPointRelation/queryList

> Body Parameters

```json
{
  "deviceType": "string",
  "dictionaryCode": "string",
  "dictionaryId": 0,
  "dictionaryName": "string",
  "id": 0,
  "paramDef": "string",
  "psrType": "string",
  "tagType": 0,
  "tagTypes": [
    0
  ],
  "unit": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSensorPointRelation](#schematzfptsensorpointrelation)| no | TZfptSensorPointRelation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_7"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZfptSensorPointRelation/update

> Body Parameters

```json
{
  "deviceType": "string",
  "dictionaryCode": "string",
  "dictionaryId": 0,
  "dictionaryName": "string",
  "id": 0,
  "paramDef": "string",
  "psrType": "string",
  "tagType": 0,
  "tagTypes": [
    0
  ],
  "unit": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSensorPointRelation](#schematzfptsensorpointrelation)| no | TZfptSensorPointRelation|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# code表

<a id="opIdaddUsingPOST_8"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZfptSysCode/add

> Body Parameters

```json
{
  "children": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "code": "string",
  "createBy": 0,
  "createTime": "2019-08-24T14:15:22Z",
  "id": 0,
  "isUse": 0,
  "names": "string",
  "orderNum": 0,
  "parentId": 0,
  "remarks": "string",
  "updateBy": 0,
  "updateTime": "2019-08-24T14:15:22Z",
  "yaoce": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "yaoxin": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ]
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSysCode](#schematzfptsyscode)| no | TZfptSysCode|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdcodeTreeUsingPOST"></a>

## POST codeTree

POST /zfpt-pdyzz-web/advance/tZfptSysCode/codeTree

> Body Parameters

```json
{
  "children": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "code": "string",
  "createBy": 0,
  "createTime": "2019-08-24T14:15:22Z",
  "id": 0,
  "isUse": 0,
  "names": "string",
  "orderNum": 0,
  "parentId": 0,
  "remarks": "string",
  "updateBy": 0,
  "updateTime": "2019-08-24T14:15:22Z",
  "yaoce": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "yaoxin": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ]
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSysCode](#schematzfptsyscode)| no | TZfptSysCode|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "children": [
        {
          "children": [],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {
              "deviceType": "string",
              "dictionaryCode": "string",
              "dictionaryId": 0,
              "dictionaryName": "string",
              "id": 0,
              "paramDef": "string",
              "psrType": "string",
              "tagType": 0,
              "tagTypes": [
                0
              ],
              "unit": "string"
            }
          ],
          "yaoxin": [
            {
              "deviceType": "string",
              "dictionaryCode": "string",
              "dictionaryId": 0,
              "dictionaryName": "string",
              "id": 0,
              "paramDef": "string",
              "psrType": "string",
              "tagType": 0,
              "tagTypes": [
                0
              ],
              "unit": "string"
            }
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_4"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZfptSysCode/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetAllPointUsingGET"></a>

## GET 获取 所有设备类型  和 遥测遥信点

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getAllPoint

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_4"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "children": [
      {
        "children": [],
        "code": "string",
        "createBy": 0,
        "createTime": "2019-08-24T14:15:22Z",
        "id": 0,
        "isUse": 0,
        "names": "string",
        "orderNum": 0,
        "parentId": 0,
        "remarks": "string",
        "updateBy": 0,
        "updateTime": "2019-08-24T14:15:22Z",
        "yaoce": [
          {
            "deviceType": "string",
            "dictionaryCode": "string",
            "dictionaryId": 0,
            "dictionaryName": "string",
            "id": 0,
            "paramDef": "string",
            "psrType": "string",
            "tagType": 0,
            "tagTypes": [
              0
            ],
            "unit": "string"
          }
        ],
        "yaoxin": [
          {
            "deviceType": "string",
            "dictionaryCode": "string",
            "dictionaryId": 0,
            "dictionaryName": "string",
            "id": 0,
            "paramDef": "string",
            "psrType": "string",
            "tagType": 0,
            "tagTypes": [
              0
            ],
            "unit": "string"
          }
        ]
      }
    ],
    "code": "string",
    "createBy": 0,
    "createTime": "2019-08-24T14:15:22Z",
    "id": 0,
    "isUse": 0,
    "names": "string",
    "orderNum": 0,
    "parentId": 0,
    "remarks": "string",
    "updateBy": 0,
    "updateTime": "2019-08-24T14:15:22Z",
    "yaoce": [
      {
        "deviceType": "string",
        "dictionaryCode": "string",
        "dictionaryId": 0,
        "dictionaryName": "string",
        "id": 0,
        "paramDef": "string",
        "psrType": "string",
        "tagType": 0,
        "tagTypes": [
          0
        ],
        "unit": "string"
      }
    ],
    "yaoxin": [
      {
        "deviceType": "string",
        "dictionaryCode": "string",
        "dictionaryId": 0,
        "dictionaryName": "string",
        "id": 0,
        "paramDef": "string",
        "psrType": "string",
        "tagType": 0,
        "tagTypes": [
          0
        ],
        "unit": "string"
      }
    ]
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetDeviceTypeUsingGET"></a>

## GET 获取 所有一次设备类型

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getDeviceType

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetEventTypeUsingGET"></a>

## GET 获取所有事件类型

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getEventType

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetFaultTypeUsingGET"></a>

## GET 获取所有故障类型

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getFaultType

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetStationTypeUsingGET"></a>

## GET 获取 所有站房类型

GET /zfpt-pdyzz-web/advance/tZfptSysCode/getStationType

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_4"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZfptSysCode/queryList

> Body Parameters

```json
{
  "children": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "code": "string",
  "createBy": 0,
  "createTime": "2019-08-24T14:15:22Z",
  "id": 0,
  "isUse": 0,
  "names": "string",
  "orderNum": 0,
  "parentId": 0,
  "remarks": "string",
  "updateBy": 0,
  "updateTime": "2019-08-24T14:15:22Z",
  "yaoce": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "yaoxin": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ]
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSysCode](#schematzfptsyscode)| no | TZfptSysCode|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "children": [
        {
          "children": [],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {
              "deviceType": "string",
              "dictionaryCode": "string",
              "dictionaryId": 0,
              "dictionaryName": "string",
              "id": 0,
              "paramDef": "string",
              "psrType": "string",
              "tagType": 0,
              "tagTypes": [
                0
              ],
              "unit": "string"
            }
          ],
          "yaoxin": [
            {
              "deviceType": "string",
              "dictionaryCode": "string",
              "dictionaryId": 0,
              "dictionaryName": "string",
              "id": 0,
              "paramDef": "string",
              "psrType": "string",
              "tagType": 0,
              "tagTypes": [
                0
              ],
              "unit": "string"
            }
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_8"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZfptSysCode/update

> Body Parameters

```json
{
  "children": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "code": "string",
  "createBy": 0,
  "createTime": "2019-08-24T14:15:22Z",
  "id": 0,
  "isUse": 0,
  "names": "string",
  "orderNum": 0,
  "parentId": 0,
  "remarks": "string",
  "updateBy": 0,
  "updateTime": "2019-08-24T14:15:22Z",
  "yaoce": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "yaoxin": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ]
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZfptSysCode](#schematzfptsyscode)| no | TZfptSysCode|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# realScore

<a id="opIdaddUsingPOST_9"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZrRealScore/add

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "id": "string",
  "orderBy": "string",
  "pubKey": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "spaceId": "string",
  "spaceIds": [
    "string"
  ],
  "spaceName": "string",
  "stationType": "string",
  "status": 0,
  "type": "string",
  "updateTime": "2019-08-24T14:15:22Z"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrRealScore](#schematzrrealscore)| no | TZrRealScore|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_5"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZrRealScore/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_5"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZrRealScore/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "createBy": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "id": "string",
    "orderBy": "string",
    "pubKey": "string",
    "score": "string",
    "scoreItemDetail": "string",
    "spaceId": "string",
    "spaceIds": [
      "string"
    ],
    "spaceName": "string",
    "stationType": "string",
    "status": 0,
    "type": "string",
    "updateTime": "2019-08-24T14:15:22Z"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetPageUsingPOST_1"></a>

## POST getPage

POST /zfpt-pdyzz-web/advance/tZrRealScore/getPage

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "id": "string",
  "orderBy": "string",
  "pubKey": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "spaceId": "string",
  "spaceIds": [
    "string"
  ],
  "spaceName": "string",
  "stationType": "string",
  "status": 0,
  "type": "string",
  "updateTime": "2019-08-24T14:15:22Z"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrRealScore](#schematzrrealscore)| no | TZrRealScore|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_5"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZrRealScore/queryList

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "id": "string",
  "orderBy": "string",
  "pubKey": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "spaceId": "string",
  "spaceIds": [
    "string"
  ],
  "spaceName": "string",
  "stationType": "string",
  "status": 0,
  "type": "string",
  "updateTime": "2019-08-24T14:15:22Z"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrRealScore](#schematzrrealscore)| no | TZrRealScore|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "id": "string",
      "orderBy": "string",
      "pubKey": "string",
      "score": "string",
      "scoreItemDetail": "string",
      "spaceId": "string",
      "spaceIds": [
        "string"
      ],
      "spaceName": "string",
      "stationType": "string",
      "status": 0,
      "type": "string",
      "updateTime": "2019-08-24T14:15:22Z"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_9"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZrRealScore/update

> Body Parameters

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "id": "string",
  "orderBy": "string",
  "pubKey": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "spaceId": "string",
  "spaceIds": [
    "string"
  ],
  "spaceName": "string",
  "stationType": "string",
  "status": 0,
  "type": "string",
  "updateTime": "2019-08-24T14:15:22Z"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrRealScore](#schematzrrealscore)| no | TZrRealScore|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# t-zr-score-item-controller

<a id="opIdaddUsingPOST_10"></a>

## POST add

POST /zfpt-pdyzz-web/advance/tZrScoreItem/add

> Body Parameters

```json
{
  "addr": "string",
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "desc": "string",
  "id": 0,
  "isEnv": 0,
  "koufen": "string",
  "name": "string",
  "ownerId": "string",
  "plugin": "string",
  "remark": "string",
  "root": "string",
  "sensorType": "string",
  "stationId": "string",
  "status": 0,
  "tag": "string",
  "tagType": "string",
  "type": "string",
  "updateBy": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "url": "string",
  "yuzhileft": "string",
  "yuzhiright": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrScoreItem](#schematzrscoreitem)| no | TZrScoreItem|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdaddsUsingPOST"></a>

## POST adds

POST /zfpt-pdyzz-web/advance/tZrScoreItem/adds

> Body Parameters

```json
{
  "plugin": "string",
  "rule": [
    {
      "addr": "string",
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "desc": "string",
      "id": 0,
      "isEnv": 0,
      "koufen": "string",
      "name": "string",
      "ownerId": "string",
      "plugin": "string",
      "remark": "string",
      "root": "string",
      "sensorType": "string",
      "stationId": "string",
      "status": 0,
      "tag": "string",
      "tagType": "string",
      "type": "string",
      "updateBy": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "url": "string",
      "yuzhileft": "string",
      "yuzhiright": "string"
    }
  ],
  "stationId": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrScoreItemAddsDto](#schematzrscoreitemaddsdto)| no | TZrScoreItemAddsDto|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIddeleteUsingPOST_6"></a>

## POST delete

POST /zfpt-pdyzz-web/advance/tZrScoreItem/delete

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|ids|query|string| yes ||ids|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdgetByIdUsingGET_6"></a>

## GET getById

GET /zfpt-pdyzz-web/advance/tZrScoreItem/getById/{id}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|id|path|integer| yes ||id|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {
    "addr": "string",
    "createBy": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "desc": "string",
    "id": 0,
    "isEnv": 0,
    "koufen": "string",
    "name": "string",
    "ownerId": "string",
    "plugin": "string",
    "remark": "string",
    "root": "string",
    "sensorType": "string",
    "stationId": "string",
    "status": 0,
    "tag": "string",
    "tagType": "string",
    "type": "string",
    "updateBy": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "url": "string",
    "yuzhileft": "string",
    "yuzhiright": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListUsingPOST_6"></a>

## POST queryList

POST /zfpt-pdyzz-web/advance/tZrScoreItem/queryList

> Body Parameters

```json
{
  "addr": "string",
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "desc": "string",
  "id": 0,
  "isEnv": 0,
  "koufen": "string",
  "name": "string",
  "ownerId": "string",
  "plugin": "string",
  "remark": "string",
  "root": "string",
  "sensorType": "string",
  "stationId": "string",
  "status": 0,
  "tag": "string",
  "tagType": "string",
  "type": "string",
  "updateBy": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "url": "string",
  "yuzhileft": "string",
  "yuzhiright": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrScoreItem](#schematzrscoreitem)| no | TZrScoreItem|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "addr": "string",
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "desc": "string",
      "id": 0,
      "isEnv": 0,
      "koufen": "string",
      "name": "string",
      "ownerId": "string",
      "plugin": "string",
      "remark": "string",
      "root": "string",
      "sensorType": "string",
      "stationId": "string",
      "status": 0,
      "tag": "string",
      "tagType": "string",
      "type": "string",
      "updateBy": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "url": "string",
      "yuzhileft": "string",
      "yuzhiright": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListInUseUsingPOST"></a>

## POST queryListInUse

POST /zfpt-pdyzz-web/advance/tZrScoreItem/queryListInUse

> Body Parameters

```json
{
  "addr": "string",
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "desc": "string",
  "id": 0,
  "isEnv": 0,
  "koufen": "string",
  "name": "string",
  "ownerId": "string",
  "plugin": "string",
  "remark": "string",
  "root": "string",
  "sensorType": "string",
  "stationId": "string",
  "status": 0,
  "tag": "string",
  "tagType": "string",
  "type": "string",
  "updateBy": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "url": "string",
  "yuzhileft": "string",
  "yuzhiright": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrScoreItem](#schematzrscoreitem)| no | TZrScoreItem|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": [
    {
      "addr": "string",
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "desc": "string",
      "id": 0,
      "isEnv": 0,
      "koufen": "string",
      "name": "string",
      "ownerId": "string",
      "plugin": "string",
      "remark": "string",
      "root": "string",
      "sensorType": "string",
      "stationId": "string",
      "status": 0,
      "tag": "string",
      "tagType": "string",
      "type": "string",
      "updateBy": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "url": "string",
      "yuzhileft": "string",
      "yuzhiright": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryStationTypeByStationIdUsingGET"></a>

## GET queryStationTypeByStationId

GET /zfpt-pdyzz-web/advance/tZrScoreItem/queryStationTypeByStationId/{stationId}

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|stationId|path|string| yes ||stationId|
|token|header|string| no ||none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdqueryListSepConUsingPOST"></a>

## POST queryListSepCon

POST /zfpt-pdyzz-web/advance/tZrScoreItem/sepCon/queryList

> Body Parameters

```json
{
  "current": 0,
  "pageNum": 0,
  "size": 0
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[SepConQuery](#schemasepconquery)| no | SepConQuery|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|[Result](#schemaresult)|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

<a id="opIdupdateUsingPOST_10"></a>

## POST update

POST /zfpt-pdyzz-web/advance/tZrScoreItem/update

> Body Parameters

```json
{
  "addr": "string",
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "desc": "string",
  "id": 0,
  "isEnv": 0,
  "koufen": "string",
  "name": "string",
  "ownerId": "string",
  "plugin": "string",
  "remark": "string",
  "root": "string",
  "sensorType": "string",
  "stationId": "string",
  "status": 0,
  "tag": "string",
  "tagType": "string",
  "type": "string",
  "updateBy": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "url": "string",
  "yuzhileft": "string",
  "yuzhiright": "string"
}
```

### Params

|Name|Location|Type|Required|Title|Description|
|---|---|---|---|---|---|
|token|header|string| no ||none|
|body|body|[TZrScoreItem](#schematzrscoreitem)| no | TZrScoreItem|none|

> Response Examples

> 200 Response

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}
```

### Responses

|HTTP Status Code |Meaning|Description|Data schema|
|---|---|---|---|
|200|[OK](https://tools.ietf.org/html/rfc7231#section-6.3.1)|OK|Inline|
|201|[Created](https://tools.ietf.org/html/rfc7231#section-6.3.2)|Created|Inline|
|401|[Unauthorized](https://tools.ietf.org/html/rfc7235#section-3.1)|Unauthorized|Inline|
|403|[Forbidden](https://tools.ietf.org/html/rfc7231#section-6.5.3)|Forbidden|Inline|
|404|[Not Found](https://tools.ietf.org/html/rfc7231#section-6.5.4)|Not Found|Inline|

### Responses Data Schema

# Data Schema

<h2 id="tocS_评估规则">评估规则</h2>

<a id="schema评估规则"></a>
<a id="schema_评估规则"></a>
<a id="tocS评估规则"></a>
<a id="tocs评估规则"></a>

```json
{
  "name": "string",
  "remark": "string",
  "status": "string",
  "type": "string"
}

```

评估规则

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|name|string|false|none||配置名称|
|remark|string|false|none||备注|
|status|string|false|none||是否启用 0:停用  1:启用|
|type|string|false|none||配置类型|

<h2 id="tocS_规则详情">规则详情</h2>

<a id="schema规则详情"></a>
<a id="schema_规则详情"></a>
<a id="tocS规则详情"></a>
<a id="tocs规则详情"></a>

```json
{
  "monitorId": "string",
  "monitorType": "string",
  "name": "string",
  "options": "string",
  "parentId": "string",
  "remark": "string",
  "ruleLeft": "string",
  "ruleRight": "string",
  "source": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}

```

规则详情

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|monitorId|string|false|none||测点ID|
|monitorType|string|false|none||监测类型|
|name|string|false|none||名称|
|options|string|false|none||方案|
|parentId|string|false|none||传感器规则ID|
|remark|string|false|none||备注|
|ruleLeft|string|false|none||规则|
|ruleRight|string|false|none||规则|
|source|string|false|none||扣分|
|tag|string|false|none||标签|
|type|string|false|none||传感器类型|
|weight|string|false|none||权重|

<h2 id="tocS_规则设备关联表">规则设备关联表</h2>

<a id="schema规则设备关联表"></a>
<a id="schema_规则设备关联表"></a>
<a id="tocS规则设备关联表"></a>
<a id="tocs规则设备关联表"></a>

```json
{
  "evalId": 0,
  "evalName": "string",
  "stationId": 0,
  "stationName": "string"
}

```

规则设备关联表

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|evalId|integer(int64)|false|none||规则表ID|
|evalName|string|false|none||规则名称|
|stationId|integer(int64)|false|none||设备ID|
|stationName|string|false|none||设备名称|

<h2 id="tocS_传感器规则">传感器规则</h2>

<a id="schema传感器规则"></a>
<a id="schema_传感器规则"></a>
<a id="tocS传感器规则"></a>
<a id="tocs传感器规则"></a>

```json
{
  "name": "string",
  "optionType": "string",
  "parentId": "string",
  "remark": "string",
  "tag": "string",
  "type": "string",
  "weight": "string"
}

```

传感器规则

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|name|string|false|none||传感器名称|
|optionType|string|false|none||方案类型|
|parentId|string|false|none||评估规则ID|
|remark|string|false|none||备注|
|tag|string|false|none||标签|
|type|string|false|none||传感器类型|
|weight|string|false|none||权重|

<h2 id="tocS_ViePom">ViePom</h2>

<a id="schemaviepom"></a>
<a id="schema_ViePom"></a>
<a id="tocSviepom"></a>
<a id="tocsviepom"></a>

```json
{
  "objId": "string",
  "sxtFlag": true,
  "type": 0
}

```

ViePom

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|objId|string|false|none||none|
|sxtFlag|boolean|false|none||none|
|type|integer(int32)|false|none||none|

<h2 id="tocS_TZrScoreItemAddsDto">TZrScoreItemAddsDto</h2>

<a id="schematzrscoreitemaddsdto"></a>
<a id="schema_TZrScoreItemAddsDto"></a>
<a id="tocStzrscoreitemaddsdto"></a>
<a id="tocstzrscoreitemaddsdto"></a>

```json
{
  "plugin": "string",
  "rule": [
    {
      "addr": "string",
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "desc": "string",
      "id": 0,
      "isEnv": 0,
      "koufen": "string",
      "name": "string",
      "ownerId": "string",
      "plugin": "string",
      "remark": "string",
      "root": "string",
      "sensorType": "string",
      "stationId": "string",
      "status": 0,
      "tag": "string",
      "tagType": "string",
      "type": "string",
      "updateBy": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "url": "string",
      "yuzhileft": "string",
      "yuzhiright": "string"
    }
  ],
  "stationId": "string"
}

```

TZrScoreItemAddsDto

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|plugin|string|false|none||none|
|rule|[[TZrScoreItem](#schematzrscoreitem)]|false|none||none|
|stationId|string|false|none||none|

<h2 id="tocS_TZrScoreItem">TZrScoreItem</h2>

<a id="schematzrscoreitem"></a>
<a id="schema_TZrScoreItem"></a>
<a id="tocStzrscoreitem"></a>
<a id="tocstzrscoreitem"></a>

```json
{
  "addr": "string",
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "desc": "string",
  "id": 0,
  "isEnv": 0,
  "koufen": "string",
  "name": "string",
  "ownerId": "string",
  "plugin": "string",
  "remark": "string",
  "root": "string",
  "sensorType": "string",
  "stationId": "string",
  "status": 0,
  "tag": "string",
  "tagType": "string",
  "type": "string",
  "updateBy": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "url": "string",
  "yuzhileft": "string",
  "yuzhiright": "string"
}

```

TZrScoreItem

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|addr|string|false|none||none|
|createBy|string|false|none||none|
|createTime|string(date-time)|false|none||none|
|desc|string|false|none||none|
|id|integer(int64)|false|none||主见|
|isEnv|integer(int32)|false|none||是否是环境类 默认是|
|koufen|string|false|none||越限扣分 逗号分割|
|name|string|false|none||描述|
|ownerId|string|false|none||none|
|plugin|string|false|none||一次设备类型|
|remark|string|false|none||none|
|root|string|false|none||权重|
|sensorType|string|false|none||none|
|stationId|string|false|none||站点id|
|status|integer(int32)|false|none||状态，是否启动|
|tag|string|false|none||监测类型（同一类型的不同tag 可以逗号分割）|
|tagType|string|false|none||标签类型 遥信或者遥测|
|type|string|false|none||none|
|updateBy|string|false|none||none|
|updateTime|string(date-time)|false|none||none|
|url|string|false|none||none|
|yuzhileft|string|false|none||大于等于逗号分割|
|yuzhiright|string|false|none||小于逗号分割|

<h2 id="tocS_TZrRealScore">TZrRealScore</h2>

<a id="schematzrrealscore"></a>
<a id="schema_TZrRealScore"></a>
<a id="tocStzrrealscore"></a>
<a id="tocstzrrealscore"></a>

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "id": "string",
  "orderBy": "string",
  "pubKey": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "spaceId": "string",
  "spaceIds": [
    "string"
  ],
  "spaceName": "string",
  "stationType": "string",
  "status": 0,
  "type": "string",
  "updateTime": "2019-08-24T14:15:22Z"
}

```

TZrRealScore

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|createBy|string|false|none||none|
|createTime|string(date-time)|false|none||none|
|id|string|false|none||none|
|orderBy|string|false|none||none|
|pubKey|string|false|none||none|
|score|string|false|none||none|
|scoreItemDetail|string|false|none||none|
|spaceId|string|false|none||none|
|spaceIds|[string]|false|none||none|
|spaceName|string|false|none||none|
|stationType|string|false|none||none|
|status|integer(int32)|false|none||none|
|type|string|false|none||none|
|updateTime|string(date-time)|false|none||none|

<h2 id="tocS_TZfptSysCode">TZfptSysCode</h2>

<a id="schematzfptsyscode"></a>
<a id="schema_TZfptSysCode"></a>
<a id="tocStzfptsyscode"></a>
<a id="tocstzfptsyscode"></a>

```json
{
  "children": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "code": "string",
  "createBy": 0,
  "createTime": "2019-08-24T14:15:22Z",
  "id": 0,
  "isUse": 0,
  "names": "string",
  "orderNum": 0,
  "parentId": 0,
  "remarks": "string",
  "updateBy": 0,
  "updateTime": "2019-08-24T14:15:22Z",
  "yaoce": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "yaoxin": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ]
}

```

TZfptSysCode

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|children|[[TZfptSysCode](#schematzfptsyscode)]|false|none||none|
|code|string|false|none||编号|
|createBy|integer(int64)|false|none||创建人|
|createTime|string(date-time)|false|none||创建日期|
|id|integer(int64)|false|none||主键ID|
|isUse|integer(int32)|false|none||是否有效  1 有效  2 无效|
|names|string|false|none||名称|
|orderNum|integer(int32)|false|none||显示顺序|
|parentId|integer(int64)|false|none||父级ID|
|remarks|string|false|none||说明|
|updateBy|integer(int64)|false|none||修改人|
|updateTime|string(date-time)|false|none||修改日期|
|yaoce|[[TZfptSensorPointRelation](#schematzfptsensorpointrelation)]|false|none||[二次设备与测点关联表]|
|yaoxin|[[TZfptSensorPointRelation](#schematzfptsensorpointrelation)]|false|none||[二次设备与测点关联表]|

<h2 id="tocS_TZfptSensorPointRelation">TZfptSensorPointRelation</h2>

<a id="schematzfptsensorpointrelation"></a>
<a id="schema_TZfptSensorPointRelation"></a>
<a id="tocStzfptsensorpointrelation"></a>
<a id="tocstzfptsensorpointrelation"></a>

```json
{
  "deviceType": "string",
  "dictionaryCode": "string",
  "dictionaryId": 0,
  "dictionaryName": "string",
  "id": 0,
  "paramDef": "string",
  "psrType": "string",
  "tagType": 0,
  "tagTypes": [
    0
  ],
  "unit": "string"
}

```

TZfptSensorPointRelation

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|deviceType|string|false|none||设备类型|
|dictionaryCode|string|false|none||字典表中的测点标签|
|dictionaryId|integer(int32)|false|none||字典表内测点ID|
|dictionaryName|string|false|none||名称|
|id|integer(int32)|false|none||主键ID|
|paramDef|string|false|none||值定义|
|psrType|string|false|none||电网资源标识|
|tagType|integer(int32)|false|none||1-遥测，2-遥信，3-遥控,4-遥设|
|tagTypes|[integer]|false|none||none|
|unit|string|false|none||单位|

<h2 id="tocS_TZfptHstScoreDto">TZfptHstScoreDto</h2>

<a id="schematzfpthstscoredto"></a>
<a id="schema_TZfptHstScoreDto"></a>
<a id="tocStzfpthstscoredto"></a>
<a id="tocstzfpthstscoredto"></a>

```json
{
  "createBy": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "current": 0,
  "endTime": "string",
  "id": "string",
  "score": "string",
  "scoreItemDetail": "string",
  "size": 0,
  "spaceId": "string",
  "spaceName": "string",
  "startTime": "string",
  "status": "string",
  "tableName": "string"
}

```

TZfptHstScoreDto

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|createBy|string|false|none||none|
|createTime|string(date-time)|false|none||none|
|current|integer(int32)|false|none||none|
|endTime|string|false|none||none|
|id|string|false|none||none|
|score|string|false|none||none|
|scoreItemDetail|string|false|none||none|
|size|integer(int32)|false|none||none|
|spaceId|string|false|none||none|
|spaceName|string|false|none||none|
|startTime|string|false|none||none|
|status|string|false|none||none|
|tableName|string|false|none||none|

<h2 id="tocS_TZfptAlarm">TZfptAlarm</h2>

<a id="schematzfptalarm"></a>
<a id="schema_TZfptAlarm"></a>
<a id="tocStzfptalarm"></a>
<a id="tocstzfptalarm"></a>

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "alarmSource": "string",
  "alarmState": "string",
  "alarmType": "string",
  "areaId": 0,
  "columnId": 0,
  "confirmStatus": 0,
  "continued": 0,
  "current": 0,
  "dataTime": "string",
  "deviceId": 0,
  "deviceName": "string",
  "deviceType": "string",
  "deviceTypeList": [
    "string"
  ],
  "endTime": "string",
  "evtConfirmRemarks": "string",
  "id": 0,
  "imageUuid": "string",
  "iotId": "string",
  "method": "string",
  "pageNum": 0,
  "pointId": 0,
  "remarks": "string",
  "returnTime": "2019-08-24T14:15:22Z",
  "size": 0,
  "startTime": "string",
  "stationId": 0,
  "stationName": "string",
  "tableName": "string",
  "threshold": "string",
  "timestamp": "2019-08-24T14:15:22Z",
  "value": "string"
}

```

TZfptAlarm

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|alarmLastTime|string(date-time)|false|none||最后一次告警时间|
|alarmLevel|string|false|none||1一般，2重要，3紧急|
|alarmNum|integer(int32)|false|none||告警次数|
|alarmSource|string|false|none||告警测点名|
|alarmState|string|false|none||0-恢复，1-发生|
|alarmType|string|false|none||1状态告警，2越注意上限，3越注意下限，4越警告上限，5越警告下限，6越报警上限，7越报警下限，8死态数据，20未带安全帽，21区域入侵，22人员倒地，23生物入侵|
|areaId|integer(int64)|false|none||区域ID|
|columnId|integer(int32)|false|none||域id|
|confirmStatus|integer(int32)|false|none||确认状态，0未确认1已确认|
|continued|integer(int64)|false|none||持续时间|
|current|integer(int64)|false|none||分页查询参数，当前页数|
|dataTime|string|false|none||none|
|deviceId|integer(int64)|false|none||设备id|
|deviceName|string|false|none||none|
|deviceType|string|false|none||设备类型|
|deviceTypeList|[string]|false|none||设备类型|
|endTime|string|false|none||告警结束时间|
|evtConfirmRemarks|string|false|none||none|
|id|integer(int64)|false|none||告警id|
|imageUuid|string|false|none||告警图片|
|iotId|string|false|none||设备iotId|
|method|string|false|none||事件类型|
|pageNum|integer(int64)|false|none||none|
|pointId|integer(int64)|false|none||测点id|
|remarks|string|false|none||事件分类|
|returnTime|string(date-time)|false|none||复归时间|
|size|integer(int64)|false|none||分页查询参数，当前页面每页显示的数量|
|startTime|string|false|none||告警开始时间|
|stationId|integer(int64)|false|none||站房ID|
|stationName|string|false|none||站房名称|
|tableName|string|false|none||none|
|threshold|string|false|none||告警阈值|
|timestamp|string(date-time)|false|none||告警时间|
|value|string|false|none||告警值|

<h2 id="tocS_TZfptAccountmgStation">TZfptAccountmgStation</h2>

<a id="schematzfptaccountmgstation"></a>
<a id="schema_TZfptAccountmgStation"></a>
<a id="tocStzfptaccountmgstation"></a>
<a id="tocstzfptaccountmgstation"></a>

```json
{
  "acceptancePer": "string",
  "acceptanceResult": 0,
  "acceptanceState": 0,
  "acquisitioningStrategy": 0,
  "areaId": "string",
  "areaIds": "string",
  "areaName": "string",
  "cimUuid": "string",
  "consstructionType": 0,
  "coverArea": 0,
  "createDate": "2019-08-24T14:15:22Z",
  "createFactory": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "gatewayId": 0,
  "gatewaySn": "string",
  "gatewayType": "string",
  "height": 0,
  "inspectionStrategy": 0,
  "isCalled": 0,
  "lastAcceptanceTime": "2019-08-24T14:15:22Z",
  "lastOfflineAcceptanceResult": 0,
  "lat": 0,
  "linkageStrategy": 0,
  "lon": 0,
  "operationDept": "string",
  "operationDepts": "string",
  "phone": 0,
  "pinYin": "string",
  "pinYinShouZiMu": "string",
  "pmsId": "string",
  "remark": "string",
  "rulePer": "string",
  "runState": "string",
  "stationAddr": "string",
  "stationCode": "string",
  "stationId": 0,
  "stationLevel": "string",
  "stationLine": "string",
  "stationLines": "string",
  "stationName": "string",
  "stationType": "string",
  "stationVoltId": 0,
  "svgUuid": "string",
  "thresholdStrategy": 0,
  "topicName": "string",
  "tyrq": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "usUp": 0
}

```

TZfptAccountmgStation

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|acceptancePer|string|false|none||验收人|
|acceptanceResult|integer(int32)|false|none||验收结果(0-未通过 1-已通过)|
|acceptanceState|integer(int32)|false|none||验收状态(0-未验收 1-线下验收 2-线上验收)|
|acquisitioningStrategy|integer(int32)|false|none||采集策略 0：未配置 1：已配置|
|areaId|string|false|none||所属地市,区域代码表主键ID|
|areaIds|string|false|none||所属地市,区域代码表主键ID及其父级集合|
|areaName|string|false|none||所属地市名称|
|cimUuid|string|false|none||cim模型uuid|
|consstructionType|integer(int64)|false|none||建设类型（参照字典表）|
|coverArea|number(bigdecimal)|false|none||站房面积|
|createDate|string(date-time)|false|none||建设日期|
|createFactory|string|false|none||建设厂家|
|createPer|string|false|none||创建人|
|createTime|string(date-time)|false|none||创建时间|
|gatewayId|integer(int64)|false|none||none|
|gatewaySn|string|false|none||none|
|gatewayType|string|false|none||网关类型|
|height|number(bigdecimal)|false|none||海拔|
|inspectionStrategy|integer(int32)|false|none||巡检策略 0：未配置 1：已配置|
|isCalled|integer(int32)|false|none||是否已召json文件|
|lastAcceptanceTime|string(date-time)|false|none||最后一次验收时间|
|lastOfflineAcceptanceResult|integer(int32)|false|none||最近一次线下验收结果(0未通过 1已通过)|
|lat|number(bigdecimal)|false|none||维度|
|linkageStrategy|integer(int32)|false|none||联动策略|
|lon|number(bigdecimal)|false|none||经度|
|operationDept|string|false|none||运维单位|
|operationDepts|string|false|none||运维单位ID及其父级ID集合|
|phone|integer(int64)|false|none||联系电话|
|pinYin|string|false|none||拼音|
|pinYinShouZiMu|string|false|none||拼音首字母|
|pmsId|string|false|none||none|
|remark|string|false|none||备注|
|rulePer|string|false|none||责任人|
|runState|string|false|none||运行状态  1 运行  2 停用|
|stationAddr|string|false|none||站房地址|
|stationCode|string|false|none||站房编码|
|stationId|integer(int64)|false|none||站房ID|
|stationLevel|string|false|none||1 一般 2中级 3高级|
|stationLine|string|false|none||站房所属线路|
|stationLines|string|false|none||站房所属线路ID及其父级ID集合|
|stationName|string|false|none||站所名称|
|stationType|string|false|none||1开闭所 2 环网柜 3站房|
|stationVoltId|integer(int64)|false|none||电压等级|
|svgUuid|string|false|none||站房平面图uuid|
|thresholdStrategy|integer(int32)|false|none||阈值策略 0：未配置 1：已配置|
|topicName|string|false|none||none|
|tyrq|string(date-time)|false|none||投运日期|
|updatePer|string|false|none||更改人|
|updateTime|string(date-time)|false|none||更改日期|
|usUp|integer(int32)|false|none||是否地面站房，一半地下属于地下|

<h2 id="tocS_TZfptAccountmgSensor">TZfptAccountmgSensor</h2>

<a id="schematzfptaccountmgsensor"></a>
<a id="schema_TZfptAccountmgSensor"></a>
<a id="tocStzfptaccountmgsensor"></a>
<a id="tocstzfptaccountmgsensor"></a>

```json
{
  "assetCode": "string",
  "cityId": 0,
  "cityName": "string",
  "code": "string",
  "createPer": "string",
  "describes": "string",
  "deviceId": 0,
  "deviceTemplateId": 0,
  "deviceTypeId": 0,
  "durationTime": 0,
  "durationTimes": 0,
  "gatewayId": 0,
  "id": 0,
  "manufacturerId": 0,
  "manufacturerNum": "string",
  "monthTime": 0,
  "monthTimes": 0,
  "name": "string",
  "offlineTimes": 0,
  "onlineTime": 0,
  "operationDept": 0,
  "pinYin": "string",
  "pmsId": "string",
  "posX": 0,
  "postion": "string",
  "psrId": "string",
  "remark": "string",
  "samplingFrequency": 0,
  "sensorControType": 0,
  "sensorType": "string",
  "signState": "string",
  "stationId": 0,
  "stationName": "string",
  "synStatus": "string",
  "updatePer": "string",
  "useYears": 0,
  "weekTime": 0,
  "weekTimes": 0,
  "yearTime": 0,
  "yearTimes": 0
}

```

TZfptAccountmgSensor

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|assetCode|string|false|none||none|
|cityId|number(bigdecimal)|false|none||none|
|cityName|string|false|none||none|
|code|string|false|none||none|
|createPer|string|false|none||none|
|describes|string|false|none||none|
|deviceId|number(bigdecimal)|false|none||none|
|deviceTemplateId|number(bigdecimal)|false|none||none|
|deviceTypeId|number(bigdecimal)|false|none||none|
|durationTime|number(bigdecimal)|false|none||季度在线时长|
|durationTimes|integer(int64)|false|none||季度离线次数|
|gatewayId|number(bigdecimal)|false|none||none|
|id|integer(int64)|false|none||none|
|manufacturerId|number(bigdecimal)|false|none||none|
|manufacturerNum|string|false|none||none|
|monthTime|number(bigdecimal)|false|none||月在线时长|
|monthTimes|integer(int64)|false|none||月离线次数|
|name|string|false|none||none|
|offlineTimes|integer(int64)|false|none||总离线次数|
|onlineTime|number(bigdecimal)|false|none||总在线时长|
|operationDept|number(bigdecimal)|false|none||none|
|pinYin|string|false|none||none|
|pmsId|string|false|none||none|
|posX|number(bigdecimal)|false|none||none|
|postion|string|false|none||none|
|psrId|string|false|none||none|
|remark|string|false|none||none|
|samplingFrequency|number(bigdecimal)|false|none||none|
|sensorControType|number(bigdecimal)|false|none||none|
|sensorType|string|false|none||none|
|signState|string|false|none||none|
|stationId|number(bigdecimal)|false|none||none|
|stationName|string|false|none||none|
|synStatus|string|false|none||none|
|updatePer|string|false|none||none|
|useYears|number(bigdecimal)|false|none||none|
|weekTime|number(bigdecimal)|false|none||周在线时长|
|weekTimes|integer(int64)|false|none||周离线次数|
|yearTime|number(bigdecimal)|false|none||年在线时长|
|yearTimes|integer(int64)|false|none||年离线次数|

<h2 id="tocS_TZfptAccountmgDevice">TZfptAccountmgDevice</h2>

<a id="schematzfptaccountmgdevice"></a>
<a id="schema_TZfptAccountmgDevice"></a>
<a id="tocStzfptaccountmgdevice"></a>
<a id="tocstzfptaccountmgdevice"></a>

```json
{
  "assetCode": "string",
  "cityId": 0,
  "cityName": "string",
  "createPer": "string",
  "createTime": "2019-08-24T14:15:22Z",
  "describes": "string",
  "deviceCode": "string",
  "deviceId": "string",
  "deviceModelId": "string",
  "deviceName": "string",
  "deviceTemplateId": 0,
  "deviceTypeChildrenid": 0,
  "deviceTypeId": 0,
  "dydj": "string",
  "feederId": "string",
  "id": 0,
  "manufacturerDate": "2019-08-24T14:15:22Z",
  "manufacturerId": "string",
  "manufacturerNum": "string",
  "operationDept": 0,
  "pinYin": "string",
  "pmsId": "string",
  "position": "string",
  "putDate": "2019-08-24T14:15:22Z",
  "ratedCur": "string",
  "ratedVolt": "string",
  "remark": "string",
  "retireDate": "2019-08-24T14:15:22Z",
  "stationId": 0,
  "stationName": "string",
  "takeDate": "2019-08-24T14:15:22Z",
  "updatePer": "string",
  "updateTime": "2019-08-24T14:15:22Z",
  "useYears": 0
}

```

TZfptAccountmgDevice

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|assetCode|string|false|none||资产编号|
|cityId|integer(int32)|false|none||所属地市|
|cityName|string|false|none||所属地市名称 所属地市名|
|createPer|string|false|none||创建人|
|createTime|string(date-time)|false|none||创建日期|
|describes|string|false|none||描述|
|deviceCode|string|false|none||设备编码  （设备SN）|
|deviceId|string|false|none||机器人设备id|
|deviceModelId|string|false|none||设备型号|
|deviceName|string|false|none||设备名称|
|deviceTemplateId|integer(int64)|false|none||设备模型ID|
|deviceTypeChildrenid|integer(int64)|false|none||none|
|deviceTypeId|integer(int64)|false|none||设备类型|
|dydj|string|false|none||电压等级|
|feederId|string|false|none||主变关联线路(设备为主变时填写)|
|id|integer(int64)|false|none||站房设备ID|
|manufacturerDate|string(date-time)|false|none||出厂日期|
|manufacturerId|string|false|none||生产厂商ID|
|manufacturerNum|string|false|none||出厂编号|
|operationDept|integer(int64)|false|none||运维单位ID|
|pinYin|string|false|none||拼音|
|pmsId|string|false|none||关联一次设备的资源ID|
|position|string|false|none||安装位置|
|putDate|string(date-time)|false|none||投运日期|
|ratedCur|string|false|none||额定电流|
|ratedVolt|string|false|none||额定电压|
|remark|string|false|none||备注|
|retireDate|string(date-time)|false|none||报废日期|
|stationId|integer(int64)|false|none||所属站房ID|
|stationName|string|false|none||所属站房名称|
|takeDate|string(date-time)|false|none||退役日期|
|updatePer|string|false|none||更改人|
|updateTime|string(date-time)|false|none||更改日期|
|useYears|integer(int32)|false|none||可使用年限|

<h2 id="tocS_StationQuery">StationQuery</h2>

<a id="schemastationquery"></a>
<a id="schema_StationQuery"></a>
<a id="tocSstationquery"></a>
<a id="tocsstationquery"></a>

```json
{
  "objId": "string",
  "stationName": "string",
  "type": "string"
}

```

StationQuery

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|objId|string|false|none||none|
|stationName|string|false|none||none|
|type|string|false|none||none|

<h2 id="tocS_SepConQuery">SepConQuery</h2>

<a id="schemasepconquery"></a>
<a id="schema_SepConQuery"></a>
<a id="tocSsepconquery"></a>
<a id="tocssepconquery"></a>

```json
{
  "current": 0,
  "pageNum": 0,
  "size": 0
}

```

SepConQuery

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|current|integer(int32)|false|none||none|
|pageNum|integer(int64)|false|none||none|
|size|integer(int32)|false|none||none|

<h2 id="tocS_Result«string»">Result«string»</h2>

<a id="schemaresult«string»"></a>
<a id="schema_Result«string»"></a>
<a id="tocSresult«string»"></a>
<a id="tocsresult«string»"></a>

```json
{
  "code": "string",
  "data": "string",
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«string»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|string|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«boolean»">Result«boolean»</h2>

<a id="schemaresult«boolean»"></a>
<a id="schema_Result«boolean»"></a>
<a id="tocSresult«boolean»"></a>
<a id="tocsresult«boolean»"></a>

```json
{
  "code": "string",
  "data": true,
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«boolean»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|boolean|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZrScoreItem»">Result«TZrScoreItem»</h2>

<a id="schemaresult«tzrscoreitem»"></a>
<a id="schema_Result«TZrScoreItem»"></a>
<a id="tocSresult«tzrscoreitem»"></a>
<a id="tocsresult«tzrscoreitem»"></a>

```json
{
  "code": "string",
  "data": {
    "addr": "string",
    "createBy": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "desc": "string",
    "id": 0,
    "isEnv": 0,
    "koufen": "string",
    "name": "string",
    "ownerId": "string",
    "plugin": "string",
    "remark": "string",
    "root": "string",
    "sensorType": "string",
    "stationId": "string",
    "status": 0,
    "tag": "string",
    "tagType": "string",
    "type": "string",
    "updateBy": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "url": "string",
    "yuzhileft": "string",
    "yuzhiright": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZrScoreItem»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZrScoreItem](#schematzrscoreitem)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZrRealScore»">Result«TZrRealScore»</h2>

<a id="schemaresult«tzrrealscore»"></a>
<a id="schema_Result«TZrRealScore»"></a>
<a id="tocSresult«tzrrealscore»"></a>
<a id="tocsresult«tzrrealscore»"></a>

```json
{
  "code": "string",
  "data": {
    "createBy": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "id": "string",
    "orderBy": "string",
    "pubKey": "string",
    "score": "string",
    "scoreItemDetail": "string",
    "spaceId": "string",
    "spaceIds": [
      "string"
    ],
    "spaceName": "string",
    "stationType": "string",
    "status": 0,
    "type": "string",
    "updateTime": "2019-08-24T14:15:22Z"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZrRealScore»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZrRealScore](#schematzrrealscore)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZfptSysCode»">Result«TZfptSysCode»</h2>

<a id="schemaresult«tzfptsyscode»"></a>
<a id="schema_Result«TZfptSysCode»"></a>
<a id="tocSresult«tzfptsyscode»"></a>
<a id="tocsresult«tzfptsyscode»"></a>

```json
{
  "code": "string",
  "data": {
    "children": [
      {
        "children": [
          {
            "children": null,
            "code": null,
            "createBy": null,
            "createTime": null,
            "id": null,
            "isUse": null,
            "names": null,
            "orderNum": null,
            "parentId": null,
            "remarks": null,
            "updateBy": null,
            "updateTime": null,
            "yaoce": null,
            "yaoxin": null
          }
        ],
        "code": "string",
        "createBy": 0,
        "createTime": "2019-08-24T14:15:22Z",
        "id": 0,
        "isUse": 0,
        "names": "string",
        "orderNum": 0,
        "parentId": 0,
        "remarks": "string",
        "updateBy": 0,
        "updateTime": "2019-08-24T14:15:22Z",
        "yaoce": [
          {
            "deviceType": null,
            "dictionaryCode": null,
            "dictionaryId": null,
            "dictionaryName": null,
            "id": null,
            "paramDef": null,
            "psrType": null,
            "tagType": null,
            "tagTypes": null,
            "unit": null
          }
        ],
        "yaoxin": [
          {
            "deviceType": null,
            "dictionaryCode": null,
            "dictionaryId": null,
            "dictionaryName": null,
            "id": null,
            "paramDef": null,
            "psrType": null,
            "tagType": null,
            "tagTypes": null,
            "unit": null
          }
        ]
      }
    ],
    "code": "string",
    "createBy": 0,
    "createTime": "2019-08-24T14:15:22Z",
    "id": 0,
    "isUse": 0,
    "names": "string",
    "orderNum": 0,
    "parentId": 0,
    "remarks": "string",
    "updateBy": 0,
    "updateTime": "2019-08-24T14:15:22Z",
    "yaoce": [
      {
        "deviceType": "string",
        "dictionaryCode": "string",
        "dictionaryId": 0,
        "dictionaryName": "string",
        "id": 0,
        "paramDef": "string",
        "psrType": "string",
        "tagType": 0,
        "tagTypes": [
          0
        ],
        "unit": "string"
      }
    ],
    "yaoxin": [
      {
        "deviceType": "string",
        "dictionaryCode": "string",
        "dictionaryId": 0,
        "dictionaryName": "string",
        "id": 0,
        "paramDef": "string",
        "psrType": "string",
        "tagType": 0,
        "tagTypes": [
          0
        ],
        "unit": "string"
      }
    ]
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZfptSysCode»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZfptSysCode](#schematzfptsyscode)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZfptSensorPointRelation»">Result«TZfptSensorPointRelation»</h2>

<a id="schemaresult«tzfptsensorpointrelation»"></a>
<a id="schema_Result«TZfptSensorPointRelation»"></a>
<a id="tocSresult«tzfptsensorpointrelation»"></a>
<a id="tocsresult«tzfptsensorpointrelation»"></a>

```json
{
  "code": "string",
  "data": {
    "deviceType": "string",
    "dictionaryCode": "string",
    "dictionaryId": 0,
    "dictionaryName": "string",
    "id": 0,
    "paramDef": "string",
    "psrType": "string",
    "tagType": 0,
    "tagTypes": [
      0
    ],
    "unit": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZfptSensorPointRelation»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZfptSensorPointRelation](#schematzfptsensorpointrelation)|false|none||二次设备与测点关联表|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZfptAlarm»">Result«TZfptAlarm»</h2>

<a id="schemaresult«tzfptalarm»"></a>
<a id="schema_Result«TZfptAlarm»"></a>
<a id="tocSresult«tzfptalarm»"></a>
<a id="tocsresult«tzfptalarm»"></a>

```json
{
  "code": "string",
  "data": {
    "alarmLastTime": "2019-08-24T14:15:22Z",
    "alarmLevel": "string",
    "alarmNum": 0,
    "alarmSource": "string",
    "alarmState": "string",
    "alarmType": "string",
    "areaId": 0,
    "columnId": 0,
    "confirmStatus": 0,
    "continued": 0,
    "current": 0,
    "dataTime": "string",
    "deviceId": 0,
    "deviceName": "string",
    "deviceType": "string",
    "deviceTypeList": [
      "string"
    ],
    "endTime": "string",
    "evtConfirmRemarks": "string",
    "id": 0,
    "imageUuid": "string",
    "iotId": "string",
    "method": "string",
    "pageNum": 0,
    "pointId": 0,
    "remarks": "string",
    "returnTime": "2019-08-24T14:15:22Z",
    "size": 0,
    "startTime": "string",
    "stationId": 0,
    "stationName": "string",
    "tableName": "string",
    "threshold": "string",
    "timestamp": "2019-08-24T14:15:22Z",
    "value": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZfptAlarm»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZfptAlarm](#schematzfptalarm)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZfptAccountmgStation»">Result«TZfptAccountmgStation»</h2>

<a id="schemaresult«tzfptaccountmgstation»"></a>
<a id="schema_Result«TZfptAccountmgStation»"></a>
<a id="tocSresult«tzfptaccountmgstation»"></a>
<a id="tocsresult«tzfptaccountmgstation»"></a>

```json
{
  "code": "string",
  "data": {
    "acceptancePer": "string",
    "acceptanceResult": 0,
    "acceptanceState": 0,
    "acquisitioningStrategy": 0,
    "areaId": "string",
    "areaIds": "string",
    "areaName": "string",
    "cimUuid": "string",
    "consstructionType": 0,
    "coverArea": 0,
    "createDate": "2019-08-24T14:15:22Z",
    "createFactory": "string",
    "createPer": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "gatewayId": 0,
    "gatewaySn": "string",
    "gatewayType": "string",
    "height": 0,
    "inspectionStrategy": 0,
    "isCalled": 0,
    "lastAcceptanceTime": "2019-08-24T14:15:22Z",
    "lastOfflineAcceptanceResult": 0,
    "lat": 0,
    "linkageStrategy": 0,
    "lon": 0,
    "operationDept": "string",
    "operationDepts": "string",
    "phone": 0,
    "pinYin": "string",
    "pinYinShouZiMu": "string",
    "pmsId": "string",
    "remark": "string",
    "rulePer": "string",
    "runState": "string",
    "stationAddr": "string",
    "stationCode": "string",
    "stationId": 0,
    "stationLevel": "string",
    "stationLine": "string",
    "stationLines": "string",
    "stationName": "string",
    "stationType": "string",
    "stationVoltId": 0,
    "svgUuid": "string",
    "thresholdStrategy": 0,
    "topicName": "string",
    "tyrq": "2019-08-24T14:15:22Z",
    "updatePer": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "usUp": 0
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZfptAccountmgStation»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZfptAccountmgStation](#schematzfptaccountmgstation)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«TZfptAccountmgDevice»">Result«TZfptAccountmgDevice»</h2>

<a id="schemaresult«tzfptaccountmgdevice»"></a>
<a id="schema_Result«TZfptAccountmgDevice»"></a>
<a id="tocSresult«tzfptaccountmgdevice»"></a>
<a id="tocsresult«tzfptaccountmgdevice»"></a>

```json
{
  "code": "string",
  "data": {
    "assetCode": "string",
    "cityId": 0,
    "cityName": "string",
    "createPer": "string",
    "createTime": "2019-08-24T14:15:22Z",
    "describes": "string",
    "deviceCode": "string",
    "deviceId": "string",
    "deviceModelId": "string",
    "deviceName": "string",
    "deviceTemplateId": 0,
    "deviceTypeChildrenid": 0,
    "deviceTypeId": 0,
    "dydj": "string",
    "feederId": "string",
    "id": 0,
    "manufacturerDate": "2019-08-24T14:15:22Z",
    "manufacturerId": "string",
    "manufacturerNum": "string",
    "operationDept": 0,
    "pinYin": "string",
    "pmsId": "string",
    "position": "string",
    "putDate": "2019-08-24T14:15:22Z",
    "ratedCur": "string",
    "ratedVolt": "string",
    "remark": "string",
    "retireDate": "2019-08-24T14:15:22Z",
    "stationId": 0,
    "stationName": "string",
    "takeDate": "2019-08-24T14:15:22Z",
    "updatePer": "string",
    "updateTime": "2019-08-24T14:15:22Z",
    "useYears": 0
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«TZfptAccountmgDevice»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[TZfptAccountmgDevice](#schematzfptaccountmgdevice)|false|none||一次设备表|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«RealApiVo»">Result«RealApiVo»</h2>

<a id="schemaresult«realapivo»"></a>
<a id="schema_Result«RealApiVo»"></a>
<a id="tocSresult«realapivo»"></a>
<a id="tocsresult«realapivo»"></a>

```json
{
  "code": "string",
  "data": {
    "timestamp": "string",
    "value": "string"
  },
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«RealApiVo»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[RealApiVo](#schemarealapivo)|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZrScoreItem»»">Result«List«TZrScoreItem»»</h2>

<a id="schemaresult«list«tzrscoreitem»»"></a>
<a id="schema_Result«List«TZrScoreItem»»"></a>
<a id="tocSresult«list«tzrscoreitem»»"></a>
<a id="tocsresult«list«tzrscoreitem»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "addr": "string",
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "desc": "string",
      "id": 0,
      "isEnv": 0,
      "koufen": "string",
      "name": "string",
      "ownerId": "string",
      "plugin": "string",
      "remark": "string",
      "root": "string",
      "sensorType": "string",
      "stationId": "string",
      "status": 0,
      "tag": "string",
      "tagType": "string",
      "type": "string",
      "updateBy": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "url": "string",
      "yuzhileft": "string",
      "yuzhiright": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZrScoreItem»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZrScoreItem](#schematzrscoreitem)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZrRealScore»»">Result«List«TZrRealScore»»</h2>

<a id="schemaresult«list«tzrrealscore»»"></a>
<a id="schema_Result«List«TZrRealScore»»"></a>
<a id="tocSresult«list«tzrrealscore»»"></a>
<a id="tocsresult«list«tzrrealscore»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "createBy": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "id": "string",
      "orderBy": "string",
      "pubKey": "string",
      "score": "string",
      "scoreItemDetail": "string",
      "spaceId": "string",
      "spaceIds": [
        "string"
      ],
      "spaceName": "string",
      "stationType": "string",
      "status": 0,
      "type": "string",
      "updateTime": "2019-08-24T14:15:22Z"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZrRealScore»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZrRealScore](#schematzrrealscore)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptSysCode»»">Result«List«TZfptSysCode»»</h2>

<a id="schemaresult«list«tzfptsyscode»»"></a>
<a id="schema_Result«List«TZfptSysCode»»"></a>
<a id="tocSresult«list«tzfptsyscode»»"></a>
<a id="tocsresult«list«tzfptsyscode»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "children": [
        {
          "children": [
            {}
          ],
          "code": "string",
          "createBy": 0,
          "createTime": "2019-08-24T14:15:22Z",
          "id": 0,
          "isUse": 0,
          "names": "string",
          "orderNum": 0,
          "parentId": 0,
          "remarks": "string",
          "updateBy": 0,
          "updateTime": "2019-08-24T14:15:22Z",
          "yaoce": [
            {}
          ],
          "yaoxin": [
            {}
          ]
        }
      ],
      "code": "string",
      "createBy": 0,
      "createTime": "2019-08-24T14:15:22Z",
      "id": 0,
      "isUse": 0,
      "names": "string",
      "orderNum": 0,
      "parentId": 0,
      "remarks": "string",
      "updateBy": 0,
      "updateTime": "2019-08-24T14:15:22Z",
      "yaoce": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ],
      "yaoxin": [
        {
          "deviceType": "string",
          "dictionaryCode": "string",
          "dictionaryId": 0,
          "dictionaryName": "string",
          "id": 0,
          "paramDef": "string",
          "psrType": "string",
          "tagType": 0,
          "tagTypes": [
            0
          ],
          "unit": "string"
        }
      ]
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptSysCode»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptSysCode](#schematzfptsyscode)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptSensorPointRelation»»">Result«List«TZfptSensorPointRelation»»</h2>

<a id="schemaresult«list«tzfptsensorpointrelation»»"></a>
<a id="schema_Result«List«TZfptSensorPointRelation»»"></a>
<a id="tocSresult«list«tzfptsensorpointrelation»»"></a>
<a id="tocsresult«list«tzfptsensorpointrelation»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "deviceType": "string",
      "dictionaryCode": "string",
      "dictionaryId": 0,
      "dictionaryName": "string",
      "id": 0,
      "paramDef": "string",
      "psrType": "string",
      "tagType": 0,
      "tagTypes": [
        0
      ],
      "unit": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptSensorPointRelation»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptSensorPointRelation](#schematzfptsensorpointrelation)]|false|none||[二次设备与测点关联表]|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptAlarm»»">Result«List«TZfptAlarm»»</h2>

<a id="schemaresult«list«tzfptalarm»»"></a>
<a id="schema_Result«List«TZfptAlarm»»"></a>
<a id="tocSresult«list«tzfptalarm»»"></a>
<a id="tocsresult«list«tzfptalarm»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "alarmSource": "string",
      "alarmState": "string",
      "alarmType": "string",
      "areaId": 0,
      "columnId": 0,
      "confirmStatus": 0,
      "continued": 0,
      "current": 0,
      "dataTime": "string",
      "deviceId": 0,
      "deviceName": "string",
      "deviceType": "string",
      "deviceTypeList": [
        "string"
      ],
      "endTime": "string",
      "evtConfirmRemarks": "string",
      "id": 0,
      "imageUuid": "string",
      "iotId": "string",
      "method": "string",
      "pageNum": 0,
      "pointId": 0,
      "remarks": "string",
      "returnTime": "2019-08-24T14:15:22Z",
      "size": 0,
      "startTime": "string",
      "stationId": 0,
      "stationName": "string",
      "tableName": "string",
      "threshold": "string",
      "timestamp": "2019-08-24T14:15:22Z",
      "value": "string"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptAlarm»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptAlarm](#schematzfptalarm)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptAccountmgStation»»">Result«List«TZfptAccountmgStation»»</h2>

<a id="schemaresult«list«tzfptaccountmgstation»»"></a>
<a id="schema_Result«List«TZfptAccountmgStation»»"></a>
<a id="tocSresult«list«tzfptaccountmgstation»»"></a>
<a id="tocsresult«list«tzfptaccountmgstation»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "acceptancePer": "string",
      "acceptanceResult": 0,
      "acceptanceState": 0,
      "acquisitioningStrategy": 0,
      "areaId": "string",
      "areaIds": "string",
      "areaName": "string",
      "cimUuid": "string",
      "consstructionType": 0,
      "coverArea": 0,
      "createDate": "2019-08-24T14:15:22Z",
      "createFactory": "string",
      "createPer": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "gatewayId": 0,
      "gatewaySn": "string",
      "gatewayType": "string",
      "height": 0,
      "inspectionStrategy": 0,
      "isCalled": 0,
      "lastAcceptanceTime": "2019-08-24T14:15:22Z",
      "lastOfflineAcceptanceResult": 0,
      "lat": 0,
      "linkageStrategy": 0,
      "lon": 0,
      "operationDept": "string",
      "operationDepts": "string",
      "phone": 0,
      "pinYin": "string",
      "pinYinShouZiMu": "string",
      "pmsId": "string",
      "remark": "string",
      "rulePer": "string",
      "runState": "string",
      "stationAddr": "string",
      "stationCode": "string",
      "stationId": 0,
      "stationLevel": "string",
      "stationLine": "string",
      "stationLines": "string",
      "stationName": "string",
      "stationType": "string",
      "stationVoltId": 0,
      "svgUuid": "string",
      "thresholdStrategy": 0,
      "topicName": "string",
      "tyrq": "2019-08-24T14:15:22Z",
      "updatePer": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "usUp": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptAccountmgStation»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptAccountmgStation](#schematzfptaccountmgstation)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptAccountmgSensor»»">Result«List«TZfptAccountmgSensor»»</h2>

<a id="schemaresult«list«tzfptaccountmgsensor»»"></a>
<a id="schema_Result«List«TZfptAccountmgSensor»»"></a>
<a id="tocSresult«list«tzfptaccountmgsensor»»"></a>
<a id="tocsresult«list«tzfptaccountmgsensor»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "assetCode": "string",
      "cityId": 0,
      "cityName": "string",
      "code": "string",
      "createPer": "string",
      "describes": "string",
      "deviceId": 0,
      "deviceTemplateId": 0,
      "deviceTypeId": 0,
      "durationTime": 0,
      "durationTimes": 0,
      "gatewayId": 0,
      "id": 0,
      "manufacturerId": 0,
      "manufacturerNum": "string",
      "monthTime": 0,
      "monthTimes": 0,
      "name": "string",
      "offlineTimes": 0,
      "onlineTime": 0,
      "operationDept": 0,
      "pinYin": "string",
      "pmsId": "string",
      "posX": 0,
      "postion": "string",
      "psrId": "string",
      "remark": "string",
      "samplingFrequency": 0,
      "sensorControType": 0,
      "sensorType": "string",
      "signState": "string",
      "stationId": 0,
      "stationName": "string",
      "synStatus": "string",
      "updatePer": "string",
      "useYears": 0,
      "weekTime": 0,
      "weekTimes": 0,
      "yearTime": 0,
      "yearTimes": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptAccountmgSensor»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptAccountmgSensor](#schematzfptaccountmgsensor)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«TZfptAccountmgDevice»»">Result«List«TZfptAccountmgDevice»»</h2>

<a id="schemaresult«list«tzfptaccountmgdevice»»"></a>
<a id="schema_Result«List«TZfptAccountmgDevice»»"></a>
<a id="tocSresult«list«tzfptaccountmgdevice»»"></a>
<a id="tocsresult«list«tzfptaccountmgdevice»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "assetCode": "string",
      "cityId": 0,
      "cityName": "string",
      "createPer": "string",
      "createTime": "2019-08-24T14:15:22Z",
      "describes": "string",
      "deviceCode": "string",
      "deviceId": "string",
      "deviceModelId": "string",
      "deviceName": "string",
      "deviceTemplateId": 0,
      "deviceTypeChildrenid": 0,
      "deviceTypeId": 0,
      "dydj": "string",
      "feederId": "string",
      "id": 0,
      "manufacturerDate": "2019-08-24T14:15:22Z",
      "manufacturerId": "string",
      "manufacturerNum": "string",
      "operationDept": 0,
      "pinYin": "string",
      "pmsId": "string",
      "position": "string",
      "putDate": "2019-08-24T14:15:22Z",
      "ratedCur": "string",
      "ratedVolt": "string",
      "remark": "string",
      "retireDate": "2019-08-24T14:15:22Z",
      "stationId": 0,
      "stationName": "string",
      "takeDate": "2019-08-24T14:15:22Z",
      "updatePer": "string",
      "updateTime": "2019-08-24T14:15:22Z",
      "useYears": 0
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«TZfptAccountmgDevice»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[TZfptAccountmgDevice](#schematzfptaccountmgdevice)]|false|none||[一次设备表]|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result«List«AlarmDto»»">Result«List«AlarmDto»»</h2>

<a id="schemaresult«list«alarmdto»»"></a>
<a id="schema_Result«List«AlarmDto»»"></a>
<a id="tocSresult«list«alarmdto»»"></a>
<a id="tocsresult«list«alarmdto»»"></a>

```json
{
  "code": "string",
  "data": [
    {
      "alarmLastTime": "2019-08-24T14:15:22Z",
      "alarmLevel": "string",
      "alarmNum": 0,
      "deviceType": "string",
      "deviceTypeName": "string",
      "endTime": "2019-08-24T14:15:22Z",
      "imageUuid": "string",
      "method": "string",
      "methodName": "string",
      "remarks": "string",
      "startTime": "2019-08-24T14:15:22Z",
      "stationId": 0,
      "stationName": "string",
      "timestamp": "2019-08-24T14:15:22Z"
    }
  ],
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result«List«AlarmDto»»

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|[[AlarmDto](#schemaalarmdto)]|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_Result">Result</h2>

<a id="schemaresult"></a>
<a id="schema_Result"></a>
<a id="tocSresult"></a>
<a id="tocsresult"></a>

```json
{
  "code": "string",
  "data": {},
  "i18n": "string",
  "message": "string",
  "time": "2019-08-24T14:15:22Z",
  "total": 0,
  "value": "string"
}

```

Result

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|code|string|false|none||none|
|data|object|false|none||none|
|i18n|string|false|none||none|
|message|string|false|none||none|
|time|string(date-time)|false|none||none|
|total|integer(int64)|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_RealApiVo">RealApiVo</h2>

<a id="schemarealapivo"></a>
<a id="schema_RealApiVo"></a>
<a id="tocSrealapivo"></a>
<a id="tocsrealapivo"></a>

```json
{
  "timestamp": "string",
  "value": "string"
}

```

RealApiVo

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|timestamp|string|false|none||none|
|value|string|false|none||none|

<h2 id="tocS_AlarmDto">AlarmDto</h2>

<a id="schemaalarmdto"></a>
<a id="schema_AlarmDto"></a>
<a id="tocSalarmdto"></a>
<a id="tocsalarmdto"></a>

```json
{
  "alarmLastTime": "2019-08-24T14:15:22Z",
  "alarmLevel": "string",
  "alarmNum": 0,
  "deviceType": "string",
  "deviceTypeName": "string",
  "endTime": "2019-08-24T14:15:22Z",
  "imageUuid": "string",
  "method": "string",
  "methodName": "string",
  "remarks": "string",
  "startTime": "2019-08-24T14:15:22Z",
  "stationId": 0,
  "stationName": "string",
  "timestamp": "2019-08-24T14:15:22Z"
}

```

AlarmDto

### Attribute

|Name|Type|Required|Restrictions|Title|Description|
|---|---|---|---|---|---|
|alarmLastTime|string(date-time)|false|none||最后一次告警时间|
|alarmLevel|string|false|none||1一般，2重要，3紧急|
|alarmNum|integer(int32)|false|none||告警次数|
|deviceType|string|false|none||设备类型|
|deviceTypeName|string|false|none||none|
|endTime|string(date-time)|false|none||告警结束时间|
|imageUuid|string|false|none||告警图片|
|method|string|false|none||事件类型|
|methodName|string|false|none||事件类型名称|
|remarks|string|false|none||设备类型名称|
|startTime|string(date-time)|false|none||告警开始时间|
|stationId|integer(int64)|false|none||站房ID|
|stationName|string|false|none||站房名称|
|timestamp|string(date-time)|false|none||告警时间|

