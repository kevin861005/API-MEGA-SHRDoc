# apiGetUpdateURL
取得兌換碼網址

### HTTP Request
```
http://192.168.10.111/servlet/apiM/megaOtp/V1/interfaces/apiGetUpdateURL
```

### HTTP Request Mehod
```
POST
```

### JSON representation
Here is a JSON representation of request.
```
json
{
  "requestHeader": {
  },
  "requestBody": {
    "device": "xxx",
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
| device | iOS/Android | String | 裝置型別 | Y | n/a |
| employeeId | xxx | String | 員工編號 | iOS(Y)/Android(N) | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| url | 兌換碼更新網址 |

### HTTP Response when Successful
```
json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "url": "xxx"
   }
}
```

### HTTP Response when No Data
此程式不會有查無資料發生

### HTTP Response when Failed
```
json
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
```
json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "406"
    },
    "responseBody": {
    }
}
```
