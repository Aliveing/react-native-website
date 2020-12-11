---
id: rect
title: Rect Object Type
---

##### 本文档贡献者：[sunnylqm](https://github.com/search?q=sunnylqm&type=Users)(100.00%)

`Rect` accepts numeric pixel values to describe how far to extend a rectangular area. These values are added to the original area's size to expand it.

## Example

```js
{
    bottom: 20,
    left: null,
    right: undefined,
    top: 50
}
```

## Keys and values

### `bottom`

| Type                        | Required |
| --------------------------- | -------- |
| number, `null`, `undefined` | No       |

### `left`

| Type                        | Required |
| --------------------------- | -------- |
| number, `null`, `undefined` | No       |

### `right`

| Type                        | Required |
| --------------------------- | -------- |
| number, `null`, `undefined` | No       |

### `top`

| Type                        | Required |
| --------------------------- | -------- |
| number, `null`, `undefined` | No       |

## Used by

- [`Image`](image)
- [`Presssable`](pressable)
- [`Text`](text)
- [`TouchableWithoutFeedback`](touchablewithoutfeedback)
