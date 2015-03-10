---
会议管家数据库文档 
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
nickname|String|是| | 昵称
job|String|否| | 职位
state|Integer|是| 0 |状态
role|Integer| 是| 0 |角色 0：普通用户 1：供应商
os_type| String| 是| 0 |操作类型 0：安卓 1：ios
token|String|是| | 秘钥 

#活动会场
## 3：meetingplaces

### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 活动名称
category_id|Integer|是| |分类
user_id|Integer|是||用户
state|Integer| 是| 0 |状态
address|String|是| | 地址
lng|String | 否| | 经度
lat|String | 否| | 纬度
desc|String | 否| | 描述


#展厅
##4：exhibition_rooms

### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 展厅名称
area|String |是| | 面积
pdf | String |是| | pdf文件
ai |String |否|| ai文件
price |float|是 || 价格
long |String |是|| 长
width |String |是|| 宽
height |String |是|| 净高
light_height |String |是|| 灯下高


 
