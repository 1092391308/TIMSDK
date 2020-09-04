## 镜像下载

腾讯云分流下载地址： [DOWNLOAD](https://github-1252463788.cos.ap-shanghai.myqcloud.com/imsdk/TIMSDK.zip)

## TUIKit集成

<table >
  <tr>
    <th width="180px" style="text-align:center">功能模块</th>
    <th width="180px" style="text-align:center">平台</th>
    <th width="500px" style="text-align:center">文档链接</th>
  </tr>

  <tr >
​    <td rowspan='2' style="text-align:center">快速集成</td>
​    <td style="text-align:center">iOS</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37060">TUIKit-iOS快速集成</a></td>
  </tr>

  <tr>
​    <td style="text-align:center">Android</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37059">TUIKit-Android快速集成</a></td>
  </tr>

  <tr>
​    <td rowspan='2' style="text-align:center">快速搭建</td>
​    <td style="text-align:center">iOS</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37063">TUIKit-iOS快速搭建</a></td>
  </tr>

  <tr>
​    <td style="text-align:center">Android</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37062">TUIKit-Android快速搭建</a></td>
  </tr>

  <tr>
​    <td rowspan='2' style="text-align:center">修改界面样式</td>
​    <td style="text-align:center">iOS</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37065">TUIKit-iOS修改界面样式</a></td>

  </tr>

  <tr>
​    <td style="text-align:center">Android</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37064">TUIKit-Android修改界面样式</a></td>
  </tr>

  <tr>
​    <td rowspan='2' style="text-align:center">自定义消息</td>
​    <td style="text-align:center">iOS</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37067">TUIKit-iOS自定义消息</a></td>
  </tr>

  <tr>
​    <td style="text-align:center">Android</td>
​    <td style="text-align:center"><a href="https://cloud.tencent.com/document/product/269/37066">TUIKit-Android自定义消息</a></td>
  </tr>

</table>


## 接口升级

- [iOS v2 v3 v4](https://github.com/tencentyun/TIMSDK/wiki/iOS-IMSDK-%E6%8E%A5%E5%8F%A3%E5%8F%98%E5%8C%96%EF%BC%88v2---v3---v4%EF%BC%89)
- [Android v2 v3 v4](https://github.com/tencentyun/TIMSDK/wiki/Android-IMSDK-%E6%8E%A5%E5%8F%A3%E5%8F%98%E5%8C%96%EF%BC%88v2---v3---v4%EF%BC%89)
- [Windows v2 v4](https://github.com/tencentyun/TIMSDK/wiki/Windows-IMSDK-%E6%8E%A5%E5%8F%A3%E5%8F%98%E5%8C%96%EF%BC%88v2---v4%EF%BC%89)

## 问题反馈
- 为了更好的了解您使用TIMSDK所遇到的问题，方便快速有效定位解决TIMSDK问题，希望您按如下反馈指引反馈issue，方便我们尽快解决您的问题
- [TIMSDK issue反馈指引](https://github.com/tencentyun/TIMSDK/wiki/TIMSDK-issue%E6%9C%89%E6%95%88%E5%8F%8D%E9%A6%88%E6%A8%A1%E6%9D%BF)

## 精简版 5.0.102 @2020.09.04

### SDK

**通用变更点**

- 发布 Android & iOS 精简版 SDK
- 精简版 SDK 在原有标准版的基础上裁剪了好友和会话两项能力，并对部分业务逻辑做了优化，以实现更高的执行效率，更小的安装包增量。


## 标准版 4.9.1 @2020.07.24

### SDK

**通用变更点**

- 优化海外登录问题
- 修复部分海外地区文件上传失败问题
- 修复含@符号的帐号上传文件失败问题
- 修复 C2C 未读数偶现错误问题
- 修复会话 showName 偶现展示异常的问题
- 文件类型消息增加获取下载 url 的接口

**iOS 平台**

- 修复断网时获取 C2C 消息无回调问题

**Android 平台**

- 修复信令解析接口偶现崩溃问题
- 修复消息中获取离线推送信息偶现崩溃问题
- 修复 API2.0 getFriendApplicationList 接口无数据不回调问题以及 getGroupMembersInfo 接口传入非群成员不回调问题

**Windows 平台**

- 获取加入群组时增加群组的详细信息
- 修复小文件发不出去问题
- 修复日志上报的 6002 错误

### TUIKit & Demo

**iOS**

- 增加音视频离线通话的推送，并可以跳转到接听界面
- 优化自定义消息删除、撤回无效的问题
- 优化界面
- 音视频代码 swift -> oc，大幅减少第三方依赖库
- 支持 LiteAV_TRTC ，LiteAV_Professional 两种音视频依赖库 TUIKit pod 集成。

**Android**

- 优化 Demo 的离线推送，升级各厂商的推送 SDK 版本
- 增加音视频离线通话的推送，并可以跳转到接听界面
