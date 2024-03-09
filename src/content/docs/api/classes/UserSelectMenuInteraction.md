---
editUrl: false
next: false
prev: false
title: "UserSelectMenuInteraction"
---

## Extends

- [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/)

## Constructors

### new UserSelectMenuInteraction(client, interaction, __reply)

```ts
new UserSelectMenuInteraction(
   client: BaseClient, 
   interaction: APIMessageComponentSelectMenuInteraction, 
   __reply?: __InternalReplyFunction): UserSelectMenuInteraction
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `client` | `BaseClient` |
| `interaction` | `APIMessageComponentSelectMenuInteraction` |
| `__reply`? | `__InternalReplyFunction` |

#### Returns

[`UserSelectMenuInteraction`](/api/classes/userselectmenuinteraction/)

#### Overrides

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`constructor`](/api/classes/selectmenuinteraction/#constructors)

#### Source

[seyfert/src/structures/Interaction.ts:590](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L590)

## Properties

| Property | Modifier | Type | Inherited from |
| :------ | :------ | :------ | :------ |
| `appPermissions?` | `public` | `PermissionsBitField` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`appPermissions` |
| `applicationId` | `public` | `string` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`applicationId` |
| `channel` | `public` | [`AllChannels`](/api/type-aliases/allchannels/) | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`channel` |
| `channelId` | `public` | `string` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`channelId` |
| `client` | `readonly` | [`UsingClient`](/api/interfaces/usingclient/) | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`client` |
| `data` | `public` | `ObjectToLower`\<APIMessageSelectMenuInteractionData \| undefined & `APIMessageSelectMenuInteractionData`\> | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`data` |
| `entitlements` | `public` | `Object`[] | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`entitlements` |
| `guildId` | `public` | `undefined` \| `string` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`guildId` |
| `guildLocale` | `public` |  \| `undefined` \| `"id"` \| `"en-US"` \| `"en-GB"` \| `"bg"` \| `"zh-CN"` \| `"zh-TW"` \| `"hr"` \| `"cs"` \| `"da"` \| `"nl"` \| `"fi"` \| `"fr"` \| `"de"` \| `"el"` \| `"hi"` \| `"hu"` \| `"it"` \| `"ja"` \| `"ko"` \| `"lt"` \| `"no"` \| `"pl"` \| `"pt-BR"` \| `"ro"` \| `"ru"` \| `"es-ES"` \| `"es-419"` \| `"sv-SE"` \| `"th"` \| `"tr"` \| `"uk"` \| `"vi"` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`guildLocale` |
| `id` | `public` | `string` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`id` |
| `locale` | `public` |  \| `"id"` \| `"en-US"` \| `"en-GB"` \| `"bg"` \| `"zh-CN"` \| `"zh-TW"` \| `"hr"` \| `"cs"` \| `"da"` \| `"nl"` \| `"fi"` \| `"fr"` \| `"de"` \| `"el"` \| `"hi"` \| `"hu"` \| `"it"` \| `"ja"` \| `"ko"` \| `"lt"` \| `"no"` \| `"pl"` \| `"pt-BR"` \| `"ro"` \| `"ru"` \| `"es-ES"` \| `"es-419"` \| `"sv-SE"` \| `"th"` \| `"tr"` \| `"uk"` \| `"vi"` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`locale` |
| `member` | `public` | `undefined` \| [`InteractionGuildMember`](/api/classes/interactionguildmember/) | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`member` |
| `members` | `public` | [`InteractionGuildMember`](/api/classes/interactionguildmember/)[] | - |
| `message?` | `public` | [`Message`](/api/classes/message/) | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`message` |
| `replied?` | `public` | `boolean` \| `Promise`\<`boolean`\> | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`replied` |
| `token` | `public` | `string` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`token` |
| `type` | `public` | `MessageComponent` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`type` |
| `user` | `public` | [`User`](/api/classes/user/) | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`user` |
| `users` | `public` | [`User`](/api/classes/user/)[] | - |
| `version` | `public` | `1` | [`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).`version` |

## Accessors

### componentType

```ts
get componentType(): 
  | Button
  | StringSelect
  | UserSelect
  | RoleSelect
  | MentionableSelect
  | ChannelSelect
```

#### Returns

  \| `Button`
  \| `StringSelect`
  \| `UserSelect`
  \| `RoleSelect`
  \| `MentionableSelect`
  \| `ChannelSelect`

#### Source

[seyfert/src/structures/Interaction.ts:473](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L473)

***

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

### customId

```ts
get customId(): string
```

#### Returns

`string`

#### Source

[seyfert/src/structures/Interaction.ts:469](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L469)

***

### values

```ts
get values(): string[]
```

#### Returns

`string`[]

#### Source

[seyfert/src/structures/Interaction.ts:517](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L517)

## Methods

### createResponse()

```ts
createResponse(__namedParameters: Omit<RESTPostAPIWebhookWithTokenJSONBody, "components" | "embeds"> & ResolverProps): Promise<Message>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `__namedParameters` | `Omit`\<`RESTPostAPIWebhookWithTokenJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` |

#### Returns

`Promise`\<[`Message`](/api/classes/message/)\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`createResponse`](/api/classes/selectmenuinteraction/#createresponse)

#### Source

[seyfert/src/structures/Interaction.ts:409](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L409)

***

### deferReply()

```ts
deferReply(flags?: MessageFlags): Promise<void>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `flags`? | `MessageFlags` |

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`deferReply`](/api/classes/selectmenuinteraction/#deferreply)

#### Source

[seyfert/src/structures/Interaction.ts:215](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L215)

***

### deferUpdate()

```ts
deferUpdate(): Promise<void>
```

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`deferUpdate`](/api/classes/selectmenuinteraction/#deferupdate)

#### Source

[seyfert/src/structures/Interaction.ts:463](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L463)

***

### deleteMessage()

```ts
deleteMessage(messageId: string): Promise<void>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `messageId` | `string` |

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`deleteMessage`](/api/classes/selectmenuinteraction/#deletemessage)

#### Source

[seyfert/src/structures/Interaction.ts:401](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L401)

***

### deleteResponse()

```ts
deleteResponse(): Promise<void>
```

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`deleteResponse`](/api/classes/selectmenuinteraction/#deleteresponse)

#### Source

[seyfert/src/structures/Interaction.ts:397](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L397)

***

### editMessage()

```ts
editMessage(messageId: string, body: Omit<RESTPatchAPIWebhookWithTokenMessageJSONBody, "components" | "embeds"> & ResolverProps): Promise<Message>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `messageId` | `string` |
| `body` | `Omit`\<`RESTPatchAPIWebhookWithTokenMessageJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` |

#### Returns

`Promise`\<[`Message`](/api/classes/message/)\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`editMessage`](/api/classes/selectmenuinteraction/#editmessage)

#### Source

[seyfert/src/structures/Interaction.ts:379](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L379)

***

### editOrReply()

```ts
editOrReply<FR>(body: Omit<APIInteractionResponseCallbackData, "components" | "embeds"> & ResolverProps, fetchReply?: FR): Promise<When<FR, WebhookMessage, void>>
```

#### Type parameters

| Type parameter | Value |
| :------ | :------ |
| `FR` extends `boolean` | `false` |

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `Omit`\<`APIInteractionResponseCallbackData`, `"components"` \| `"embeds"`\> & `ResolverProps` |
| `fetchReply`? | `FR` |

#### Returns

`Promise`\<`When`\<`FR`, [`WebhookMessage`](/api/classes/webhookmessage/), `void`\>\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`editOrReply`](/api/classes/selectmenuinteraction/#editorreply)

#### Source

[seyfert/src/structures/Interaction.ts:367](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L367)

***

### editResponse()

```ts
editResponse(body: Omit<RESTPatchAPIWebhookWithTokenMessageJSONBody, "components" | "embeds"> & ResolverProps): Promise<Message>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `Omit`\<`RESTPatchAPIWebhookWithTokenMessageJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` |

#### Returns

`Promise`\<[`Message`](/api/classes/message/)\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`editResponse`](/api/classes/selectmenuinteraction/#editresponse)

#### Source

[seyfert/src/structures/Interaction.ts:393](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L393)

***

### fetchGuild()

```ts
fetchGuild(force: boolean): undefined | Promise<Guild<"cached"> | Guild<"api">>
```

#### Parameters

| Parameter | Type | Default value |
| :------ | :------ | :------ |
| `force` | `boolean` | `false` |

#### Returns

`undefined` \| `Promise`\<[`Guild`](/api/classes/guild/)\<`"cached"`\> \| [`Guild`](/api/classes/guild/)\<`"api"`\>\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`fetchGuild`](/api/classes/selectmenuinteraction/#fetchguild)

#### Source

[seyfert/src/structures/Interaction.ts:277](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L277)

***

### fetchMessage()

```ts
fetchMessage(messageId: string): Promise<undefined | WebhookMessage>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `messageId` | `string` |

#### Returns

`Promise`\<`undefined` \| [`WebhookMessage`](/api/classes/webhookmessage/)\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`fetchMessage`](/api/classes/selectmenuinteraction/#fetchmessage)

#### Source

[seyfert/src/structures/Interaction.ts:340](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L340)

***

### fetchResponse()

```ts
fetchResponse(): Promise<undefined | WebhookMessage>
```

#### Returns

`Promise`\<`undefined` \| [`WebhookMessage`](/api/classes/webhookmessage/)\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`fetchResponse`](/api/classes/selectmenuinteraction/#fetchresponse)

#### Source

[seyfert/src/structures/Interaction.ts:344](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L344)

***

### isButton()

```ts
isButton(): this is ButtonInteraction
```

#### Returns

`this is ButtonInteraction`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isButton`](/api/classes/selectmenuinteraction/#isbutton)

#### Source

[seyfert/src/structures/Interaction.ts:477](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L477)

***

### isChannelSelectMenu()

```ts
isChannelSelectMenu(): this is ChannelSelectMenuInteraction
```

#### Returns

`this is ChannelSelectMenuInteraction`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isChannelSelectMenu`](/api/classes/selectmenuinteraction/#ischannelselectmenu)

#### Source

[seyfert/src/structures/Interaction.ts:481](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L481)

***

### isMentionableSelectMenu()

```ts
isMentionableSelectMenu(): this is MentionableSelectMenuInteraction
```

#### Returns

`this is MentionableSelectMenuInteraction`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isMentionableSelectMenu`](/api/classes/selectmenuinteraction/#ismentionableselectmenu)

#### Source

[seyfert/src/structures/Interaction.ts:489](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L489)

***

### isRoleSelectMenu()

```ts
isRoleSelectMenu(): this is RoleSelectMenuInteraction
```

#### Returns

`this is RoleSelectMenuInteraction`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isRoleSelectMenu`](/api/classes/selectmenuinteraction/#isroleselectmenu)

#### Source

[seyfert/src/structures/Interaction.ts:485](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L485)

***

### isStringSelectMenu()

```ts
isStringSelectMenu(): this is StringSelectMenuInteraction<string[]>
```

#### Returns

`this is StringSelectMenuInteraction<string[]>`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isStringSelectMenu`](/api/classes/selectmenuinteraction/#isstringselectmenu)

#### Source

[seyfert/src/structures/Interaction.ts:497](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L497)

***

### isUserSelectMenu()

```ts
isUserSelectMenu(): this is UserSelectMenuInteraction
```

#### Returns

`this is UserSelectMenuInteraction`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`isUserSelectMenu`](/api/classes/selectmenuinteraction/#isuserselectmenu)

#### Source

[seyfert/src/structures/Interaction.ts:493](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L493)

***

### modal()

```ts
modal(body: ModalCreateBodyRequest): Promise<void>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `ModalCreateBodyRequest` |

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`modal`](/api/classes/selectmenuinteraction/#modal)

#### Source

[seyfert/src/structures/Interaction.ts:360](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L360)

***

### reply()

```ts
reply(body: ReplyInteractionBody): Promise<void>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | [`ReplyInteractionBody`](/api/type-aliases/replyinteractionbody/) |

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`reply`](/api/classes/selectmenuinteraction/#reply)

#### Source

[seyfert/src/structures/Interaction.ts:189](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L189)

***

### update()

```ts
update(data: Omit<APIInteractionResponseCallbackData, "components" | "embeds"> & ResolverProps): Promise<void>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `data` | `Omit`\<`APIInteractionResponseCallbackData`, `"components"` \| `"embeds"`\> & `ResolverProps` |

#### Returns

`Promise`\<`void`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`update`](/api/classes/selectmenuinteraction/#update)

#### Source

[seyfert/src/structures/Interaction.ts:456](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L456)

***

### write()

```ts
write<FR>(body: Omit<APIInteractionResponseCallbackData, "components" | "embeds"> & ResolverProps, fetchReply?: FR): Promise<When<FR, WebhookMessage, void>>
```

#### Type parameters

| Type parameter | Value |
| :------ | :------ |
| `FR` extends `boolean` | `false` |

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `Omit`\<`APIInteractionResponseCallbackData`, `"components"` \| `"embeds"`\> & `ResolverProps` |
| `fetchReply`? | `FR` |

#### Returns

`Promise`\<`When`\<`FR`, [`WebhookMessage`](/api/classes/webhookmessage/), `void`\>\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`write`](/api/classes/selectmenuinteraction/#write)

#### Source

[seyfert/src/structures/Interaction.ts:348](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L348)

***

### from()

```ts
static from(
   client: BaseClient, 
   gateway: APIInteraction, 
__reply?: __InternalReplyFunction): StringSelectMenuInteraction<string[]> | AutocompleteInteraction<boolean> | BaseInteraction<boolean, APIPingInteraction>
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `client` | `BaseClient` |
| `gateway` | `APIInteraction` |
| `__reply`? | `__InternalReplyFunction` |

#### Returns

[`StringSelectMenuInteraction`](/api/classes/stringselectmenuinteraction/)\<`string`[]\> \| [`AutocompleteInteraction`](/api/classes/autocompleteinteraction/)\<`boolean`\> \| [`BaseInteraction`](/api/classes/baseinteraction/)\<`boolean`, `APIPingInteraction`\>

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`from`](/api/classes/selectmenuinteraction/#from)

#### Source

[seyfert/src/structures/Interaction.ts:224](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L224)

***

### transformBody()

```ts
static transformBody<T>(body: Omit<RESTPostAPIChannelMessageJSONBody, "components" | "embeds"> & ResolverProps | Omit<RESTPatchAPIChannelMessageJSONBody, "components" | "embeds"> & ResolverProps | Omit<RESTPostAPIWebhookWithTokenJSONBody, "components" | "embeds"> & ResolverProps | Omit<RESTPatchAPIWebhookWithTokenMessageJSONBody, "components" | "embeds"> & ResolverProps): T
```

#### Type parameters

| Type parameter |
| :------ |
| `T` |

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | `Omit`\<`RESTPostAPIChannelMessageJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` \| `Omit`\<`RESTPatchAPIChannelMessageJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` \| `Omit`\<`RESTPostAPIWebhookWithTokenJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` \| `Omit`\<`RESTPatchAPIWebhookWithTokenMessageJSONBody`, `"components"` \| `"embeds"`\> & `ResolverProps` |

#### Returns

`T`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`transformBody`](/api/classes/selectmenuinteraction/#transformbody)

#### Source

[seyfert/src/structures/Interaction.ts:163](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L163)

***

### transformBodyRequest()

```ts
static transformBodyRequest(body: ReplyInteractionBody): APIInteractionResponse
```

#### Parameters

| Parameter | Type |
| :------ | :------ |
| `body` | [`ReplyInteractionBody`](/api/type-aliases/replyinteractionbody/) |

#### Returns

`APIInteractionResponse`

#### Inherited from

[`SelectMenuInteraction`](/api/classes/selectmenuinteraction/).[`transformBodyRequest`](/api/classes/selectmenuinteraction/#transformbodyrequest)

#### Source

[seyfert/src/structures/Interaction.ts:119](https://github.com/potoland/potocuit/blob/fe122a1/src/structures/Interaction.ts#L119)