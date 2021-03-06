  **原文链接**：[http://how.bitshares.works/en/master/bts_holders/dex.html](http://how.bitshares.works/en/master/bts_holders/dex.html)
 
 **译者**：[https://github.com/b-t-s-1](b-t-s-1)
 
 **校对者**： 
  
***    

# 5. 去中心化交易所（DEX）

去中心化交易所（简称为DEX）允许直接交易在BitShares生态系统中交易的数字商品。

与传统的中心化交易所相比，去中心化交易所具有非常特殊的优势，我们希望在下面简要介绍其中的一些。虽然BitShares DEX附带了所有这些功能，但是读者和客户可以全部或部分地利用这些功能。

* **权利分离**:没有理由要求同一实体负责签发欠条和处理订单。在BitShares中，订单匹配由协议执行，协议不知道涉及的资产的含义。
* **全球统一订单簿**:由于BitShares是全球性的，任何拥有互联网访问权限的人都可以使用DEX进行交易。这使得全球的流动性成为去中心化交易的单一订单。
* **交易几乎任何东西**:BitShares DEX与资产无关。因此，你可以交易**任何**交易对。虽然有些货币对可能最终流动性较低，例如白银：黄金，其他货币对如美元：欧元交易的外汇将会出现大量交易。
* **无限制**:BitShares协议无法限制你的交易体验。
* **去中心化**:DEX在全球范围内分散。这不仅意味着没有单点故障，而且还意味着BitShares交易所全天候交易，因为它总是在某个时间点。
* **安全**:你的资金和交易采用行业级椭圆曲线加密技术进行保护。除非你允许，否则没有人能够获得你的资金。为了进一步加强安全性，我们允许客户设置托管和多签名方案。
* **快速**:与其他去中心化网络相比，BitShares DEX允许实时交易，并且仅受光速和行星大小的限制。
* **可证明的订单匹配算法**:BitShares DEX的独特之处在于可证明的订单匹配算法。给定一组订单，你将始终能够证明这些订单已正确匹配。
* **抵押智能货币**:BitShares的最大特点之一是它的智能货币，如bitUSD，bitEUR，bitCNY等。为方便起见，这些资产仅表示钱包中的美元，欧元，人民币等。这些数字代币与其承保的实物资产具有相同的价值。因此，这个钱包中的1美元价值1美元，可以兑换。任何这些代币都由BitShares的公司股票（BTS）作为抵押担保，并可以当前价格结算。

* 5.1. 交易
  - 5.1.1. 交易对
  - 5.1.2. 市场概况
  - 5.1.3. 市场
  - 5.1.4. 订购簿
  - 5.1.5. 交易
  - 5.1.6. 订单匹配
  - 5.1.7. 放置订单
  - 5.1.8. 费用
* 5.2. 卖空BitAssets
  - 5.2.1. 借款
  - 5.2.2. 追加保证金
  - 5.2.3. 清算
  - 5.2.4. 售卖
  - 5.2.5. 更新抵押品比率
  - 5.2.6. 覆盖
  - 5.2.7. 讨论
*  5.3. 保证金追加机制
  - 5.3.1. 什么是追加保证金？
  - 5.3.2. 如何计算清算价格？
  - 5.3.3. 如何计算抵押比率（CR）？
  - 5.3.4. 执行条件
    + 5.3.4.1. 保证金追加何时会发生？
      * 5.3.4.1.1. **SQPR of `1.1`**
      * [5.3.4.1.2. **SQPR of `1.5`**
    + 5.3.4.2. 讨论
    + 5.3.4.3. 保证金追加会以什么价格执行？
  - 5.3.5. 保证金追加仅在[清算价格 - SQPP]范围内执行

