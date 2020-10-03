---
id: version-0.62-imagebackground
title: ImageBackground
original_id: imagebackground
---

##### 本文档贡献者：[sunnylqm](https://github.com/search?q=sunnylqm&type=Users)(100.00%)

A common feature request from developers familiar with the web is `background-image`. To handle this use case, you can use the `<ImageBackground>` component, which has the same props as `<Image>`, and add whatever children to it you would like to layer on top of it.

You might not want to use `<ImageBackground>` in some cases, since the implementation is very simple. Refer to `<ImageBackground>`'s [source code](https://github.com/facebook/react-native/blob/master/Libraries/Image/ImageBackground.js) for more insight, and create your own custom component when needed.

Note that you must specify some width and height style attributes.

## 示例

```SnackPlayer name=ImageBackground
import React from "react";
import { ImageBackground, StyleSheet, Text, View } from "react-native";

const image = { uri: "https://reactjs.org/logo-og.png" };

const App = () => (
  <View style={styles.container}>
    <ImageBackground source={image} style={styles.image}>
      <Text style={styles.text}>Inside</Text>
    </ImageBackground>
  </View>
);

const styles = StyleSheet.create({
  container: {
    flex: 1,
    flexDirection: "column"
  },
  image: {
    flex: 1,
    resizeMode: "cover",
    justifyContent: "center"
  },
  text: {
    color: "grey",
    fontSize: 30,
    fontWeight: "bold"
  }
});

export default App;
```

---

# 文档

## Props

### `style`

| 类型                               | 必填 |
| ---------------------------------- | ---- |
| [view styles](view-style-props.md) | 否   |

### `imageStyle`

| 类型                                 | 必填 |
| ------------------------------------ | ---- |
| [image styles](image-style-props.md) | 否   |

### `imageRef`

Allows to set a reference to the inner `Image` component

| 类型                                                  | 必填 |
| ----------------------------------------------------- | ---- |
| [Ref](https://reactjs.org/docs/refs-and-the-dom.html) | 否   |