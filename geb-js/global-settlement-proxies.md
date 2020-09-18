---
description: >-
  Proxy functions meant to facilitate collateral redemption during Global
  Settlement
---

# Global Settlement Proxies

Convenience class used to call functions from [GebProxyActionsGlobalSettlement](https://github.com/reflexer-labs/geb-proxy-actions/blob/master/src/GebProxyActions.sol) using a proxy registered in the [GebProxyRegistry](https://github.com/reflexer-labs/geb-proxy-registry/blob/master/src/GebProxyRegistry.sol). Useful only during Global Settlement in order for users to redeem collateral.

## Constructors

+ **new GebProxyActionsGlobalSettlement**\(`proxyAddress`: string, `network`: GebDeployment, `chainProvider`: GebProviderInterface\): [_GebProxyActionsGlobalSettlement_](global-settlement-proxies.md)

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:32_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L32)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `proxyAddress` | string |
| `network` | GebDeployment |
| `chainProvider` | GebProviderInterface |

**Returns:** [_GebProxyActionsGlobalSettlement_](global-settlement-proxies.md)

## Properties

### address

• **address**: _string_

_Inherited from_ [_GebProxyActions_](safe-proxies.md)_._[_address_](safe-proxies.md#address)

Defined in packages/geb-contract-base/lib/base-contract-api.d.ts:19

### chainProvider

• **chainProvider**: _GebProviderInterface_

_Inherited from_ [_GebProxyActions_](safe-proxies.md)_._[_chainProvider_](safe-proxies.md#chainprovider)

Defined in packages/geb-contract-base/lib/base-contract-api.d.ts:20

### proxy

• **proxy**: _DsProxy_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:26_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L26)

Underlying proxy object. Can be used to make custom calls to the proxy using `proxy.execute()`.

### proxyActionAddress

• **proxyActionAddress**: _string_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:31_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L31)

Address of the proxy actions global settlement contract.

### proxyAddress

• **proxyAddress**: _string_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:38_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L38)

Address of the underlying proxy.

## Methods

### coinJoin\_join

▸ **coinJoin\_join**\(`apt`: string, `safeHandler`: string, `wad`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:64_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L64)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `apt` | string |
| `safeHandler` | string |
| `wad` | BigNumberish |

**Returns:** _TransactionRequest_

### freeETH

▸ **freeETH**\(`ethJoin`: string, `globalSettlement`: string, `safe`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:75_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L75)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `ethJoin` | string |
| `globalSettlement` | string |
| `safe` | BigNumberish |

**Returns:** _TransactionRequest_

### freeTokenCollateral

▸ **freeTokenCollateral**\(`collateralJoin`: string, `safe`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:91_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L91)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `collateralJoin` | string |
| `safe` | BigNumberish |

**Returns:** _TransactionRequest_

### prepareCoinsForRedeeming

▸ **prepareCoinsForRedeeming**\(`wad`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:106_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L106)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `wad` | BigNumberish |

**Returns:** _TransactionRequest_

### redeemETH

▸ **redeemETH**\(`ethJoin`: string, `collateralType`: BytesLike, `wad`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:117_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L117)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `ethJoin` | string |
| `collateralType` | BytesLike |
| `wad` | BigNumberish |

**Returns:** _TransactionRequest_

### redeemTokenCollateral

▸ **redeemTokenCollateral**\(`collateralJoin`: string, `collateralType`: BytesLike, `wad`: BigNumberish\): _TransactionRequest_

_Defined in_ [_packages/geb/src/proxy-action-global-settlement.ts:133_](https://github.com/reflexer-labs/geb.js/blob/31f836f/packages/geb/src/proxy-action-global-settlement.ts#L133)

**Parameters:**

| Name | Type |
| :--- | :--- |
| `collateralJoin` | string |
| `collateralType` | BytesLike |
| `wad` | BigNumberish |

**Returns:** _TransactionRequest_
