  **原文链接**：[http://how.bitshares.works/en/master/bts_holders/tokens/pm.html](http://how.bitshares.works/en/master/bts_holders/tokens/pm.html)
 
 **译者**：[https://github.com/b-t-s-1](b-t-s-1)
 
 **校对者**： 
  
***

2.6.预测市场
==========================

预测市场是一种专门的BitAsset，总债务和总抵押品总是相等的金额（尽管资产ID不同）。不能对预测市场资产执行追加保证金或强制结算。在预测事件解决后，预测市场由发行方全球结算，因此预测市场必须始终启用“global_settle”权限。全球结算或卖空预测市场资产的最高价格是1：1。

目录

* 创建
* 赌注
  - 投注正面结果
  - 投注负面结果
* 解决

 <table style="width: 750px;"><tbody>
    <tr>
        <td bgcolor="LightBlue">注意</td>
    </tr>
    <tr>
        <td bgcolor="MintCream">在下面，我们将预测市场正面结果解析为真实（即喂价1）和结果解析为假（即喂价0）</td>
    </tr>
</table>

如果下注结算为真（即喂价1），则可以结算PM资产，将抵押品释放给资产持有者。

相反，如果下注结算为假（即喂价0），那么那些在市场上卖出PM资产并做空的人就会获利，因为PM资产变得毫无价值。

2.6.1.创建
---------------

预测市场是自由交易的资产，可以与支持资产（可能是任何其他资产，包括BTS，USD，GOLD）以1：1的比例从市场借入。

2.6.2.投注
-------------

用户可以对正面结果或负面结果下注。我们在这里展示了它的工作原理。

### 2.6.2.1.投注正面结果


如果你确信该赌注将结算为正，那么你希望**持有**该特定PM资产，因为它允许你以1：1的比例结算它的抵押品。

为了获得这些代币，你可以以任何价格（0到1之间）为它们下订单并等待成交，或以市场价格购买。通过这种技术，用户可以预先定义购买股票的几率。

例如，如果你认为投注以80％的概率正面结果，你可以将你的买单价格放在0.8。如果赌注得到正面结果（价格为1），那么你可以以1结算你的股票并获得20％的利润。

如果你能以0.2的价格购买代币（即市场参与者认为它不太可能得到正面结果），那么你可以以80％的概率获得80％的利润。

在下注结束后，用户可以通过**结算**其借入头寸并取出抵押品来索取其利润：

* **CLI钱包中的结算**:

    `>>> settle_asset <account> <amount> <symbol> True`

* **从GUI钱包中借入**:
  将资产展示在帐户概览中时，可以使用结算按钮。

### 2.6.2.2投注负面结果


为了下注负面结果（下注结果为假并且价格为0），您需要**卖出**代币。为了得到它们，你应该**不要** 在市场上买它们，而是通过以1：1的比例支付抵押品从网络**借用**它们。

例如，在“PM.PRESIDENT2016”中，如果你想用“100k BTS”打赌一个负面结果，你可以通过向网络支付“100k BTS”来借用“100k PM.PRESIDENT2016”。

 <table style="width: 750px;"><tbody>
    <tr>
        <td bgcolor="LightBlue">注意</td>
    </tr>
    <tr>
        <td bgcolor="MintCream"> 由于PM资产在技术上可以被任何其他资产锚定，你可能需要支付USD（或其他任何东西）而不是BTS。</td>
    </tr>
</table>

一旦你借用了代币，就可以以0和1之间的任何价格出售它们。如果你认为负面结果的概率为20％，你应该考虑以0.2的价格出售你的代币。

如果下注消极结果（喂价为0），你的债务值“债务=数量*价格= 0 BTS”，你可以零成本收回抵押品，并通过以0.2的价格卖出获得20％的利润。相反，如果赌注得到正面结果并且你卖出了所有代币，则无法关闭借入头寸以兑换抵押品。但是，在市场上销售代币时，你的总损失减少了20％。

如果在投注结束时你还剩下一些代币，你当然可以部分关闭你的借入头寸并兑换相应比例抵押品。

* **从CLI钱包借入**:

    ` >>> borrow_asset <account> <amount> <PMsymbol> <1:1-amount> true`

* **从GUI钱包借入**:
  当然，也可以使用市场上的“借用x”按钮在**GUI/网络钱包**中借用资产。

![](http://how.bitshares.works/en/master/_images/pm-borrow-btn.png)

解决
-----------------

发行人或feed生产者需要为预测市场公布喂价。它本质上是一个全球结算，它将设置资产的参数，使资产持有人能够在投注结果（0或1）下结算。详细信息显示在指南pm-close-manual中（参考：*dev.bitshares.works* 资料）
