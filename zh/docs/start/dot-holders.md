# 领取KSM

如果你参加了DOT销售并获取了以太坊上的DOT，你可以领取相同数量的KSM。

确保在这个过程中使用你当时使用的以太坊密钥。

*注意：我们鼓励那些不想参与Kusama网络的DOT持有人把他们的KSM捐给社区。你可以通过水龙头实现捐赠。作为感谢你也许会收到一些有价值的东西！*

## 在 Kusama创世以前领取

如果在Kusama创世以前完成领取，你就可以在最初的网络启动时就拥有KSM。可以很轻易的通过领取KSM的Dapp来完成。

### 生成一个Kusama地址

如果你还没有的话，你需要先生成一个Kusama地址。参考[该页](./claims.md)。

### 用MyCrypto领取你的KSM

该Dapp会协助你从MyCrypto发送一笔转账。如果你保存DOT分配的密钥是储存在像Ledger Nano S或Trezor这样的硬件钱包中的，那么MyCrypto是一个很好的选择。当然它也支持使用私钥、助记词或者parity签名接口。

**注意**：下载并使用本地版本的MyCrypto将极大地提高安全性。请确保下载了适配你操作系统的最新版本。你总是可以在他们的[发布页面](https://github.com/MyCryptoHQ/MyCrypto/releases)上找到最新版的桌面客户端。

一旦你下载了MyCrypto并在本地（在一台被隔离的电脑上运行会最大化地增加安全性）运行，进入[领取用Dapp](https://claim.kusama.network)并从下拉菜单中选择`Claim on Ethereum (before genesis)` 。该Dapp会显示领取用合约的地址和ABI，并要求你输入你的Kusama地址。当你输入你的Kusama地址后，16进制编码后的公钥将会被显示。

**注意**: 如果你生成地址使用的是`subkey` ，那你应该已经获取了你的公钥。

Go to the MyCrypto application and click on "Interact with Contracts" under the Tools tab. Choose the Custom selection for the contract and copy the address and ABI of the Claims contract. The mainnet Claims contract address is `0x9a1B58399EdEBd0606420045fEa0347c24fB86c2`. Click `Access`.

从下拉菜单中选择`claim`函数并输入你想要用来领取KSM的那个拥有DOT分配额度的以太坊地址。一般来说这个地址应该是你准备用来发起交易的地址。例外是当你使用修订（amendment）密钥的情况。（如果这对你来说很陌生也不用担心）。

接着输入领取用Dapp输出给你的16进制编码的公钥。

使用`150000` 作为输入的gas上限，而不要选中`Automatically Calculate Gas Limit` 。你可以自由的选择gas价格，或者就使用默认值。你可以在[这里](https://www.ethgasstation.info/)看到网络的平均gas价格。

在MyCrypto中点击`Write`并使用你偏好的方式解锁钱包。之后点击"Sign Transaction"并最终把交易发送到网络中。

你可以点击链接以在Etherscan上查看你的交易。当交易被打包入块之后你就完成了你的KSM领取流程！当Kusama网络启动之后你就在自己的Kusama地址中拥有了KSM。

### Claiming your KSM with a web3 enabled wallet (ie, metamask)

**This section links out to an external third-party app. Please exercise caution if you choose to use a third-party app to make your claim!**

If you have access to a web3 enabled wallet, you can use [this app](http://m.maiziqianbao.net/eth/mapping), created by community members, to claim your KSM.

After inputting your Kusama address under "Mapping Account", click the "Map" button.

**NOTE**: Before signing the transaction in your wallet, ensure that the destination is the mainnet claims contract, `0x9a1B58399EdEBd0606420045fEa0347c24fB86c2`, and that the transaction data includes your eth wallet address, and the hex-encoded public key (which you can verify using the claims dapp). **Please exercise caution if you choose to use a third-party app to make your claim!**

After signing the transaction and broadcasting it, once the transaction is mined, you are finished! When the Kusama network starts you will already have the balance of KSM in your Kusama address.

## 在Kusama创世之后领取

这一部分的信息敬请期待Kusama网络的启动。
