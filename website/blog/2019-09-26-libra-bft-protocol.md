---
author: Mathieu Baudet, Calibra
title: 改进LibraBFT协议
---
<script>
    let items = document.getElementsByClassName("post-meta");   
    for (var i = items.length - 1; i >= 0; i--) {
        if (items[i].innerHTML = '<p class="post-meta">August 14, 2019</p>') items[i].innerHTML = '<p class="post-meta">September 26, 2019</p>';
    }
</script>

We are happy to announce a new release of the [LibraBFT technical report](https://developers.libra.org/docs/state-machine-replication-paper).

我们很高兴宣布[LibraBFT技术报告](https://developers.libra.org/docs/state-machine-replication-paper)的新版本。

The LibraBFT protocol operates at the heart of the Libra blockchain to guarantee secure state machine replication. The new version of the protocol, LibraBFTv2, includes several optimizations that were designed to reduce networking and improve commit latency of the Libra blockchain.

LibraBFT协议在Libra区块链的核心运行，以确保安全的状态机复制。该协议的新版本LibraBFTv2包含多项优化，旨在减少联网并改善Libra区块链的提交延迟。

Together with this release, we are happy to make available the code of the Rust simulator used as a reference in the LibraBFT report. This code can be found in the [github repository](https://github.com/calibra/research) of the research team of Calibra.

与此版本一起，我们很高兴在LibraBFT报告中提供Rust模拟器的代码作为参考。可以在Calibra研究团队的[github存储库](https://github.com/calibra/research)中找到此代码。

### Reducing network complexity in practice

LibraBFT is a refinement of the HotStuff protocol that makes explicit the mechanisms used to achieve round synchronization between nodes. Informally, a round is a period of time where a specific leader is trusted to drive progress --- typically by proposing a block (B), gathering votes (V), and broadcasting a quorum certificate (C) (see picture below). Round synchronization aims at making nodes eventually execute the same round with sufficiently long overlap so that the leader of this round can succeed.

LibraBFT是HotStuff协议的改进，它明确说明了用于在节点之间实现轮次同步的机制。非正式地说，回合是一段时期，在此期间，可以信任特定的领导者来推动进度 - 通常通过提议一个区块（B），收集选票（V）和广播法定人数证书（C）（请参见下图）。回合同步旨在使节点最终以足够长的重叠执行同一回合，以便此回合的领导者可以成功。

![](https://libra.org/wp-content/uploads/2019/09/libraBFT2.png)

In the optimistic case (aka "happy path"), *LibraBFTv2 reduces the
overhead of round synchronization to a single message per node per
round* (see green arrows in the picture).

在乐观的情况下（也称为“幸福之路”），*LibraBFTv2会减少将每个节点每个节点的循环同步到单个消息的开销圆形*（请参阅图片中的绿色箭头）。

The initial "v1" version of LibraBFT relied on probabilistic gossip to ensure uniform propagation of quorum certificates (C). This uniform propagation was needed to achieve round synchronization and guarantee liveness in presence of malicious leaders. While probabilistic gossip is a popular technique suitable to many applications, it typically requires a non-linear number of messages and causes increased latency due to the intermediate hops. From an engineering point of view, the network overhead and the probabilistic nature of gossiping may also complicate debugging.

LibraBFT的初始“v1”版本依靠概率性八卦来确保仲裁证书（C）的均匀传播。需要这种统一的传播来实现全面同步，并在恶意领导者在场的情况下保证生命力。尽管概率性八卦是一种适用于许多应用程序的流行技术，但它通常需要非线性消息数量，并且由于中间跃点而导致延迟增加。从工程角度来看，网络开销和闲聊的概率性质也可能使调试复杂化。

In contrast, LibraBFTv2 achieves round synchronization in a different way, without using probabilistic gossip. First, the new protocol introduces a new type of failsafe mechanisms that regularly pull missing data in case no progress is made. Second, LibraBFTv2 simplifies the constraints on block proposals. The new constraints ensure that an honest leader can always propose a block and force round synchronization soon after the first honest node enters her round.

相反，LibraBFTv2以不同的方式实现了轮次同步，而无需使用概率八卦。首先，新协议引入了一种新型的故障安全机制，该机制会在未取得任何进展的情况下定期提取丢失的数据。其次，LibraBFTv2简化了对提案提案的约束。新的约束条件确保诚实的领导者始终可以在第一个诚实节点进入其回合后立即提出阻止并强制回合同步。

The proof of liveness of LibraBFTv2 shows that the new protocol still performs in a satisfying way under Byzantine (worst-case) scenarios, while the number of messages is now linear in the best case.

LibraBFTv2的活跃性证明表明，在拜占庭（最坏情况）方案下，新协议仍然可以令人满意地执行，而在最佳情况下，消息数量现在是线性的。

### What's next

We expect new releases of the LibraBFT report to continue in the future as the research and the engineering teams of Calibra keep improving the theoretical analysis and the implementation of the LibraBFT protocol.

Stay tuned!

我们期望LibraBFT报告的新版本将在未来继续，因为Calibra的研究和工程团队将继续改善理论分析和LibraBFT协议的实施。

敬请关注！
