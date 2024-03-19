# Type alias: ExtractFunction`<Schema>`

> **ExtractFunction**\<`Schema`\>: (`params`, `context`?) => `Promise`\<`z.infer`\<`Schema`\>\>

## Type parameters

| Parameter |
| :------ |
| `Schema` extends `z.ZodObject`\<`any`\> |

A function used to extract data using OpenAI function calling.

## Parameters

| Parameter | Type |
| :------ | :------ |
| `params` | `string` \| [`Params`](../namespaces/Runner/type-aliases/Params.md) |
| `context`? | [`Ctx`](../../Model/type-aliases/Ctx.md) |

## Returns

`Promise`\<`z.infer`\<`Schema`\>\>

## Source

[src/prompt/types.ts:48](https://github.com/colelawrence/dexter/blob/6b94c49/src/prompt/types.ts#L48)
