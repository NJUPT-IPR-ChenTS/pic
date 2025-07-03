## 账户管理API

### 1.获取主账户名下的所有小红书账号
**Endpoint**:  
`GET http://0.0.0.0:8088/accounts/{admin}`
#### 参数说明: 1、admin:主账户名称；2、xhs_username:主账户下关联的小红书本地账户名；3、user_id:主账户下关联的小红书平台账户id；
#### 响应示例
```json
[
    {
        "xhs_username": "Xhs_account2",
        "xhs_id": "default",
        "user_id": "xxxxx"
    },
]
```
