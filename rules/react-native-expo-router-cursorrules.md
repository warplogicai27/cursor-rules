---
title: "React Native Expo Router v4 Production Cursor Rules"
framework: "React Native"
language: "TypeScript"
category: "Mobile Development"
slug: "react-native-expo-router-cursorrules"
url: "https://www.warplogicai.com/prompts/react-native-expo-router-cursorrules"
---

# React Native Expo Router v4 Production Cursor Rules

> **Quick Install via Terminal:**
> ```bash
> npx warplogic add react-native-expo-router-cursorrules
> ```
> Or pull directly:
> * Cursor: `curl -s https://warplogicai.com/api/v1/prompts/react-native-expo-router-cursorrules/raw?tool=cursor > .cursor/rules/react-native-expo-router-cursorrules.mdc`
> * Claude Code: `curl -s https://warplogicai.com/api/v1/prompts/react-native-expo-router-cursorrules/raw?tool=claude >> CLAUDE.md`
> * AGENTS.md: `curl -s https://warplogicai.com/api/v1/prompts/react-native-expo-router-cursorrules/raw?tool=agents >> AGENTS.md`

---

## Production Rule Content

---
description: React Native Expo Router v4 Production Rules
globs: ["app/**/*", "components/**/*"]
alwaysApply: true
---

# React Native Expo Router v4 Architecture

You are an expert React Native and Expo Mobile Engineer.

## 1. Routing & Layouts
- Enforce Expo Router v4 directory-based routing inside `app/`.
- Use `(tabs)` and `(auth)` route groups for distinct navigational hierarchies.
- Handle deep-links via typed routes with `Link` and `useRouter()`.

## 2. Performance & Animations
- Run all complex animations on the UI thread using `react-native-reanimated` worklets.
- Avoid anonymous arrow functions in `FlatList` or `FlashList` `renderItem` props.
