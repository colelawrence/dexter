# Class: `abstract` AbstractDatastore`<DocMeta, Filter>`

## Extended By

- [`AbstractHybridDatastore`](AbstractHybridDatastore.md)
- [`PineconeDatastore`](PineconeDatastore.md)

## Type parameters

| Parameter |
| :------ |
| `DocMeta` extends [`BaseMeta`](../namespaces/Datastore/type-aliases/BaseMeta.md) |
| `Filter` extends [`BaseFilter`](../namespaces/Datastore/type-aliases/BaseFilter.md)\<`DocMeta`\> |

## Constructors

### new AbstractDatastore(args)

> **new AbstractDatastore**\<`DocMeta`, `Filter`\>(`args`): [`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `args` | [`Opts`](../namespaces/Datastore/interfaces/Opts.md)\<`DocMeta`, `Filter`\> |

#### Returns

[`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

#### Source

[src/datastore/datastore.ts:36](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L36)

## Properties

| Modifier | Property | Type | Description | Source |
| :------ | :------ | :------ | :------ | :------ |
| `abstract` | `datastoreProvider` | [`Provider`](../namespaces/Datastore/type-aliases/Provider.md) | - | [src/datastore/datastore.ts:26](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L26) |
| `abstract` | `datastoreType` | [`Type`](../namespaces/Datastore/type-aliases/Type.md) | - | [src/datastore/datastore.ts:25](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L25) |

## Methods

### addEvents()

> **addEvents**(`events`): [`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

Add event handlers to the datastore.

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `events` | [`Events`](../namespaces/Datastore/interfaces/Events.md)\<`DocMeta`, `Filter`\> |

#### Returns

[`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

#### Source

[src/datastore/datastore.ts:153](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L153)

***

### `abstract` delete()

> **`abstract`** **delete**(`docIds`): `Promise`\<`void`\>

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `docIds` | `string`[] |

#### Returns

`Promise`\<`void`\>

#### Source

[src/datastore/datastore.ts:22](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L22)

***

### `abstract` deleteAll()

> **`abstract`** **deleteAll**(): `Promise`\<`void`\>

#### Returns

`Promise`\<`void`\>

#### Source

[src/datastore/datastore.ts:23](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L23)

***

### getEvents()

> **getEvents**(): [`Events`](../namespaces/Datastore/interfaces/Events.md)\<`DocMeta`, `Filter`\>

Get the current event handlers

#### Returns

[`Events`](../namespaces/Datastore/interfaces/Events.md)\<`DocMeta`, `Filter`\>

#### Source

[src/datastore/datastore.ts:148](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L148)

***

### query()

> **query**(`query`, `context`?): `Promise`\<[`QueryResult`](../namespaces/Datastore/interfaces/QueryResult.md)\<`DocMeta`\>\>

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `query` | [`Query`](../namespaces/Datastore/interfaces/Query.md)\<`DocMeta`, `Filter`\> |
| `context`? | [`Ctx`](../namespaces/Datastore/type-aliases/Ctx.md) |

#### Returns

`Promise`\<[`QueryResult`](../namespaces/Datastore/interfaces/QueryResult.md)\<`DocMeta`\>\>

#### Source

[src/datastore/datastore.ts:53](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L53)

***

### setEvents()

> **setEvents**(`events`): [`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

Set the event handlers to a new set of events. Removes all existing event handlers.
Set to empty object `{}` to remove all events.

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `events` | [`Events`](../namespaces/Datastore/interfaces/Events.md)\<`DocMeta`, `Filter`\> |

#### Returns

[`AbstractDatastore`](AbstractDatastore.md)\<`DocMeta`, `Filter`\>

#### Source

[src/datastore/datastore.ts:162](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L162)

***

### `abstract` upsert()

> **`abstract`** **upsert**(`docs`, `context`?): `Promise`\<`void`\>

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `docs` | [`Doc`](../namespaces/Datastore/interfaces/Doc.md)\<`DocMeta`\>[] |
| `context`? | [`Ctx`](../namespaces/Datastore/type-aliases/Ctx.md) |

#### Returns

`Promise`\<`void`\>

#### Source

[src/datastore/datastore.ts:18](https://github.com/colelawrence/dexter/blob/6b94c49/src/datastore/datastore.ts#L18)
