# Interop Services

The NeoVM is a lightweight virtual machine focused on fast arithmetic and other basic operations, however Neo Blockchain has much more to offer on the Interoperability Layer (NeoContract).

The interop services are divided on two categories: Standard Services and Neo Services.

## Neo Services (Neo 2.x)


| Name                                 | Price    | Description                              | Inputs | Outputs |
|--------------------------------------|----------|------------------------------------------|--------|---------|
| `Neo.Runtime.GetTrigger`             |  1       |   |  |  |
| `Neo.Runtime.CheckWitness`           |  200     |   |  |  |
| `Neo.Runtime.Notify`                 |  1       |   |  |  |
| `Neo.Runtime.Log`                    |  1       |   |  |  |
| `Neo.Runtime.GetTime`                |  1       |   |  |  |
| `Neo.Runtime.Serialize`              |  1       |   |  |  |
| `Neo.Runtime.Deserialize`            |  1       |   |  |  |
| `Neo.Blockchain.GetHeight`           |   1 |   |  |  |
| `Neo.Blockchain.GetHeader`           |  100 |   |  |  |
| `Neo.Blockchain.GetBlock`            |   200 |   |  |  |
| `Neo.Blockchain.GetTransaction`      |   100 |   |  |  |
| `Neo.Blockchain.GetTransactionHeight`|   100 |   |  |  |
| `Neo.Blockchain.GetAccount`          |   100 |   |  |  |
| `Neo.Blockchain.GetValidators` |  200 |   |  |  |
| `Neo.Blockchain.GetAsset` |  100 |   |  |  |
| `Neo.Header.GetHash` |   1 |   |  |  |
| `Neo.Header.GetVersion` |   1 |   |  |  |
| `Neo.Header.GetPrevHash` |   1 |   |  |  |
| `Neo.Header.GetMerkleRoot` |   1 |   |  |  |
| `Neo.Header.GetTimestamp` |   1 |   |  |  |
| `Neo.Header.GetIndex` |   1 |   |  |  |
| `Neo.Header.GetConsensusData` |   1 |   |  |  |
| `Neo.Header.GetNextConsensus` |   1 |   |  |  |
| `Neo.Block.GetTransactionCount` |   1 |   |  |  |
| `Neo.Block.GetTransactions` |   1 |   |  |  |
| `Neo.Block.GetTransaction` |   1 |   |  |  |
| `Neo.Transaction.GetHash` |   1 |   |  |  |
| `Neo.Transaction.GetType` |   1 |   |  |  |
| `Neo.Transaction.GetAttributes` |   1 |   |  |  |
| `Neo.Transaction.GetInputs` |   1 |   |  |  |
| `Neo.Transaction.GetOutputs` |   1 |   |  |  |
| `Neo.Transaction.GetReferences` |   200 |   |  |  |
| `Neo.Transaction.GetUnspentCoins` |   200 |   |  |  |
| `Neo.Transaction.GetWitnesses` |   200 |   |  |  |
| `Neo.InvocationTransaction.GetScript` |   1 |   |  |  |
| `Neo.Witness.GetVerificationScript` |   100 |   |  |  |
| `Neo.Attribute.GetUsage` |   1 |   |  |  |
| `Neo.Attribute.GetData` |   1 |   |  |  |
| `Neo.Input.GetHash` |   1 |   |  |  |
| `Neo.Input.GetIndex` |   1 |   |  |  |
| `Neo.Output.GetAssetId` |   1 |   |  |  |
| `Neo.Output.GetValue` |   1 |   |  |  |
| `Neo.Output.GetScriptHash` |   1 |   |  |  |
| `Neo.Account.GetScriptHash` |   1 |   |  |  |
| `Neo.Account.GetVotes` |   1 |   |  |  |
| `Neo.Account.GetBalance` |   1 |   |  |  |
| `Neo.Account.IsStandard` |   100 |   |  |  |
| `Neo.Asset.Create` |   |  |  |   |
| `Neo.Asset.Renew` |   |  |  |   |
| `Neo.Asset.GetAssetId` |   1 |   |  |  |
| `Neo.Asset.GetAssetType` |   1 |   |  |  |
| `Neo.Asset.GetAmount` |   1 |   |  |  |
| `Neo.Asset.GetAvailable` |   1 |   |  |  |
| `Neo.Asset.GetPrecision` |   1 |   |  |  |
| `Neo.Asset.GetOwner` |   1 |   |  |  |
| `Neo.Asset.GetAdmin` |   1 |   |  |  |
| `Neo.Asset.GetIssuer` |   1 |   |  |  |
| `Neo.Contract.Create` |   |  |  |   |
| `Neo.Contract.Migrate` |   |  |  |   |
| `Neo.Contract.Destroy` |   1 |   |  |  |
| `Neo.Contract.GetScript` |   1 |   |  |  |
| `Neo.Contract.IsPayable` |   1 |   |  |  |
| `Neo.Contract.GetStorageContext` |   1 |   |  |  |
| `Neo.Storage.GetContext` |   1 |   |  |  |
| `Neo.Storage.GetReadOnlyContext` |   1 |   |  |  |
| `Neo.Storage.Get` |   100 |   |  |  |
| `Neo.Storage.Put` |   |  |  |   |
| `Neo.Storage.Delete` |   100 |   |  |  |
| `Neo.Storage.Find` |   1 |   |  |  |
| `Neo.StorageContext.AsReadOnly` |   1 |   |  |  |
| `Neo.Enumerator.Create` |   1 |   |  |  |
| `Neo.Enumerator.Next` |   1 |   |  |  |
| `Neo.Enumerator.Value` |   1 |   |  |  |
| `Neo.Enumerator.Concat` |   1 |   |  |  |
| `Neo.Iterator.Create` |   1 |   |  |  |
| `Neo.Iterator.Key` |   1 |   |  |  |
| `Neo.Iterator.Keys` |   1 |   |  |  |
| `Neo.Iterator.Values` |   1 |   |  |  |
| `Neo.Iterator.Concat` |   1 |   |  |  |
| `Neo.Iterator.Next` |  1 |   |  |  |
| `Neo.Iterator.Value` |  1 |   |  |  |


### Cross-Service Mappings (2.X)
| Neo Service | Standard Service | AntShares Service |
|-------------|------------------|-------------------|
| `Neo.Blockchain.GetContract` | `Standard.Blockchain.GetContract` | N.A. |





## Standard Services (Neo 2.x)

| Name                                 | Price    | Description                              | Inputs | Outputs |
|--------------------------------------|----------|------------------------------------------|--------|---------|
| `System.ExecutionEngine.GetScriptContainer` |   1|    |  |  |
| `System.ExecutionEngine.GetExecutingScriptHash` |   1|    |  |  |
| `System.ExecutionEngine.GetCallingScriptHash` |   1|    |  |  |
| `System.ExecutionEngine.GetEntryScriptHash` |   1|    |  |  |
| `System.Runtime.Platform` |   1|    |  |  |
| `System.Runtime.GetTrigger` |   1|    |  |  |
| `System.Runtime.CheckWitness` |   200|    |  |  |
| `System.Runtime.Notify` |   1|    |  |  |
| `System.Runtime.Log` |   1|    |  |  |
| `System.Runtime.GetTime` |   1|    |  |  |
| `System.Runtime.Serialize` |   1|    |  |  |
| `System.Runtime.Deserialize` |   1|    |  |  |
| `System.Blockchain.GetHeight` |   1|    |  |  |
| `System.Blockchain.GetHeader` |   100|    |  |  |
| `System.Blockchain.GetBlock` |   200|    |  |  |
| `System.Blockchain.GetTransaction` |   200|    |  |  |
| `System.Blockchain.GetTransactionHeight` |   100|    |  |  |
| `System.Blockchain.GetContract` | 100 | Passes contract scripthash and retrieves Contract (or null). | `UInt160` | `ContractState` as `InteropInterface` [C# Example](#blockchain_getcontract) |
| `System.Header.GetIndex` |   1|    |  |  |
| `System.Header.GetHash` |   1|    |  |  |
| `System.Header.GetPrevHash` |   1|    |  |  |
| `System.Header.GetTimestamp` |   1|    |  |  |
| `System.Block.GetTransactionCount` |   1|    |  |  |
| `System.Block.GetTransactions` |   1|    |  |  |
| `System.Block.GetTransaction`          |   1|    |  |  |
| `System.Transaction.GetHash`           |   1|    |  |  |
| `System.Contract.Destroy`              |   1|    |  |  |
| `System.Contract.GetStorageContext`    |   1|    |  |  |
| `System.Storage.GetContext`            |   1|    |  |  |
| `System.Storage.GetReadOnlyContext`    |   1|    |  |  |
| `System.Storage.Get`                   |   100|    |  |  |
| `System.Storage.Put`                   | * |    |  |  |
| `System.Storage.PutEx`                 | * |    |  |  |
| `System.Storage.Delete`                |   100|    |  |  |
| `System.StorageContext.AsReadOnly`     |   1|    |  |  |

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
