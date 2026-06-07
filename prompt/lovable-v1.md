
# 预约管家（Booking Manager）

## 项目简介

开发一个移动端优先（Mobile First）的预约管理系统。

目标用户：

- 美甲店
- 美睫店
- 美容院
- SPA店
- 理发店

主要用于：

- 客户预约管理
- 技师管理
- 服务项目管理
- 预约排班管理

技术栈：

- Next.js 15
- TypeScript
- TailwindCSS
- Shadcn UI
- Supabase
- Responsive Design

---

# UI要求

风格参考：

- 微信
- 企业微信
- 美团商家版

要求：

- 简洁
- 清爽
- 大按钮
- 手机优先

主色：

#2563EB

辅助色：

#10B981

警告色：

#EF4444

---

# 登录页

字段：

邮箱

密码

按钮：

登录

使用 Supabase Auth

---

# 首页 Dashboard

显示：

今日预约数

待到店数量

服务中数量

已完成数量

今日营业额

按钮：

新增预约

查看预约

客户管理

技师管理

服务项目

---

# 客户管理

数据表：

customers

字段：

name

phone

wechat_nickname

wechat_id

note

功能：

新增客户

编辑客户

删除客户

搜索客户

支持手机号搜索

---

# 技师管理

数据表：

technicians

字段：

name

phone

specialties

status

note

功能：

新增

编辑

删除

搜索

---

# 服务项目管理

数据表：

services

字段：

name

default_price

duration

status

功能：

新增

编辑

删除

---

# 预约管理

数据表：

appointments

关联：

customers

services

technicians

列表显示：

预约时间

客户姓名

服务项目

技师

状态

预计金额

实际金额

---

# 状态

待到店

已到店

服务中

已完成

已取消

未到店

---

# 状态颜色

待到店 蓝色

已到店 绿色

服务中 紫色

已完成 灰色

已取消 红色

未到店 深红色

---

# 新增预约

字段：

客户

预约时间

服务项目（多选）

技师（多选）

预计金额

来源

备注

支持：

创建预约

编辑预约

删除预约

---

# 首页适配手机

底部导航：

首页

预约

客户

我的

---

# 数据来源

全部使用 Supabase

不要使用 Mock Data

不要生成假数据

所有 CRUD 操作直接连接 Supabase

---

# 代码要求

使用：

Server Components

TypeScript

Reusable Components

Form Validation

Loading States

Empty States

Error Handling

---

# 输出要求

生成完整项目结构

生成页面

生成 Supabase 数据访问层

生成 CRUD 页面

生成移动端UI

确保可以直接运行
