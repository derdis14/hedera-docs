# TokenDelete

Marks a token as deleted, though it will remain in the ledger.

The operation must be signed by the specified Admin Key of the Token. If admin key is not set, Transaction will result in TOKEN\_IS\_IMMUTABlE.

Once deleted update, mint, burn, wipe, freeze, unfreeze, grant kyc, revoke kyc and token transfer transactions will resolve to TOKEN\_WAS\_DELETED.

## TokenDeleteTransactionBody

| Field | Type | Description |
| :--- | :--- | :--- |
| `token` | [TokenID](../basic-types/tokenid.md) | The token to be deleted. If invalid token is specified, transaction will result in INVALID\_TOKEN\_ID |

