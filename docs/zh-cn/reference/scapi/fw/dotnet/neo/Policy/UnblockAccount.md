# UnblockAccount 方法

将指定账户解除黑名单。

命名空间：[Neo.SmartContract.Framework.Services.Neo](../../neo.md)

程序集：Neo.SmartContract.Framework

> [!Note]
>
> 需要验证委员会的多签。签名超过委员会数量的一半的向上取整即为有效，相应操作将被执行。

## 语法

```c#
public static extern bool UnblockAccount(UInt160 account);
```

参数：

- account: 待解除黑名单的账户脚本哈希

## 示例

```c#
public class Contract1 : SmartContract.Framework.SmartContract
{
    private static readonly UInt160 account = "NirHUAteaMr6CqWuAAMaEUScPcS3FDKebM".ToScriptHash();

    public static object Test()
    {
        bool result = Policy.UnblockAccount(account);
        return result;
    }
}
```

部署后，调用该合约，响应正文为：

```json
{
	"type":"Boolean",
	"value":"true"
}
```

响应说明：

- Boolean类型：true表示解除屏蔽地址成功。

- 其他：失败。

[返回上级](../Policy.md)
