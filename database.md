---
那刻魔镜端API接口文档 
---

# 设备管理
## 1： 获取设备码
### 请求地址
/devices/generate_code
### 请求方式
post
### 请求参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
product_id|String|是| |设备号
###示例
```
正确
{"recode":0,"msg":"返回成功","data":{"device_code":"8we03mps"}}
错误：
{:recode=>-1, :msg:'返回失败' }
```
 
