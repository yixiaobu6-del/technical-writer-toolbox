# API 文档模板

## 接口概览

```
# {{接口名称}}

## {{接口描述}}

### 请求方式
{{GET / POST / PUT / DELETE}}

### 请求地址
```
{{API_ENDPOINT}}/{{path}}
```

### 请求头
| 参数名 | 类型 | 必填 | 说明 |
|--------|------|:----:|------|
| Content-Type | string | 是 | application/json |
| Authorization | string | 是 | Bearer {{token}} |

### 请求参数
| 参数名 | 类型 | 必填 | 说明 | 示例 |
|--------|------|:----:|------|------|
| id | integer | 是 | 用户ID | 12345 |
| name | string | 否 | 用户名 | "张三" |

### 响应示例

```json
{
  "code": 0,
  "message": "success",
  "data": {
    "id": 12345,
    "name": "张三"
  }
}
```

### 错误码
| 错误码 | 说明 |
|:------:|------|
| 10001 | 参数错误 |
| 10002 | 认证失败 |
```

---

> 版本：1.0