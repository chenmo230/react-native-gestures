React Native Gestures
=====================

> React Native Composable Gesture Library

[![js-standard-style](https://cdn.rawgit.com/feross/standard/master/badge.svg)](https://github.com/feross/standard)
[![Build Status](https://travis-ci.org/kiddkai/react-native-gestures.svg)](https://travis-ci.org/kiddkai/react-native-gestures)
[![npm version](http://img.shields.io/npm/v/react-native-gestures.svg?style=flat-square)](https://npmjs.org/package/react-native-gestures "View this project on npm")
[![npm version](http://img.shields.io/npm/dm/react-native-gestures.svg?style=flat-square)](https://npmjs.org/package/react-native-gestures "View this project on npm")
[![Issue Stats](http://issuestats.com/github/kiddkai/react-native-gestures/badge/pr?style=flat-square)](https://github.com/kiddkai/react-native-gestures/pulls?q=is%3Apr+is%3Aclosed)
[![Issue Stats](http://issuestats.com/github/kiddkai/react-native-gestures/badge/issue?style=flat-square)](https://github.com/kiddkai/react-native-gestures/issues?q=is%3Aissue+is%3Aclosed)
[![js-standard-style](https://img.shields.io/badge/code%20style-standard-brightgreen.svg?style=flat)](http://standardjs.com/)


Showcase
--------

![](http://i.imgur.com/qxzroIb.gif?1)


Quick Sample
------------

```js
import React, {
  View,
  Text
} from 'react-native';

import {
  drag,
  pinch,
  GestureView
} from 'react-native-gestures';

export default React.createClass({
  render() {
    onGestureError(err) {
      console.error(err);
    },
    return (
      <View>
        <GestureView gestures={[drag]}>
          <Text>I can move</Text>
        </GestureView>

        <GestureView gestures={[pinch]}>
          <Text>I can do pinch</Text>
        </GestureView>

        <GestureView gestures={[pinch, drag]}>
          <Text>I can move and pinch</Text>
        </GestureView>
      </View>
    );
  }
});
```
