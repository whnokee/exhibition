---
#会展通数据库文档 
---
 
 
# 用户表
## 1：users
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
account|String|是| |帐号
password|String|是| |密码
nickname|String|是| | 昵称
job|String|否| | 职位
state|Integer|是| 0 |状态
role|Integer| 是| 0 |角色 0：普通用户 1：供应商 2：系统管理员
os_type| String| 是| 0 |操作类型 0：安卓 1：ios
head|String|是||头像
token|String|是| | 秘钥 
email|String|否| |邮箱

#短信
##2：sms
名称|类型|是否必须|默认值|描述
---|---|----|---|---
captcha|String|是| |激活码
captchatime|Date|是| |截止时间
mobile|Integer|是|| 手机
state|Integer|是|0|是否激活


#活动会场
## 3：places
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 会场名称
category_id|Integer|是| |分类
user_id|Integer|是||用户
province|String|是||省
city|String|是||市
business_area|String|否|商圈
state|Integer| 是| 0 |状态
address|String|是| | 地址
lng|String | 否| | 经度
lat|String | 否| | 纬度
desc|String | 否| | 描述
tel|String | 否||电话
star|Integer|否||星级
sale_info|String| 否||促销信息
price_area |String|是 || 价格范围

#展厅
##4： rooms
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
place_id|Integer|是| |会场
name|String |是| | 展厅名称
area|String |是| | 面积
pdf | String |是| | pdf文件
ai |String |否|| ai文件
price |float|是 || 价格
long |String |是|| 长
width |String |是|| 宽
height |String |是|| 净高
light_height |String |是|| 灯下高
juyuan|String|是||剧院式
yanhui|String|是||宴会式
kezhuo|String|是||课桌式
comment_count|Integer|是|0|评论数

#活动
## 5 events
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
place_id|Integer|是| |会场
name|String |是| | 活动名称
zan|Integer|是| 0 |赞
desc|String|否| | 描述


#鲜花组合
##6：group_flowers
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 名称
desc|String |是| | 描述
price|float|是| | 价格

#鲜花
##7：flowers
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 名称
group_flower_id|Integer|是| |鲜花组合
cnt|Integer|是 || 数量
desc|String |是| | 描述

#订单
##8：orders
### 字段参数
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String |是| | 名称
desc|String |是| | 描述
target_type|String|是|| 订单类型 
target_id |Integer|是|| 购买产品
price |float|是 || 价格
state|integer|是|0| 订单状态
user_id|integer|是| |用户
cnt|Integer|是|0|数量

#图片库
##9：assets
名称|类型|是否必须|默认值|描述
---|---|----|---|---
target_id|Integer|是| | 附件
target_type|String|是| | 附件类型
file|String|是||图片路径
desc|String|是||图片描述
size|String|否||文件大小

#分类
## 10： categories
名称|类型|是否必须|默认值|描述
---|---|----|---|---
name|String|是||名称
type|Inteter|是|0|类型
state|Inteter|是|1|状态

#反馈
## 11： feedbacks
名称|类型|是否必须|默认值|描述
---|---|----|---|---
content|String|是||内容
user_id|integer|是|| 用户

#版本
##12：versions
名称|类型|是否必须|默认值|描述
---|---|----|---|---
number|integer|是|| 版本号
file|String| 是||文件
desc|String|是||描述
os_type|integer|是|0|操作系统
state|integer|是|0|状态

#评论
##13：comments
名称|类型|是否必须|默认值|描述
---|---|----|---|---
content|String|是|| 内容
user_id|Integer|是||用户
target_id|Integer|是|| 会场
target_type|String|是|| 类型
state|Integer|是|0|状态

#广告栏目
##13：advertisements
名称|类型|是否必须|默认值|描述
---|---|----|---|---
title|String|是|| 标题
state|Integer|是|0|状态
link_url|String|否||外链
target_id|Integer|否|| 会场or鲜花
target_type|String|否|| 会场or鲜花类型
 
