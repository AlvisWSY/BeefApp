# Beef Ordering Platform

## 项目概述
本项目旨在构建一个跨平台的购物应用，用户可以在平台上购买商品（以牛肉为例），并支持用户之间的拼单功能。商家可以通过一个专用的网页后台管理商品、库存和订单。

该项目主要面向特定区域的商家和用户，目标是提供一个简单高效的在线购物与拼单体验。同时，该项目也被设计为一个可扩展的框架，未来可以根据需要调整以适应其他商品或服务。

## 项目目标
- 为用户提供便捷的在线购物体验，包括查看商品库存、价格，并支持单独购买和拼单。
- 实现拼单功能，包括公开拼单和私密拼单，支持团长管理订单分发。
- 提供商家一个后台管理系统，能够管理商品的上架、库存和订单。
- 系统支持多种支付方式（如二维码和 PayNow），并能在支付后自动更新订单状态。

## 功能需求

### 用户端功能
- **用户登录和注册**：支持用户使用邮箱或手机号注册和登录系统。
- **商品展示**：用户可以查看商品信息（如价格、库存、描述等），并选择商品加入购物车。
- **拼单功能**：
  - **公开拼单**：用户可以选择公开拼单，由系统自动选择团长。
  - **私密拼单**：用户可以创建私密拼单，并通过链接邀请其他用户参与拼单，同时手动指定团长。
- **订单支付**：支持用户通过二维码或 PayNow 进行支付，并在支付完成后更新订单状态。
- **订单管理**：用户可以查看历史订单，跟踪订单状态，并通过团长确认收货。

### 商家后台功能
- **商品管理**：商家可以上架、修改和删除商品，并设置商品的价格、库存和截止日期等。
- **订单管理**：商家可以查看并处理订单状态，确认付款后安排发货或自提。
- **拼单折扣**：商家可以为团长设置特定的折扣，吸引更多用户参与拼单。

### 共享功能
- **跨平台支持**：用户可以通过移动端（iOS 和 Android）或网页端进行下单，商家通过网页后台管理系统进行管理。
- **社交分享**：用户可以通过短信或社交平台分享拼单链接。
- **身份验证**：使用 JWT 进行用户身份验证，确保系统的安全性。

## 技术栈
### 前端
- **React**：用于构建网页端用户界面。
- **React Native**：用于构建移动端应用（iOS 和 Android）。
- **HTML/CSS/JavaScript**：网页端界面基础。
  
### 后端
- **Node.js + Express**：用于构建 API，处理用户请求、订单和支付管理。
- **MongoDB**：用于存储用户、商品、订单等信息。

### 其他
- **JWT**：用于用户身份验证，确保系统的安全性。
- **PayNow / QR Code 支付**：集成支付功能，支持用户在线支付。

## 未来扩展
- **框架化设计**：该平台被设计为一个通用框架，未来可以轻松地适应其他商家的需求和不同的商品类型。
- **多商家支持**：当前仅支持单一商家，未来可扩展为支持多个商家的平台。
- **内置通讯功能**：未来可能集成即时通讯功能，方便拼单成员内部沟通（待政府监管许可）。

## 结论
该项目为用户和商家提供了一个简单高效的购物与拼单平台，并通过灵活的框架设计为未来的扩展提供了便利。在开发过程中优先实现核心功能，后续再逐步扩展其他功能。
