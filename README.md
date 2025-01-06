# React Native FlatList: Inconsistent Rendering with Non-Unique `keyExtractor` Keys

This repository demonstrates a common error in React Native's `FlatList` component: using a `keyExtractor` function that doesn't provide unique keys for each item.  This leads to incorrect rendering and potential performance problems.

## Problem

When the `keyExtractor` function returns non-unique keys, `FlatList` might reuse components incorrectly, causing visual glitches and unexpected behavior. This often arises when your data contains duplicate IDs or other keys used for identification.

## Solution

Ensure your `keyExtractor` function consistently returns a unique identifier for each item in your data array. Consider generating a UUID or using a combination of fields if necessary to guarantee uniqueness.