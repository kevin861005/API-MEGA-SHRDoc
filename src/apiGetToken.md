# apiGetToken
取得登入token

### HTTP Request
```
http://59.124.100.151:8090/servlet/apiM/megaOtp/V1/interfaces/apiGetToken
```

### HTTP Request Mehod
```
POST
```

### JSON representation

Here is a JSON representation of request.
```json
{
    "requestHeader": {
    },
    "requestBody": {
        "employeeId": "xxx"
    }
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
| employeeId | "850921" | String | 員工編號 | Y | n/a |

### responseBody FieldName
| FieldName | Description |
|:----------|:-------------|
| token | 登入 token |


### HTTP Response when Successful
```json
{
    "responseHeader": {
        "resultMessage": "執行成功",
        "resultCode": "200"
    },
    "responseBody": {
        "token": "12724332507640369936588067624218587609270069965590708406437785953105268880553881948858089532274080"
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
