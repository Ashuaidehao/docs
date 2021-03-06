# NameService 类

提供了原生合约 NameService 的一系列方法，合约哈希为 `0x7a8fcf0392cd625647907afa8e45cc66872b596b`。

NameService 同时也是NFT（Non-fungible token）合约，继承了NFT合约所有的属性和方法。

命名空间：[Neo.SmartContract.Framework.Services.Neo](../neo.md)

程序集：Neo.SmartContract.Framework

## 语法

```c#
public class NameService 
```

## 属性

| 名称     | 说明              |
| -------- | ----------------- |
| Hash     | 合约哈希          |
| Symbol   | 获取符号, 即: NNS |
| Decimals | 获取精度          |

## 方法

| 名称 | 说明 |
| ---- | ---- |
| [TotalSupply()](NameService/TotalSupply.md) | 获取 NNS 资产总发行量                                |
| [BalanceOf(UInt160 owner)](NameService/BalanceOf.md) | 获取某人持有的域名数量                         |
| [OwnerOf(string name)](NameService/OwnerOf.md) | 获取域名的所有人 |
| [Properties(string name)](NameService/Properties.md) | 获取域名的属性 |
| [Tokens()](NameService/Tokens.md) | 获取该合约内的所有域名 |
| [TokensOf(UInt160 owner)](NameService/TokensOf.md) | 获取某人持有的域名 |
| [Transfer(UInt160, string)](NameService/Transfer.md) | 转账                                     |
| [IsAvailable(string name)](NameService/IsAvailable.md) | 域名是否可用 |
| [Register(string name, UInt160 owner)](NameService/Register.md) | 注册域名 |
| [Renew(string name)](NameService/Renew.md) | 续费域名 |
| [SetAdmin(string name, UInt160 admin)](NameService/SetAdmin.md) | 设置域名管理员 |
| [SetRecord(string name, RecordType type, string data)](NameService/SetRecord.md) | 设置DNS记录 |
| [GetRecord(string name, RecordType type)](NameService/GetRecord.md) | 获取DNS记录 |
| [DeleteRecord(string name, RecordType type)](NameService/DeleteRecord.md) | 删除DNS记录 |
| [Resolve(string name, RecordType type)](NameService/Resolve.md) | DNS解析 |
| [GetPrice()](NameService/GetPrice.md) | 获取域名价格 |