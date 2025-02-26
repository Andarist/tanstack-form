# Interface: FieldApiOptions\<TParentData, TName, TFieldValidator, TFormValidator, TData\>

An object type representing the required options for the FieldApi class.

## Extends

- [`FieldOptions`](fieldoptions.md)\<`TParentData`, `TName`, `TFieldValidator`, `TFormValidator`, `TData`\>

## Type parameters

• **TParentData**

• **TName** *extends* [`DeepKeys`](deepkeys.md)\<`TParentData`\>

• **TFieldValidator** *extends* `Validator`\<[`DeepValue`](deepvalue.md)\<`TParentData`, `TName`\>, `unknown`\> \| `undefined` = `undefined`

• **TFormValidator** *extends* `Validator`\<`TParentData`, `unknown`\> \| `undefined` = `undefined`

• **TData** *extends* [`DeepValue`](deepvalue.md)\<`TParentData`, `TName`\> = [`DeepValue`](deepvalue.md)\<`TParentData`, `TName`\>

## Properties

### asyncAlways?

```ts
optional asyncAlways: boolean;
```

If `true`, always run async validation, even if there are errors emitted during synchronous validation.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`asyncAlways`](Interface.FieldOptions.md#asyncalways)

#### Source

[packages/form-core/src/FieldApi.ts:283](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L283)

***

### asyncDebounceMs?

```ts
optional asyncDebounceMs: number;
```

The default time to debounce async validation if there is not a more specific debounce time passed.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`asyncDebounceMs`](Interface.FieldOptions.md#asyncdebouncems)

#### Source

[packages/form-core/src/FieldApi.ts:279](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L279)

***

### defaultMeta?

```ts
optional defaultMeta: Partial<FieldMeta>;
```

An optional object with default metadata for the field.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`defaultMeta`](Interface.FieldOptions.md#defaultmeta)

#### Source

[packages/form-core/src/FieldApi.ts:301](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L301)

***

### defaultValue?

```ts
optional defaultValue: NoInfer<TData>;
```

An optional default value for the field.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`defaultValue`](Interface.FieldOptions.md#defaultvalue)

#### Source

[packages/form-core/src/FieldApi.ts:275](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L275)

***

### form

```ts
form: FormApi<TParentData, TFormValidator>;
```

#### Source

[packages/form-core/src/FieldApi.ts:324](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L324)

***

### name

```ts
name: TName;
```

The field name. The type will be `DeepKeys<TParentData>` to ensure your name is a deep key of the parent dataset.

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`name`](Interface.FieldOptions.md#name)

#### Source

[packages/form-core/src/FieldApi.ts:271](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L271)

***

### validatorAdapter?

```ts
optional validatorAdapter: TFieldValidator;
```

A validator provided by an extension, like `yupValidator` from `@tanstack/yup-form-adapter`

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`validatorAdapter`](Interface.FieldOptions.md#validatoradapter)

#### Source

[packages/form-core/src/FieldApi.ts:287](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L287)

***

### validators?

```ts
optional validators: FieldValidators<TParentData, TName, TFieldValidator, TFormValidator, TData>;
```

A list of validators to pass to the field

#### Inherited from

[`FieldOptions`](fieldoptions.md).[`validators`](Interface.FieldOptions.md#validators)

#### Source

[packages/form-core/src/FieldApi.ts:291](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L291)
