## 账户管理API

### 1.获取主账户名下的所有小红书账号
**Endpoint**:  
`GET http://0.0.0.0:8088/accounts/{main_account}`
#### 参数说明: 1、main_account:主账户名称；2、xhs_username:主账户下关联的小红书本地账户名；3、user_id:主账户下关联的小红书平台账户id；
#### 响应示例
```json
[
    {
        "xhs_username": "Xhs_account2",
        "user_id": "xxxxx"
    }
]
```

### 2.创建主账户
**Endpoint**: 
`POST "http://0.0.0.0:8088/accounts/account/create/{main_account}`
#### 参数说明: 1、main_account:主账户名称；
#### 响应示例
```json
{
    "message": "主账号创建成功"
}
```

### 3.删除主账户
**Endpoint**:
`DELETE "http://0.0.0.0:8088/accounts/account/delete/{main_account}"`
#### 参数说明: 1、main_account:主账户名称；
#### 响应示例
```json
{
    "message": "主账号删除成功"
}
```

### 4.基于某个主账户创建小红书账户
**Endpoint**:
`POST "http://0.0.0.0:8088/accounts/xhs_account/create"`
#### 参数说明: 1、main_account:主账户名称；2、xhs_username:小红书本地账户名称；
#### 请求示例
```json
{
    "main_account": "Admin",
    "xhs_username": "xxxxx"
}
```
#### 响应示例
```json
{
    "message": "小红书账号创建成功"
}
```

### 5.删除小红书账户
**Endpoint**:
`DELETE "http://0.0.0.0:8088/accounts/xhs_account/delete/{xhs_username}"`
#### 参数说明: 1、xhs_username:小红书本地账户名称；
#### 响应示例
```json
{
    "message": "小红书账号删除成功"
}
```
