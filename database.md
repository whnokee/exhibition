---
会议管理数据库文档 
---

# 后台用户管理
## 1：admin_users
 
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
account|String|是| |帐号
password|String|是| |密码
role|Integer| 是| 1 |角色 1：系统管理 2：编辑 3：运营
 
 
# 用户管理
## 2：users
 
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
account|String|是| |帐号
password|String|是| |密码
name|String|是| | 昵称
job|String|否| | 职位
state|Integer|是| 0 |状态
role|Integer| 是| 0 |角色 0：普通用户 1：供应商
token|String|是| | 秘钥 
os_type| String| 是| 0 |操作类型 0：安卓 1：ios

 
