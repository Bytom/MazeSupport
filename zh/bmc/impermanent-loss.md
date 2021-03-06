## 无常损失详解

### 什么是无常损失？

在进行流动性挖矿时会碰到的一种损失。这种损失是由于代币价格背离引起的。当价格回归时，这种损失也就没有了。我们这里说的是损失，不等同亏损。当我们把一对代币存入交易池后，如果一种代币价格有上升或下降，那么在价格变化后你把他们取出，得到的总价格比直接手握这两种代币要低一些，低的这一部分就是损失，价格偏离越大损失就越大，所以可能造成亏损。

### 为什么会有无常损失？

让我们通过一个案例，说明流动性提供者的无常损失是如何产生的。

用户Alice在流动资金池中存入了1 ETH和100 DAI。在对应自动做市商（AMM）机制中，要求存入数字货币的资金对必须具有同等价值。这意味着在存款时，1ETH价格=100 DAI。那么此时，Alice存款时资产价值为200美元。

此外，资金池中总共有10 ETH及1,000 DAI，由其他流动性提供者像Alice一样出资。因此，Alice在资金池中占有10％的份额，总流动资金为10,000美元。

假设ETH的价格上涨到400 DAI。在这种情况下，套利交易者会将DAI添加到池中并从池中移除ETH，直到比率反映市场价格。请注意，自动做市商机制是不存在订单簿的，决定池中资产价格的是池中资产之间的比率。尽管池中的流动性保持不变（即10,000），但池中资产数字资产的比率却发生了变化。

如果当前1 ETH=400 DAI，那么池中ETH数量和DAI的比率已更改。由于套利交易者的操作，现在流动池内有5 ETH和2,000 DAI。

如果Alice决定提现资金，如我们先前所知，她有权获得10％的份额。因此她可以提取0.5 ETH和200 DAI，总计400 美元。自从她存放了价值200美元的代币以来，她获得了可观的利润，对吗？但是如果她不做流动性提供者而是只是持有1 ETH和100 DAI，会发生什么？她可以获得500美元。

在这样的情况下，持币比存入资产注入流动性而会获益更高。这就是我们所说的无常损失。

虽然在上述案例下Alice的损失并不多，且她的初始存款金额相对较小。但是请记住，无常损失可能会导致重大损失（甚至包括大部分初始存款）。

虽然如此，我们上述的案例忽略了Alice提供流动性可获得的交易费用。在很多情况下，用户赚取手续费可能会抵消损失，并使提供流动性仍然可获利。