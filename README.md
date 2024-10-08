<center><h1>介绍</h1></center>

【个人翻译】W3C的 《`Decentralized Identifiers (DIDs) v1.1 Core architecture, data model, and representations W3C Editor's Draft 27 August 2024`》



+ 原文链接: https://w3c.github.io/did-core/

+ 文件

  + [pdf格式文件](https://github.com/HanHai-Space/Decentralized-Identifiers-DIDs-v1.1-Draft-07-July-2024-ZH/blob/master/docs/index.pdf)

  + [md格式文件](https://github.com/HanHai-Space/Decentralized-Identifiers-DIDs-v1.1-Draft-07-July-2024-ZH/blob/master/docs/index.md)



<center><h1>摘要</h1></center>

[Decentralized identifiers](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) (DIDs) are a new type of identifier that enables verifiable, decentralized digital identity. A [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) refers to any subject (e.g., a person, organization, thing, data model, abstract entity, etc.) as determined by the controller of the [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers). In contrast to typical, federated identifiers, [DIDs](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) have been designed so that they may be decoupled from centralized registries, identity providers, and certificate authorities. Specifically, while other parties might be used to help enable the discovery of information related to a [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers), the design enables the controller of a [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) to prove control over it without requiring permission from any other party. [DIDs](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) are [URIs](https://w3c.github.io/did-core/#dfn-uri) that associate a [DID subject](https://w3c.github.io/did-core/#dfn-did-subjects) with a [DID document](https://w3c.github.io/did-core/#dfn-did-documents) allowing trustable interactions associated with that subject.

Each [DID document](https://w3c.github.io/did-core/#dfn-did-documents) can express cryptographic material, [verification methods](https://w3c.github.io/did-core/#dfn-verification-method), or [services](https://w3c.github.io/did-core/#dfn-service), which provide a set of mechanisms enabling a [DID controller](https://w3c.github.io/did-core/#dfn-did-controllers) to prove control of the [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers). [Services](https://w3c.github.io/did-core/#dfn-service) enable trusted interactions associated with the [DID subject](https://w3c.github.io/did-core/#dfn-did-subjects). A [DID](https://w3c.github.io/did-core/#dfn-decentralized-identifiers) might provide the means to return the [DID subject](https://w3c.github.io/did-core/#dfn-did-subjects) itself, if the [DID subject](https://w3c.github.io/did-core/#dfn-did-subjects) is an information resource such as a data model.

This document specifies the DID syntax, a common data model, core properties, serialized representations, DID operations, and an explanation of the process of resolving DIDs to the resources that they represent.



去中心化标识符（DID）是一种新型标识符，支持可验证的、去中心化的数字身份。一个 DID 可以标识由 DID 控制者决定的任何主题（例如个人、组织、事物、数据模型、抽象实体等）。与典型的联合标识符相比，DIDs的设计使其分离于集中式注册表、身份提供者以及证书颁发机。具体来说，虽然可借助第三方协助发现与DID相关的信息，但该设计允许DID控制者无需任何第三方授权的情况下即可证明对其的控制。DIDs 是将 DID 主题与DID 文档相关联的URIs，允许与该主题相关联的可信交互。

每个 DID 文档都可以表达加密材料、验证方法或服务，提供了一组让DID控制者能够证明对 DID 控制的机制。服务可实现与 DID 主题相关的可信交互。如果 DID 主题是数据模型等信息资源，则 DID 可提供返回 DID 主题本身的方法。

本文档规定了 DID 语法、通用数据模型、核心属性、序列化表示、DID 操作，并解释了将 DID 解析为其所代表的资源的过程。