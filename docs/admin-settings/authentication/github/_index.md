---
title: 对接 GitHub
description: 在使用 GitHub 的环境中，您可以配置 Rancher 允许使用 GitHub 凭据登录。先决条件：请阅读外部身份验证配置和用户主体。使用分配了`系统管理员`角色的本地用户（即本地主体）登录 Rancher。
keywords:
  - rancher 2.0中文文档
  - rancher 2.x 中文文档
  - rancher中文
  - rancher 2.0中文
  - rancher2
  - rancher教程
  - rancher中国
  - rancher 2.0
  - rancher2.0 中文教程
  - 系统管理员指南
  - 登录认证
  - 对接 GitHub
---

在使用 GitHub 的环境中，您可以配置 Rancher 允许使用 GitHub 凭据登录。

> **先决条件：** 请阅读[外部身份验证配置和用户主体](/docs/admin-settings/authentication/_index)

1.  使用分配了`系统管理员`角色的本地用户（即本地主体）登录 Rancher。

2.  在**全局**视图中，从主菜单中选择**安全 > 认证**。

3.  选择 **GitHub**。

4.  按照显示的说明**安装 GitHub 应用程序**。Rancher 将您重定向到 GitHub 以完成注册。

    > **什么是授权回调 URL？**
    >
    > 授权回调 URL 是用户开始使用您的应用程序的 URL（即初始屏幕显示）。
    >
    > 当您使用外部身份验证时，身份验证实际上不会在您的应用程序中进行。而是在外部进行身份验证（在本例中为 GitHub）。在此外部身份验证成功完成之后，授权回调 URL 是用户重新进入应用程序的位置。

5.  从 GitHub 中拷贝 **Client ID** 和 **Client Secret** 将它们粘贴在 Rancher 中。

    > **从哪里获取 Client ID 和 Client Secret?**
    >
    > 从 GitHub，选择 Settings > Developer Settings > OAuth Apps。此处有 Client ID 和 Client Secret。

6.  点击 **启用 GitHub 认证**.

7.  使用**访问控制**选项来配置用户授权范围.

    - **允许任何有效用户**

      不建议配置任何有效用户都可以访问 Rancher!

    - **允许集群，项目以及授权用户和组织的成员**

      添加为**集群成员**或**项目成员**的任何 GitHub 用户或组均可登录 Rancher。另外，可以添加 GitHub 用户或组到**授权用户和组织**列表中，从而使这些用户可以登录 Rancher。

    - **仅授权的用户和组织可以访问**

      只有添加到**授权的用户和组织**中的 GitHub 用户或组才能登录到 Rancher。

8.  点击**保存**。

**结果：**

- GitHub 身份验证已配置。
- 您已可以使用 GitHub 帐户（即外部主体）登录到 Rancher。
