# Storage.Put Method

Inserts a given value to the given key in the persistent storage.

Namespace: [Neo.SmartContract.Framework.Services.Neo](../../neo.md)

Assembly: Neo.SmartContract.Framework

## Syntax

```c#
Put(StorageContext context, byte[] key, ByteString value);
Put(StorageContext context, byte[] key, byte[] value);
Put(StorageContext context, byte[] key, BigInteger value);
Put(StorageContext context, ByteString key, ByteString value);
Put(StorageContext context, ByteString key, BigInteger value);
Put(StorageContext context, byte[] key, byte[] value, StorageFlags flags);
Put(StorageContext context, byte[] key, BigInteger value, StorageFlags flags);
Put(StorageContext context, ByteString key, BigInteger value, StorageFlags flags);
Put(StorageContext context, ByteString key, ByteString value, StorageFlags flags);
```

Parameters:

- context: Storage context as a [StorageContext](../StorageContext.md).
- key: Key as a byte array or string.
- value: Value as a byte array, Biginteger, or string.
- flag: StorageFlags type, representing a variable or constant in storage.


Return value: void.

## Example

```c#
public class Contract1 : SmartContract.Framework.SmartContract
{
    public static void Main()
    {
        byte[] key1 = new byte[] { 0 };
        string key2 = "aa";
        byte[] value1 = new byte[] { 1 };
        BigInteger value2 = new BigInteger("1");
        string value3 = "bb";
        Storage.Put(Storage.CurrentContext, key1, value1);
        Storage.Put(Storage.CurrentContext, key1, value2);
        Storage.Put(Storage.CurrentContext, key1, value3);
        Storage.Put(Storage.CurrentContext, key2, value1);
        Storage.Put(Storage.CurrentContext, key2, value2);
        Storage.Put(Storage.CurrentContext, key2, value3);
    }
}
```

[Back](../Storage.md)
