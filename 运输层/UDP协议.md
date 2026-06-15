---
title: "UDP协议"
category: "运输层"
layer: "运输层"
type: "专题笔记"
status: "待补充"
tags:
  - "计算机网络"
  - "运输层"
  - "UDP"
aliases:
  - "UDP 协议"
整理日期: 2026-06-08
---

UDP 协议的复习线索见 [[最后一节课复习#DNS]]，章节入口见 [[运输层]]。

### UDP报文段格式
![image.png](https://raw.githubusercontent.com/infinitepwn/note_picbed/main/20260615231148163.png)
UDP报文的首部只有8B
包括源端口号，目的端口号，UDP长度(包括首部和数据)，校验和，都是16位

==UDP整个报文会交付给IP层，变成IP层的数据部分，IP报文段又会成为数据链路层的数据部分，换而言之，上层的报文会成为下层的数据部分==
![image.png](https://raw.githubusercontent.com/infinitepwn/note_picbed/main/20260615234221482.png)

## 特点

- UDP 无连接
- UDP 尽最大努力交付
- UDP 面向报文
- UDP 首部开销小
- UDP 适合 DNS、实时音视频等场景

### 差错检测
通过校验和实现差错检测
![image.png](https://raw.githubusercontent.com/infinitepwn/note_picbed/main/20260615232734918.png)

## 相关笔记
- [[运输层]]
- [[UDP用户数据报]]
- [[复用与分用]]
- [[最后一节课复习]]
