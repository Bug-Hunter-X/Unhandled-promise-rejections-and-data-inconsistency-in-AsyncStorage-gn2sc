# AsyncStorage Bug in Expo

This repository demonstrates a common bug encountered when using AsyncStorage in Expo applications. The bug is related to unhandled promise rejections and inconsistencies in data storage and retrieval.

## Bug Description

The bug stems from improper handling of asynchronous operations within AsyncStorage. This leads to unexpected behavior such as data not being saved or retrieved correctly, or crashes caused by unhandled promise rejections.   Specifically, the issue arises from not awaiting the promises returned by `AsyncStorage.setItem` and failing to handle potential errors.