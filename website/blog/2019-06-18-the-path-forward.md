---
author: Libra Engineering Team
title: Libra: 前进的道路
---

Today we are announcing the **Libra testnet**, a live demonstration of an early prototype of the technology behind [Libra](https://libra.org/) — a simple global currency and financial infrastructure that can empower billions of people.

**Libra Core** is the open-source implementation of the [Libra protocol](https://developers.libra.org/docs/the-libra-blockchain-paper) — the specification of how transactions are submitted, ordered, executed, and recorded within the Libra ecosystem. This is the first implementation of the Libra protocol and the [Move language](https://developers.libra.org/docs/move-paper). This post, the Libra developer website, and Libra Core are published by the [Libra Association](https://libra.org/en-us/non-profit-association), an independent, not-for-profit membership organization tasked with evolving the Libra ecosystem. 

### Design Philosophy

We designed the Libra Blockchain for security, scalability, and reliability, so consumers and businesses can depend on it from day one. In order to reach these goals in a reasonable time frame, we have made conservative choices initially, using well-understood technologies ranging from Merkle trees to pseudonymous transactions. However, we know that the needs of the Libra ecosystem will evolve over time, which motivates the creation of the Move language to provide flexibility for the blockchain. Together these approaches form the philosophy that has led to the design of a currency that is reserve-backed in order to minimize volatility, and a permissioned network that will transition to permissionless.

We know that, as of today, this technology can't meet every use case for every user. **But, this is just a starting point**. Because extensibility is baked into the heart of the Libra protocol, through hard work and a collaborative community effort, we are confident that the Libra ecosystem can fulfill the vision of becoming a financial infrastructure that empowers billions of people.

我们为安全性，可扩展性和可靠性设计了Libra区块链，因此消费者和企业从一开始就可以依赖它。为了在合理的时间范围内实现这些目标，我们首先采用了从Merkle树到假名交易等广为人知的技术，做出了一些保守的选择。但是，我们知道Libra生态系统的需求会随着时间的推移而发展，这会激发Move语言的创建，从而为区块链提供灵活性。这些方法共同构成了一种哲学，该哲学导致设计出一种以储备为基础的货币，以最大程度地减少波动，并建立一种可以过渡到无许可的许可网络。

我们知道，到今天为止，这项技术还不能满足每个用户的每一个用例。 **但是，这只是一个起点**。由于可扩展性通过艰苦的工作和社区的共同努力已融入了Libra协议的核心，因此我们有信心Libra的生态系统可以实现成为数十亿人的金融基础设施的愿景。

### A note About Versioning and protocol Evolution

**The Libra protocol and Libra Core APIs are not final**. As discussed above, one of the key tasks in evolving the prototype is formalizing the protocol and APIs. We welcome experimentation with the software in the testnet, but developers should expect that work may be required to publish applications using these APIs. As part of our regular communication, we will publish our progress toward stable APIs.

**Libra协议和Libra Core API并非最终版本**。 如上所述，演进原型的关键任务之一是规范协议和API。 我们欢迎对测试网中的软件进行试验，但是开发人员应该期望使用这些API发行应用程序可能需要做一些工作。 作为常规交流的一部分，我们将发布我们向稳定API的进展。

## Building the Libra Community

Over the past year, engineers from Facebook's Calibra team have designed an early prototype of Libra Core. The project is now being open sourced, and **governance of the project has transitioned to the Libra Association**.

在过去的一年中，Facebook Calibra团队的工程师设计了Libra Core的早期原型。该项目现在开源了，并且**该项目的管理权已转移给Libra协会**。

The Libra Core project aims to follow in the footsteps of many successful open-source projects that start with and are driven by a core set of developers. In this early phase, we’ve adopted a simple process focused on rapid development; however, we are dedicated to evolving this process as the technology matures and the association expands. We have asked Calibra to manage the day-to-day development of Libra Core over the coming months, readying it for launch. That said, we are looking to build a collaborative community around Libra and will transition to an open and more formal process for making development decisions prior to the launch of the network. **No single company — including Facebook or Calibra — will have the ability to determine the future evolution of the Libra Blockchain.**

Libra Core项目旨在跟随许多成功的开源项目的脚步，这些项目始于一组核心开发人员并由其驱动。在此早期阶段，我们采用了一个专注于快速发展的简单流程；但是，随着技术的成熟和协会的扩大，我们致力于发展这一过程。我们已要求Calibra在接下来的几个月中管理Libra Core的日常开发，为发布做准备。也就是说，我们正在寻求围绕天秤座的协作社区，并将过渡到一个开放且更正式的流程，以便在网络启动之前做出发展决定。 **没有任何一家公司（包括Facebook或Calibra）能够单独决定Libra区块链的未来发展。**

In order to meet the objectives of both maintaining the development velocity needed for launch and transitioning to open development, we are first beginning with a focus on **transparency**:

* Our code is open source, as will be the progress we make going forward.
* Discussions about the Libra ecosystem are moving to open locations, such as our [Discourse forum](https://libra.trydiscourse.com/) and GitHub issues. We look forward to collaborating on our plans, designs, and APIs.
* We will publish monthly updates on our progress and our upcoming plans.
* We will push a daily release of the testnet at 11 a.m. Pacific Time. Initially, this will reset the state of the testnet on each push. As the project stabilizes, we anticipate moving to a weekly cadence and preserving the content of the testnet at each release.

为了既保持启动所需的开发速度又过渡到开放式开发的目标，我们首先要着眼于“透明度”：

* 我们的代码是开源的，我们将不断取得进步。
* 有关天秤座生态系统的讨论正在转移到开放位置，例如我们的[Discourse论坛](https://libra.trydiscourse.com/)和GitHub问题。我们期待着在我们的计划，设计和API上进行合作。
* 我们将每月发布有关我们的进度和即将到来的计划的更新。
* 我们将在太平洋时间上午11点每天发布测试网。最初，这将在每次推送时重置测试网的状态。随着项目的稳定，我们希望每周进行一次脚步跟踪，并在每次发布时保留测试网的内容。

Over the coming months, we will continue to push forward a **framework for open development**:

* We will migrate to a fully open development model where all pull requests, issues, and design documents are developed publicly and collaboratively
* We are working on continuous integration, which will allow us to scale the management of pull requests.
* Association members will use the governance process to determine a framework for managing the development of the Libra Core software and the Libra protocol.

在接下来的几个月中，我们将继续推动**开放开发框架**：

* 我们将迁移到一个完全开放的开发模型，在该模型中，所有拉动请求，问题和设计文档都是公开和协作开发的
* 我们正在努力进行持续集成，这将使我们能够扩展对拉取请求的管理。
* 协会成员将使用治理过程来确定用于管理Libra Core软件和Libra协议开发的框架。

## **What's Next?**

Because this is an early prototype of our work, our focus so far has been building the core infrastructure behind the project. There is a long road ahead before the system is ready to launch. The project is under active development. In the coming months, you'll be able to see our progress and increasingly participate in creating the Libra ecosystem.

Below is a list of some major features we are hoping to implement this year, many of which are described in greater detail in our technical papers: 

因为这是我们工作的早期原型，所以到目前为止，我们的重点一直是构建项目背后的核心基础架构。在准备好启动系统之前，还有很长的路要走。该项目正在积极开发中。在接下来的几个月中，您将能够看到我们的进展，并越来越多地参与创建Libra生态系统。

下面列出了我们希望今年实现的一些主要功能，其中许多功能在我们的技术论文中进行了详细说明：

### Libra Core

* Addressing:
    * We will formalize a specification for sharing payment addresses on the Libra Blockchain.
* Clients:
    * APIs — These APIs should provide ergonomic methods to meet real-world use cases, such as submitting transactions, accessing blockchain data, and monitoring for incoming payments. Possible approaches could include encouraging the use of a library, which acts as a light client or encouraging the use of RPCs to communicate with a process that runs the client.
* Consensus:
    * Increasing resiliency against liveness attacks — One advantage of the LibraBFT framework is that the correctness of the protocol is concentrated to a single software component — this is work which we have already completed. We plan to improve our resiliency against attacks on the liveness of the protocol by applying techniques, such as using more robust leader election mechanisms and enhancing inter-validator communication to increase the spread of information within the network. We have done an initial exploration of these and other mechanisms in the [LibraBFT paper](https://developers.libra.org/docs/state-machine-replication-paper) and are working to finalize our approach.
    * We will investigate the use of efficient signature aggregation to reduce the size of quorum certificates.
    * Mechanized proofs — We plan to start using mechanized proofs to verify our tech report and protocol claims.
* Move modules:
    * We will build modules that:
        * Manage the validator set (including staking, key rotation, and adding/removing validators) and integrate it into other system components, such as networking and consensus.
        * Track the supply of Libra coins in the system and allow the association to mint and burn Libra coins to keep the supply synchronized with the real-world reserve assets.
    * We will implement the Libra Investment Tokens as a Move resource.
    * We will implement cold wallets and multisig wallets that allow Libra users and association members to add extra security for their Libra coin and Libra Investment Token holdings. 
* Networking:
    * Full Nodes — Validator APIs to support full nodes (nodes that have a full replica of the blockchain but do *not* participate in consensus). This feature allows for the creation of replicas that can support scaling access to the blockchain and the auditing of the correct execution of transactions.
    * Gossip — Gossip-based approach to inter-validator communication may be necessary as the number of validator nodes grows.
    * Bootstrapping / Discovery — In the initial prototype, we have included placeholder implementations for finding the current validator set and bootstrapping the network. These components will need to be more fully formed before launch.
* Robust testing of real-world scenarios:
    * We will perform thorough testing of real-world scenarios that are likely to come up in a production environment, as well as ones that we hope never happen but need to be prepared for. These tests will include situations such as denial-of-service attacks, protocol upgrades, and the compromise of over one-third of the validator network.
    * We will prioritize projects to increase the resilience of the appropriate part of our infrastructure — for example, increasing our ability to withstand denial-of-service attacks by allowing for multiple admission control instances, ensuring that we have appropriate incentives to prevent excessive usage of storage on the blockchain, or creating run books for protocol upgrades.
* Security:
    * We will apply the “trusted computing base” (TCB) philosophy to security. This approach means taking important parts of the Libra Core software and ensuring that they have a minimal set of dependencies. We've already started to go down this route by designing the validator software into discrete components. We will continue down this route, ensuring that the essential components of Libra Core are isolated. For example, this means ensuring that the module that signs votes in the consensus protocol should be isolated from less critical components.
* Serialization:
    * We currently use Protocol Buffers as a storage format for transactions. While we've thought out the security implications of this design (e.g., we designed the system with the fact that Protocol Buffer serialization is not canonical), we are considering if using the canonical serialization framework we've used in other parts of the system might better suit our needs.
* Storage:
    * Pruning — We will allow a node to configure the pruning of historical storage — validators may prune past data aggressively while other nodes might keep a full replica.
* Research:
    * We know that to fulfill the mission of enabling a financial infrastructure that empowers billions of people we will need to address currently unresolved research challenges. Key research challenges include defining the path toward permissionless, security, and the usability of the blockchain.


* 地址：
    * 我们将正式制定一个在Libra区块链上共享付款地址的规范。
* 客户：
    * API-这些API应该提供符合人体工学的方法来满足实际使用情况，例如提交交易，访问区块链数据以及监视收款。可能的方法可能包括鼓励使用充当轻客户端的库，或者鼓励使用RPC与运行客户端的进程进行通信。
* 共识：
    * 增强抵御实时攻击的弹性 — LibraBFT框架的一个优势是协议的正确性集中在单个软件组件上，这是我们已经完成的工作。我们计划通过应用技术（例如使用更强大的领导者选举机制并增强验证者之间的通信以增加信息在网络中的传播）来提高针对协议活动性攻击的弹性。我们已经在[LibraBFT论文](https://developers.libra.org/docs/state-machine-replication-paper)中对这些机制和其他机制进行了初步探索，并且正在努力确定我们的方法。
    * 我们将研究使用有效的签名聚合来减少法定证书的大小。
    * 机械化的证明 — 我们计划开始使用机械化的证明来验证我们的技术报告和协议声明。
* Move模块：
    * 我们将构建以下模块：
        * 管理验证程序集（包括放样，密钥轮换和添加/删除验证程序），并将其集成到其他系统组件中，例如联网和共识。
        * 跟踪系统中天秤座硬币的供应，并允许协会铸造和燃烧天秤座硬币，以使供应与现实世界的储备资产保持同步。
    * 我们将实现Libra投资令牌作为Move资源。
    * 我们将实施冷钱包和多签名钱包，使Libra用户和协会会员可以为其Libra代币和所持有的Libra投资令牌增加额外的安全性。
* 联网：
    * 全节点-支持全节点的验证器API（具有区块链完整副本但不参与共识的节点）。此功能允许创建副本，该副本可支持扩展对区块链的访问以及对事务的正确执行的审核。
    * 闲话-随着验证者节点数量的增加，基于闲话的验证器间通信方法可能是必需的。
    自举/发现—在初始原型中，我们包括占位符实现，用于查找当前的验证器集并自举网络。在启动之前，这些组件将需要更完整地形成。
* 真实场景的强大测试：
    * 我们将对生产环境中可能出现的真实场景以及我们希望永远不会发生但需要做好准备的场景进行彻底的测试。这些测试将包括诸如拒绝服务攻击，协议升级以及超过三分之一的验证器网络遭到破坏的情况。
    * 我们将确定项目的优先级，以提高基础架构适当部分的弹性，例如，通过允许多个准入控制实例来增强我们抵御拒绝服务攻击的能力，确保我们有适当的动机来防止过度使用存储在区块链上，或者为协议升级创建运行手册。
*安全性：
    * 我们将“可信计算基础”（TCB）理念应用于安全性。这种方法意味着需要使用Libra Core软件的重要部分，并确保它们具有最小的依赖关系集。通过将验证器软件设计为分立组件，我们已经开始走这条路。我们将继续这条路线，确保将Libra Core的基本组件隔离开。例如，这意味着要确保在共识协议中签署投票的模块应与不太重要的组件隔离。
* 序列化：
    * 我们目前使用协议缓冲区作为事务的存储格式。尽管我们已经考虑了这种设计的安全性（例如，我们在设计系统时考虑到协议缓冲区序列化不是规范的），但我们正在考虑是否使用我们在系统其他部分中使用的规范化序列化框架可能更适合我们的需求。
* 储存：
    * 修剪 - 我们将允许一个节点配置历史存储的修剪-验证者可以主动删除过去的数据，而其他节点则可以保留完整副本。
* 研究：
    * 我们知道，要实现使数十亿人拥有能力的金融基础设施成为使命，我们将需要应对当前尚未解决的研究挑战。关键的研究挑战包括定义通往无许可，安全性和区块链可用性的道路。

### Libra Protocol

* Right now, Libra Core's implementation is a defacto specification for the protocol. As we finalize the design, we plan to turn this into a formal specification for the protocol. This will allow for easier auditing, design discussion, and other implementations.

* 目前为止，Libra Core的实现是该协议事实上的规范。在完成设计时，我们计划将其转变为该协议的正式规范。这将使审核，设计讨论和其他实现更加容易。

### Move Language

* Events:
    * We will improve Move’s existing functionality for notifying clients about on-chain activity via events. We will expose a dedicated type for event streams, finalize the format of event access path, and add events for important system module events, such as validator set changes or minting/burning Libra.
* Generics and collections:
    * We will add parametric polymorphism with *kind* (resource or nonresource) constraints. This will allow us to write general-purpose business logic for managing resources (e.g., we can write a multisig wallet that can work for any kind of resource instead of only for Libra coin).
    * We will add container types, such as vectors and maps. Containers will greatly increase the expressivity of Move and are required to implement some core system modules (e.g., the validator-set module manages a collection of validators).
* Move developer experience:
    * We will improve the local development and testing experience for users of the Move intermediate representation (IR).
    * We will continue working on a format for specifying functional correctness properties of Move programs and an automated verification tool for Move bytecode. We will apply this pipeline to the core Move modules first, but design it with the intention of supporting verification of arbitrary user-defined specifications.
* Versioning:
    * We will design a versioning scheme for Move modules, resources, and transaction scripts. Currently, Move modules can never be upgraded or deleted. Sustainable software infrastructure must support updates and deletion.

* 活动：
    * 我们将改进Move的现有功能，以通过事件通知客户有关链上活动的信息。我们将公开事件流的专用类型，确定事件访问路径的格式，并为重要的系统模块事件添加事件，例如验证器集更改或铸造/刻录Libra。
* 泛型和集合：
    * 我们将添加带有*（资源或非资源）约束的参数多态性。这将使我们能够编写用于管理资源的通用业务逻辑（例如，我们可以编写可用于任何类型的资源而不是仅适用于Libra代币的多签名钱包）。
    * 我们将添加容器类型，例如矢量和地图。容器将大大提高Move的表现力，并且是实现某些核心系统模块所必需的（例如，验证程序集模块管理验证程序的集合）。
* 改善开发人员的经验：
    * 我们将为Move中间表示（IR）的用户改善本地开发和测试体验。
    * 我们将继续研究用于指定Move程序的功能正确性属性的格式以及用于Move字节码的自动验证工具。我们将首先将此管道应用到核心Move模块，但是设计它的目的是支持验证任意用户定义的规范。
* 版本：
    * 我们将为Move模块，资源和事务脚本设计一个版本控制方案。当前，Move模块永远无法升级或删除。可持续的软件基础架构必须支持更新和删除。
