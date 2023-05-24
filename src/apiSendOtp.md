# apiSendOtp
產生簡訊OTP

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/megaOtp/V1/interfaces/apiSendOtp
```

### HTTP Request Mehod
```
GET
```

### JSON representation

Here is a JSON representation of request.
```json
{
  "requestHeader": {
  },
  "requestBody": {
    "phone": "0978321626",
    "employeeId": "000014"
  },
}
```

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| phone | "0978321626" | String | 手機號碼 | N | n/a |
| employeeId | "000014" | String | 員工編號 | N | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| responseDate | 回應時間 |
| returnCode | 回應代碼 |
| returnDesc | 回應代碼說明 |
| otp | 驗證碼 |


### HTTP Response when Successful
```json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "responseDate":"2023/05/24",
      "returnCode":"0000",
      "returnDesc":"成功",
      "otp":"850921"
   }
}
```

### HTTP Response when No Data
此程式不會有查無資料發生

### HTTP Response when Failed
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "500"
    },
    "responseBody": {
    }
}
```

### HTTP Response when Exception
```json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "406"
    },
    "responseBody": {
    }
}
```
