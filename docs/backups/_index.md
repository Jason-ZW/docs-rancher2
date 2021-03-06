---
title: 备份和恢复
description: 本节专门介绍在灾难情况下保护您的数据。为了保护自己免受灾难情况的影响，应定期创建备份。
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
  - 备份和恢复指南
  - 备份和恢复
---

本节专门介绍在灾难情况下保护您的数据。

为了保护自己免受灾难情况的影响，应定期创建备份。

- 备份 Rancher Server：
  - [基于 K3s 的 Rancher 高可用](/docs/backups/backups/k3s-backups/_index)
  - [基于 RKE 的 Rancher 高可用](/docs/backups/backups/ha-backups/_index)
  - [Rancher 单节点](/docs/backups/backups/single-node-backups/_index)
- [备份 Rancher 创建的 Kubernetes 集群](/docs/cluster-admin/backing-up-etcd/_index)

在灾难场景中，可以通过恢复备份来恢复`etcd`的数据。

- [恢复 Rancher Server](/docs/backups/restorations/_index)
- [恢复 Rancher 创建的 Kubernetes 集群](/docs/cluster-admin/restoring-etcd/_index)
