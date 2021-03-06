# StdLib Class

Provides a series methods of the native contract `StdLib`, which contract hash is`0xacce6fd80d44e1796aa0c2c625e9e4e0ce39efc0`。

Namespace: [Neo.SmartContract.Framework.Services.Neo](../neo.md)

Assembly: Neo.SmartContract.Framework

## Syntax

```c#
public static class StdLib
```

## Attributes

| Name | Description            |
| ---- | ---------------------- |
| Hash | Gets the contract hash |

## Methods

| Name                                   | Description   |
| ---------------------------------------- | --------------- |
| Serialize(object source) | Serializes the object to byte array |
| Deserialize(ByteString source) | Deserializes the byte array to object |
| JsonSerialize(object obj) | Serializes the object to Json |
| JsonDeserialize(string json) | Deserializes the Json to object |
| Base64Decode(string input) | Decodes the Base64-encoded string into byte array |
| Base64Encode(ByteString input) | Encodes the byte array into Base64 string |
| Base58Decode(string input) | Decodes the Base58 encoded string into byte array |
| Base58Encode(ByteString input) | Encodes the byte array into Base58 string |
| Itoa | Converts the integer to string |
| Atoi(string value, int @base = 10) | Converts the string to integer |
