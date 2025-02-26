# Interface: FieldOptions\<TParentData, TName, TFieldValidator, TFormValidator, TData\>

An object type representing the options for a field in a form.

## Extended by

- [`FieldApiOptions`](fieldapioptions.md)

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

#### Source

[packages/form-core/src/FieldApi.ts:283](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L283)

***

### asyncDebounceMs?

```ts
optional asyncDebounceMs: number;
```

The default time to debounce async validation if there is not a more specific debounce time passed.

#### Source

[packages/form-core/src/FieldApi.ts:279](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L279)

***

### defaultMeta?

```ts
optional defaultMeta: Partial<FieldMeta>;
```

An optional object with default metadata for the field.

#### Source

[packages/form-core/src/FieldApi.ts:301](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L301)

***

### defaultValue?

```ts
optional defaultValue: NoInfer<TData>;
```

An optional default value for the field.

#### Source

[packages/form-core/src/FieldApi.ts:275](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L275)

***

### name

```ts
name: TName;
```

The field name. The type will be `DeepKeys<TParentData>` to ensure your name is a deep key of the parent dataset.

#### Source

[packages/form-core/src/FieldApi.ts:271](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L271)

***

### validatorAdapter?

```ts
optional validatorAdapter: TFieldValidator;
```

A validator provided by an extension, like `yupValidator` from `@tanstack/yup-form-adapter`

#### Source

[packages/form-core/src/FieldApi.ts:287](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L287)

***

### validators?

```ts
optional validators: FieldValidators<TParentData, TName, TFieldValidator, TFormValidator, TData>;
```

A list of validators to pass to the field

#### Source

[packages/form-core/src/FieldApi.ts:291](https://github.com/TanStack/form/blob/ada0211684adc85c41587b076e1217390ff5344e/packages/form-core/src/FieldApi.ts#L291)
