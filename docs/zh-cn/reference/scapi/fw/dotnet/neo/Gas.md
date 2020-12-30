# GAS 类

提供了原生合约GasToken的一系列属性与方法，合约哈希为`0xa6a6c15dcdc9b997dac448b6926522d22efeedfb`。

命名空间：[Neo.SmartContract.Framework.Services.Neo](../neo.md)

程序集：Neo.SmartContract.Framework

## 语法

```c#
public class GAS
```

## 属性

| 名称              | 说明                                                         |
| ----------------- | ------------------------------------------------------------ |
| Hash              | 获取合约哈希                                            |
| Symbol           | 获取符号, 即: gas                                           |
| Decimals          | 获取精度                                   |

## 方法

| 名称                                                         | 说明                                                         |
| ------------------------------------------------------------ | ------------------------------------------------------------ |
| [TotalSupply()](Gas/TotalSupply.md)          | 获取GAS总发行量                                     |
| [BalanceOf(UInt160 account)](Gas/BalanceOf.md)             | 获取余额                                       |
| [Transfer(UInt160 from, UInt160 to, BigInteger amount)](Gas/Transfer.md) | 转账                                     |