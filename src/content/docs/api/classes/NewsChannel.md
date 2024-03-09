---
editUrl: false
next: false
prev: false
title: "NewsChannel"
---

## Extends

- `ObjectToLower`\<`APINewsChannel`\>.[`WebhookChannelMethods`](/api/classes/webhookchannelmethods/).[`BaseChannel`](/api/classes/basechannel/)\<`ChannelType.GuildAnnouncement`\>

## Constructors

### new NewsChannel(client, data)

```ts
new NewsChannel(client: BaseClient, data: APIChannelBase<ChannelType>): NewsChannel
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `client` | `BaseClient` |
| `data` | `APIChannelBase`\<`ChannelType`\> |

#### Returns

[`NewsChannel`](/api/classes/newschannel/)

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`constructor`](/api/classes/basechannel/#constructors)

#### Source

[seyfert/src/structures/channels.ts:48](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L48)

## Properties

| Property | Modifier | Type | Inherited from |
| :------ | :------ | :------ | :------ |
| `client` | `readonly` | [`UsingClient`](/api/interfaces/usingclient/) | [`BaseChannel`](/api/classes/basechannel/).`client` |
| `defaultAutoArchiveDuration` | `public` | `undefined` \| `ThreadAutoArchiveDuration` | `ObjectToLower.defaultAutoArchiveDuration` |
| `defaultThreadRateLimitPerUser` | `public` | `undefined` \| `number` | `ObjectToLower.defaultThreadRateLimitPerUser` |
| `flags` | `public` | `undefined` \| `ChannelFlags` | `ObjectToLower.flags` |
| `guildId` | `public` | `undefined` \| `string` | `ObjectToLower.guildId` |
| `id` | `public` | `string` | [`BaseChannel`](/api/classes/basechannel/).`id` |
| `lastMessageId` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.lastMessageId` |
| `lastPinTimestamp` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.lastPinTimestamp` |
| `name` | `public` | `string` | `ObjectToLower.name` |
| `nsfw` | `public` | `undefined` \| `boolean` | `ObjectToLower.nsfw` |
| `parentId` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.parentId` |
| `permissionOverwrites` | `public` | `undefined` \| `APIOverwrite`[] | `ObjectToLower.permissionOverwrites` |
| `position` | `public` | `number` | `ObjectToLower.position` |
| `rateLimitPerUser` | `public` | `undefined` \| `number` | `ObjectToLower.rateLimitPerUser` |
| `topic` | `public` | `undefined` \| `null` \| `string` | `ObjectToLower.topic` |
| `type` | `public` | `GuildAnnouncement` | [`BaseChannel`](/api/classes/basechannel/).`type` |
| `webhooks` | `public` | `Object` | [`WebhookChannelMethods`](/api/classes/webhookchannelmethods/).`webhooks` |
| `webhooks.create` | `public` | (`body`: `RESTPostAPIChannelWebhookJSONBody`) => `Promise`\<[`Webhook`](/api/classes/webhook/)\> | - |
| `webhooks.list` | `public` | () => `Promise`\<[`Webhook`](/api/classes/webhook/)[]\> | - |

## Accessors

### createdAt

```ts
get createdAt(): Date
```

createdAt gets the creation Date instace of the current object.

#### Returns

`Date`

#### Source

[seyfert/src/structures/extra/DiscordBase.ts:27](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/extra/DiscordBase.ts#L27)

***

### createdTimestamp

```ts
get createdTimestamp(): number
```

Create a timestamp for the current object.

#### Returns

`number`

#### Source

[seyfert/src/structures/extra/DiscordBase.ts:20](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/extra/DiscordBase.ts#L20)

***

### url

```ts
get url(): string
```

The URL to the channel

#### Returns

`string`

#### Source

[seyfert/src/structures/channels.ts:59](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L59)

## Methods

### addFollower()

```ts
addFollower(webhook_channel_id: string, reason?: string): Promise<APIFollowedChannel>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `webhook_channel_id` | `string` |
| `reason`? | `string` |

#### Returns

`Promise`\<`APIFollowedChannel`\>

#### Source

[seyfert/src/structures/channels.ts:514](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L514)

***

### delete()

```ts
delete(reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`delete`](/api/classes/basechannel/#delete)

#### Source

[seyfert/src/structures/channels.ts:67](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L67)

***

### edit()

```ts
edit(body: RESTPatchAPIChannelJSONBody, reason?: string): Promise<AllChannels>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `RESTPatchAPIChannelJSONBody` |
| `reason`? | `string` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`edit`](/api/classes/basechannel/#edit)

#### Source

[seyfert/src/structures/channels.ts:71](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L71)

***

### fetch()

```ts
fetch(force: boolean): Promise<AllChannels>
```

#### Parameters

| Parameter | Type | Default value |
| :------ | :------ | :------ |
| `force` | `boolean` | `false` |

#### Returns

`Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\>

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`fetch`](/api/classes/basechannel/#fetch)

#### Source

[seyfert/src/structures/channels.ts:63](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L63)

***

### is()

```ts
is<T>(channelTypes: T): this is IChannelTypes[T[number]]
```

#### Type parameters

| Type parameter |
| :------ |
| `T` extends keyof `IChannelTypes`[] |

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `channelTypes` | `T` |

#### Returns

`this is IChannelTypes[T[number]]`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`is`](/api/classes/basechannel/#is)

#### Source

[seyfert/src/structures/channels.ts:134](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L134)

***

### isCategory()

```ts
isCategory(): this is CategoryChannel
```

#### Returns

`this is CategoryChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isCategory`](/api/classes/basechannel/#iscategory)

#### Source

[seyfert/src/structures/channels.ts:114](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L114)

***

### isDM()

```ts
isDM(): this is DMChannel
```

#### Returns

`this is DMChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isDM`](/api/classes/basechannel/#isdm)

#### Source

[seyfert/src/structures/channels.ts:90](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L90)

***

### isDirectory()

```ts
isDirectory(): this is DirectoryChannel
```

#### Returns

`this is DirectoryChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isDirectory`](/api/classes/basechannel/#isdirectory)

#### Source

[seyfert/src/structures/channels.ts:102](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L102)

***

### isForum()

```ts
isForum(): this is ForumChannel
```

#### Returns

`this is ForumChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isForum`](/api/classes/basechannel/#isforum)

#### Source

[seyfert/src/structures/channels.ts:94](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L94)

***

### isGuildTextable()

```ts
isGuildTextable(): this is AllGuildTextableChannels
```

#### Returns

`this is AllGuildTextableChannels`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isGuildTextable`](/api/classes/basechannel/#isguildtextable)

#### Source

[seyfert/src/structures/channels.ts:126](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L126)

***

### isMedia()

```ts
isMedia(): this is MediaChannel
```

#### Returns

`this is MediaChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isMedia`](/api/classes/basechannel/#ismedia)

#### Source

[seyfert/src/structures/channels.ts:86](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L86)

***

### isNews()

```ts
isNews(): this is NewsChannel
```

#### Returns

`this is NewsChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isNews`](/api/classes/basechannel/#isnews)

#### Source

[seyfert/src/structures/channels.ts:118](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L118)

***

### isStage()

```ts
isStage(): this is StageChannel
```

#### Returns

`this is StageChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isStage`](/api/classes/basechannel/#isstage)

#### Source

[seyfert/src/structures/channels.ts:82](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L82)

***

### isTextGuild()

```ts
isTextGuild(): this is TextGuildChannel
```

#### Returns

`this is TextGuildChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isTextGuild`](/api/classes/basechannel/#istextguild)

#### Source

[seyfert/src/structures/channels.ts:110](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L110)

***

### isTextable()

```ts
isTextable(): this is AllTextableChannels
```

#### Returns

`this is AllTextableChannels`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isTextable`](/api/classes/basechannel/#istextable)

#### Source

[seyfert/src/structures/channels.ts:122](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L122)

***

### isThread()

```ts
isThread(): this is ThreadChannel
```

#### Returns

`this is ThreadChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isThread`](/api/classes/basechannel/#isthread)

#### Source

[seyfert/src/structures/channels.ts:98](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L98)

***

### isThreadOnly()

```ts
isThreadOnly(): this is MediaChannel | ForumChannel
```

#### Returns

`this is MediaChannel | ForumChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isThreadOnly`](/api/classes/basechannel/#isthreadonly)

#### Source

[seyfert/src/structures/channels.ts:130](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L130)

***

### isVoice()

```ts
isVoice(): this is VoiceChannel
```

#### Returns

`this is VoiceChannel`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`isVoice`](/api/classes/basechannel/#isvoice)

#### Source

[seyfert/src/structures/channels.ts:106](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L106)

***

### toString()

```ts
toString(): string
```

#### Returns

`string`

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`toString`](/api/classes/basechannel/#tostring)

#### Source

[seyfert/src/structures/channels.ts:78](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L78)

***

### \_\_intent\_\_()

#### \_\_intent\_\_(id)

```ts
static __intent__(id: "@me"): "DirectMessages"
```

##### Parameters

| Parameter | Type |
| :------ | :------ |
| `id` | `"@me"` |

##### Returns

`"DirectMessages"`

##### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`__intent__`](/api/classes/basechannel/#__intent__)

##### Source

[seyfert/src/structures/channels.ts:52](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L52)

#### \_\_intent\_\_(id)

```ts
static __intent__(id: string): "Guilds" | "DirectMessages"
```

##### Parameters

| Parameter | Type |
| :------ | :------ |
| `id` | `string` |

##### Returns

`"Guilds"` \| `"DirectMessages"`

##### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`__intent__`](/api/classes/basechannel/#__intent__)

##### Source

[seyfert/src/structures/channels.ts:53](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L53)

***

### allMethods()

```ts
static allMethods(ctx:     Object): Object
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `ctx` | `Object` |
| `ctx.client` | `BaseClient` |
| `ctx.guildId` | `string` |

#### Returns

`Object`

| Member | Type | Value |
| :------ | :------ | :------ |
| `create` | (`body`: `RESTPostAPIGuildChannelJSONBody`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `delete` | (`id`: `string`, `reason`?: `string`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `edit` | (`id`: `string`, `body`: `RESTPatchAPIChannelJSONBody`, `reason`?: `string`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `editPositions` | (`body`: `RESTPatchAPIGuildChannelPositionsJSONBody`) => `Promise`\<`never`\> | - |
| `fetch` | (`id`: `string`, `force`: `boolean`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)\> | - |
| `list` | (`force`: `boolean`) => `Promise`\<[`AllChannels`](/api/type-aliases/allchannels/)[]\> | - |

#### Inherited from

[`BaseChannel`](/api/classes/basechannel/).[`allMethods`](/api/classes/basechannel/#allmethods)

#### Source

[seyfert/src/structures/channels.ts:138](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/channels.ts#L138)