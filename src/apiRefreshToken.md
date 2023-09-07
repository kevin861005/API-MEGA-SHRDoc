# apiRefreshToken
重新取得Token

### HTTP Request
http://59.124.100.151:8090/servlet/apiM/megaOtp/V1/interfaces/apiRefreshToken

### HTTP Request Mehod
POST

### JSON representation

Here is a JSON representation of request.
json
{
  "requestHeader": {
  },
  "requestBody": {
    "token": "xxx"
  }
}

### Properties
| Property | Type | Description |
|:---------|:-----|:------------|
| requestHeader | Object | 要求本文 |
| requestBody | Object | 要求本文 |

### requestBody Properties
| Key | Value | Type | Description | Required | Format |
|:----------|:-------------|:-----|:------------|:------------|:------------|
| token | xxx | String | token | Y | n/a |

### requestBody FieldName
| FieldName | Description |
|:----------|:-------------|
| isSuccess | 是否成功 |
| message | 訊息 |
| refreshToken | 新token |

### Note
只要 isSuccess 為 false，或是 resultCode = 500 或 resultCode = 406，就顯示錯誤訊息，點擊後回到微軟登入畫面


### HTTP Response when Successful
json
{
   "responseHeader":{
      "resultMessage":"執行成功",
      "resultCode":"200"
   },
   "responseBody":{
      "isSuccess":false,
      "message":"取得token失敗，請重新登入",
      "refreshToken":""
   }
}

### HTTP Response when No Data
此程式不會有查無資料發生

### HTTP Response when Failed
json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "500"
    },
    "responseBody": {
    }
}

### HTTP Response when Exception
json
{
    "responseHeader": {
        "resultMessage": "xxxxx",
        "resultCode": "406"
    },
    "responseBody": {
    }
}
