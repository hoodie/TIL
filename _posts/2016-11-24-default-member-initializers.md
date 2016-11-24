---
layout: post
title: "default member initializers"
date:   2016-11-24 12:03:49 +0100
description: ""
tags: cpp11, cpp
---

[C++ Weekly E33](https://www.youtube.com/watch?v=-qNNAMH9LHA) mentions this:

```cpp
struct S
{
  int value = 5;
}
```

Which produces more efficient debug code and is by far more readable than the old way:

```cpp
struct S
{
  S() : value(5) {}
  int value;
}
```

My impression is *"Why didn't they come up with this first?"*
