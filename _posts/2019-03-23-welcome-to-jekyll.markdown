---
layout: post
title: "react Native"
date: 2021-03-23 21:03:36 +0530
categories: Javascript react reactNative
---

→ react-navigation-tab-view

```jsx
-> npm install @react-navigation/material-top-tabs react-native-tab-view@^2.16.0
```

→ 기본 인덱스 화면에서 Slide를 적용하기위해 사용

```jsx
import { createMaterialTopTabNavigator } from "@react-navigation/material-top-tabs";

const Tab = createMaterialTopTabNavigator();

function MyTabs() {
  return (
    <Tab.Navigator>
      <Tab.Screen name="Home" component={HomeScreen} />
      <Tab.Screen name="Settings" component={SettingsScreen} />
    </Tab.Navigator>
  );
}
```

→ MainNav → 기존 스택을 Tab으로 변경후 default tabBar를 height 0 으로 지우고 사용
