# Module: 3box-legacy

Load legacy 3Box profiles.

## Purpose

The`3box-legacy` module provides utility functions to load legacy 3Box profiles.

## Installation

```sh
npm install @self.id/3box-legacy
```

## Common use-cases

### Load a legacy 3Box profile as a Self.ID basic profile

```ts
import { getLegacy3BoxProfileAsBasicProfile } from '@self.id/3box-legacy'

async function getProfile() {
  // Ethereum address to load the profile of
  const address = '0x123efad...'
  return await getLegacy3BoxProfileAsBasicProfile(address)
}
```

## Functions

### getLegacy3BoxProfileAsBasicProfile

▸ **getLegacy3BoxProfileAsBasicProfile**(`address`): `Promise`<`BasicProfile` \| ``null``\>

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`BasicProfile` \| ``null``\>

___

### loadLegacy3BoxProfile

▸ **loadLegacy3BoxProfile**<`T`\>(`address`): `Promise`<`T` \| ``null``\>

#### Type parameters

| Name | Type |
| :------ | :------ |
| `T` | `Record`<`string`, `any`\> |

#### Parameters

| Name | Type |
| :------ | :------ |
| `address` | `string` |

#### Returns

`Promise`<`T` \| ``null``\>

___

### transformProfile

▸ `Const` **transformProfile**(`profile`): `BasicProfile`

#### Parameters

| Name | Type |
| :------ | :------ |
| `profile` | `Record`<`string`, `any`\> |

#### Returns

`BasicProfile`
