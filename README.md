+ 【个人翻译】W3c的 Decentralized Identifiers (DIDs) v1.1 Core architecture, data model, and representations W3C Editor's Draft 07 July 2024
  + [pdf格式文件](https://github.com/HanHai-Space/Decentralized-Identifiers-DIDs-v1.1-Draft-07-July-2024-ZH/blob/master/docs/index.pdf)
  + [md格式文件](https://github.com/HanHai-Space/Decentralized-Identifiers-DIDs-v1.1-Draft-07-July-2024-ZH/blob/master/docs/index.md)


---

#  摘要

去中心化标识符（DID）是一种新型标识符，支持可验证的、去中心化的数字身份。一个 DID 可以标识由 DID 控制者决定的任何主题（例如个人、组织、事物、数据模型、抽象实体等）。与典型的联合标识符相比，DIDs的设计使其分离于集中式注册表、身份提供者以及证书颁发机。具体来说，虽然可借助第三方协助发现与DID相关的信息，但该设计允许DID控制者无需任何第三方授权的情况下即可证明对其的控制。DIDs 是将 DID 主题与DID 文档相关联的URIs，允许与该主题相关联的可信交互每个 DID 文档都可以表达加密材料、验证方法或服务，提供了一组让DID控制者能够证明对 DID 控制的机制。服务可实现与 DID 主题相关的可信交互。如果 DID 主题是数据模型等信息资源，则 DID 可提供返回 DID 主题本身的方法。本文档规定了 DID 语法、通用数据模型、核心属性、序列化表示、DID 操作，并解释了将 DID 解析为其所代表的资源的过程。