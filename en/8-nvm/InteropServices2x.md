# Interop Services

The NeoVM is a lightweight virtual machine focused on fast arithmetic and other basic operations, however Neo Blockchain has much more to offer on the Interoperability Layer (NeoContract).

The interop services are divided on two categories: Standard Services and Neo Services.

## Interop Interfaces

Interoperable Interface for object type `X` is represented as `Interface<X>`, for simplicity.

Existing interfaces are currently used on Neo Blockchain (`2.x` and `3.x`):

| Interface                      | Protocol  | Description                                 |
|--------------------------------|-----------|---------------------------------------------|
| `Interface<ContractState>`     |`2.x`      | Information for a `Contract` in network     |



## Neo Services

(*) Price is only presented for Neo `2.x`, since after `3.x` it will be variable according to a Policy Native Contract.
Values presented in 10e-8 GAS. Some prices include `+var` notation, since they include a variable price after base price.

| Name                                 | Protocol  |Price (*) | Description                              | Inputs | Outputs |
|--------------------------------------|-----------|----------|------------------------------------------|--------|---------|
| `Neo.Runtime.GetTrigger`             |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Runtime.CheckWitness`           |`2.x`,`3.x`|  200     |   |  |  |
| `Neo.Runtime.Notify`                 |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Runtime.Log`                    |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Runtime.GetTime`                |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Runtime.Serialize`              |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Runtime.Deserialize`            |`2.x`,`3.x`|  1       |   |  |  |
| `Neo.Blockchain.GetHeight`           |`2.x`,`3.x`|   1 |   |  |  |
| `Neo.Blockchain.GetHeader`           |`2.x`,`3.x`|  100 |   |  |  |
| `Neo.Blockchain.GetBlock`            |`2.x`,`3.x`|   200 |   |  |  |
| `Neo.Blockchain.GetTransaction`      |`2.x`,`3.x`|   100 |   |  |  |
| `Neo.Blockchain.GetTransactionHeight`|`2.x`,`3.x`|   100 |   |  |  |
| `Neo.Blockchain.GetAccount`          |`2.x`,`3.x`|   100 |   |  |  |
| `Neo.Blockchain.GetValidators`       |`2.x`,`3.x`|  200 |   |  |  |
| `Neo.Blockchain.GetAsset`            |`2.x`      |  100 |   |  |  |
| `Neo.Header.GetHash`                 |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetVersion`              |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetPrevHash`             |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetMerkleRoot`           |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetTimestamp`            |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetIndex`                |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetConsensusData`        |`2.x`      |   1 |   |  |  |
| `Neo.Header.GetNextConsensus`        |`2.x`      |   1 |   |  |  |
| `Neo.Block.GetTransactionCount`      |`2.x`      |   1 |   |  |  |
| `Neo.Block.GetTransactions`          |`2.x`      |   1 |   |  |  |
| `Neo.Block.GetTransaction`           |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetHash`            |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetType`            |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetAttributes`      |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetInputs`          |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetOutputs`         |`2.x`      |   1 |   |  |  |
| `Neo.Transaction.GetReferences`      |`2.x`      |   200 |   |  |  |
| `Neo.Transaction.GetUnspentCoins`    |`2.x`      |   200 |   |  |  |
| `Neo.Transaction.GetWitnesses`       |`2.x`      |   200 |   |  |  |
| `Neo.InvocationTransaction.GetScript`|`2.x`      |   1 |   |  |  |
| `Neo.Witness.GetVerificationScript`  |`2.x`      |   100 |   |  |  |
| `Neo.Attribute.GetUsage`             |`2.x`      |   1 |   |  |  |
| `Neo.Attribute.GetData`              |`2.x`      |   1 |   |  |  |
| `Neo.Input.GetHash`                  |`2.x`      |   1 |   |  |  |
| `Neo.Input.GetIndex`                 |`2.x`      |   1 |   |  |  |
| `Neo.Output.GetAssetId`              |`2.x`      |   1 |   |  |  |
| `Neo.Output.GetValue`                |`2.x`      |   1 |   |  |  |
| `Neo.Output.GetScriptHash`           |`2.x`      |   1 |   |  |  |
| `Neo.Account.GetScriptHash`          |`2.x`      |   1 |   |  |  |
| `Neo.Account.GetVotes`               |`2.x`      |   1 |   |  |  |
| `Neo.Account.GetBalance`             |`2.x`      |   1 |   |  |  |
| `Neo.Account.IsStandard`             |`2.x`      |   100 |   |  |  |
| `Neo.Asset.Create`                   |`2.x`      |   |  |  |   |
| `Neo.Asset.Renew`                    |`2.x`      |   |  |  |   |
| `Neo.Asset.GetAssetId`               |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetAssetType`             |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetAmount`                |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetAvailable`             |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetPrecision`             |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetOwner`                 |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetAdmin`                 |`2.x`      |   1 |   |  |  |
| `Neo.Asset.GetIssuer`                |`2.x`      |   1 |   |  |  |
| `Neo.Contract.Create`                |`2.x`      |   |  |  |   |
| `Neo.Contract.Migrate`               |`2.x`      |   |  |  |   |
| `Neo.Contract.Destroy`               |`2.x`      |   1 |   |  |  |
| `Neo.Contract.GetScript`             |`2.x`      |   1 |   |  |  |
| `Neo.Contract.IsPayable`             |`2.x`      |   1 |   |  |  |
| `Neo.Contract.GetStorageContext`     |`2.x`      |   1 |   |  |  |
| `Neo.Storage.GetContext`             |`2.x`      |   1 |   |  |  |
| `Neo.Storage.GetReadOnlyContext`     |`2.x`      |   1 |   |  |  |
| `Neo.Storage.Get`                    |`2.x`      |   100 |   |  |  |
| `Neo.Storage.Put`                    |`2.x`      |   |  |  |   |
| `Neo.Storage.Delete`                 |`2.x`      |   100 |   |  |  |
| `Neo.Storage.Find`                   |`2.x`      |   1 |   |  |  |
| `Neo.StorageContext.AsReadOnly`      |`2.x`      |   1 |   |  |  |
| `Neo.Enumerator.Create`              |`2.x`      |   1 |   |  |  |
| `Neo.Enumerator.Next`                |`2.x`      |   1 |   |  |  |
| `Neo.Enumerator.Value`               |`2.x`      |   1 |   |  |  |
| `Neo.Enumerator.Concat`              |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Create`                |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Key`                   |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Keys`                  |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Values`                |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Concat`                |`2.x`      |   1 |   |  |  |
| `Neo.Iterator.Next`                  |`2.x`      |  1 |   |  |  |
| `Neo.Iterator.Value`                 |`2.x`      |  1 |   |  |  |






## Standard Services (Neo 2.x)

| Name                                        | Protocol  |Price (*) | Description                              | Inputs | Outputs |
|---------------------------------------------|-----------|----------|------------------------------------------|--------|---------|
| `System.ExecutionEngine.GetScriptContainer` |`2.x`      |   1|    |  |  |
| `System.ExecutionEngine.GetExecutingScriptHash` |`2.x`  |   1|    |  |  |
| `System.ExecutionEngine.GetCallingScriptHash` |`2.x`    |   1|    |  |  |
| `System.ExecutionEngine.GetEntryScriptHash` |`2.x`      |   1|    |  |  |
| `System.Runtime.Platform`                   |`2.x`      |   1|    |  |  |
| `System.Runtime.GetTrigger`                 |`2.x`      |   1|    |  |  |
| `System.Runtime.CheckWitness`               |`2.x`      |   200|    |  |  |
| `System.Runtime.Notify`                     |`2.x`      |   1|    |  |  |
| `System.Runtime.Log`                        |`2.x`      |   1|    |  |  |
| `System.Runtime.GetTime`                    |`2.x`      |   1|    |  |  |
| `System.Runtime.Serialize`                  |`2.x`      |   1|    |  |  |
| `System.Runtime.Deserialize`                |`2.x`      |   1|    |  |  |
| `System.Blockchain.GetHeight`               |`2.x`      |   1|    |  |  |
| `System.Blockchain.GetHeader`               |`2.x`      |   100|    |  |  |
| `System.Blockchain.GetBlock`                |`2.x`      |   200|    |  |  |
| `System.Blockchain.GetTransaction`          |`2.x`      |   200|    |  |  |
| `System.Blockchain.GetTransactionHeight`    |`2.x`      |   100|    |  |  |
| `System.Blockchain.GetContract`             |`2.x`      | 100 | Passes contract scripthash and retrieves Contract (or null). | `UInt160` | `Interface<ContractState>` [C# Example](#blockchain_getcontract) |
| `System.Header.GetIndex`                    |`2.x`      |   1|    |  |  |
| `System.Header.GetHash`                     |`2.x`      |   1|    |  |  |
| `System.Header.GetPrevHash`                 |`2.x`      |   1|    |  |  |
| `System.Header.GetTimestamp`                |`2.x`      |   1|    |  |  |
| `System.Block.GetTransactionCount`          |`2.x`      |   1|    |  |  |
| `System.Block.GetTransactions`              |`2.x`      |   1|    |  |  |
| `System.Block.GetTransaction`               |`2.x`      |   1|    |  |  |
| `System.Transaction.GetHash`                |`2.x`      |   1|    |  |  |
| `System.Contract.Destroy`                   |`2.x`      |   1|    |  |  |
| `System.Contract.GetStorageContext`         |`2.x`      |   1|    |  |  |
| `System.Storage.GetContext`                 |`2.x`      |   1|    |  |  |
| `System.Storage.GetReadOnlyContext`         |`2.x`      |   1|    |  |  |
| `System.Storage.Get`                        |`2.x`      |   100|    |  |  |
| `System.Storage.Put`                        |`2.x`      | * |    |  |  |
| `System.Storage.PutEx`                      |`2.x`      | * |    |  |  |
| `System.Storage.Delete`                     |`2.x`      |   100|    |  |  |
| `System.StorageContext.AsReadOnly`          |`2.x`      |   1|    |  |  |

### Cross-Service Mappings (2.X)
| Neo Service | Standard Service | AntShares Service |
|-------------|------------------|-------------------|
| `Neo.Blockchain.GetContract` | `Standard.Blockchain.GetContract` | N.A. |



## Coding Examples (C#)

### Blockchain_GetContract

```cs
using Neo.SmartContract.Framework.Services.Neo;
using Neo.SmartContract.Framework;
using Neo.VM;

namespace Neo.SmartContract {
    public static class HelperExternal {
        // INFO: InteropInterface result will be interpreted as Boolean
        [Syscall("Neo.Blockchain.GetContract")]
        public static extern bool GetContract(byte[] scripthash);
	}
    public class GetHelloWorld : Framework.SmartContract {
        static readonly byte[] ContractHelloWorld = "d741527ea66813c0c50e78bb403926b4c88a64c4".HexToBytes();

        public static bool Main() {
            bool contract = HelperExternal.GetContract(ContractHelloWorld);
            if(contract)
                Runtime.Notify("FOUND!");
            else
                Runtime.Notify("NOT FOUND!");

            return contract; // bool or InteropInterface
        }
    }
}
```
