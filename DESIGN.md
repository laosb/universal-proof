# 通用互联网实体验证设计

## 概述

基于 PGP 算法构建的去中心化信任系统。

## 概念

### Proof 证明

*n.* 一段 PGP 签名的电子数据，内含一段 JSON，用于证明特定公匙所属实体与 JSON 内描述的某个实体的联系。

### Proof Pattern 证明模式

*n.* 定义了内含证明的公开电子文档被认为有效的条件，格式为 JSON。包含以下信息：

* `proof_location` *证明*在电子文档中的位置
* `id_location` *证明*中 JSON 内描述的实体的唯一识别码在电子文档中的位置
* `doc_location` 电子文档公开的位置，此位置上仅能由该实体在该站点上创建

