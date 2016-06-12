# dahu
答乎（个人版） = 分答 + 值乎


# 功能点


## 首页

未发现是什么排序规则，，点击查看问题详情

## 发现

分类：默认5个，选专业，科研圈，金融街，好工作，创业路上，更多（静态）（push state进入分类列表）

All列表（recommenders）：点击查看个人详情（如未登陆，登陆）

## 我的

- 个人信息编辑
- 个人信息显示
- 问我的问题列表，点击查看问题详情

如果个人页面不是自己，显示提问窗口

如果为登陆，跳转到发现页面

# 模型

## 问题

- 提问的人
- 回答的人
- 问题内容
- 语音回答地址
- 回复时间（timeago）
- 价值
- 听过的人数
- 超值次数
- 是否过期（默认否）

使用mongodb或redis的expire特性

## 用户信息

- 微信授权获得的信息
- 个人简介：我是xx，略懂yy
- 问题价格：10元
- 总收入
- 关注者（知乎导入的，目前无入口）

和我相关的3种问题列表

- 问我的问题总数：5
- 我问的问题
- 我听过的问题

## 分类

- id：6
- 名称：创业路上
- 是否为默认分类

## 账务


# 技术点

## 微信SDK

- 授权
- 分享（首页，发现，我的，问题详情）
- 微信支付（普通的订单，退款，企业付款零钱入账）

## 前端

- react
- redux
- raven for log

# 费用规则

## 首次提问

- 填写问题，支付，支付后，创建问题
- 过期退还（暂时不知是几天）

## 听

- 1元1次，知乎要分成(具体未知)
- 超值，增加分成比例(具体未知)


# URL

## 首页

https://www.zhihu.com/zhi/

https://www.zhihu.com/zhi/infinity/feeds

## 发现

发现首页

url = https://www.zhihu.com/zhi/people

https://www.zhihu.com/zhi/infinity/recommenders

分类列表

https://www.zhihu.com/zhi/domain/23/people

https://www.zhihu.com/zhi/infinity/domains

## 我的

主页

https://www.zhihu.com/zhi/people/723274547700178944

编辑用户信息

未知url

## 问题

创建问题

未知url

问题详情

https://www.zhihu.com/zhi/messages/725371862300766208

## 分类

## 账务
