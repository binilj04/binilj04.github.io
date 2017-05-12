---
layout: post
title: "Find text in directory"
modified:
categories: blog
excerpt:
tags: []
image:
  feature:
date: 2017-05-10T10:13:51Z
---
Linux users!! This is a simple example of finding a text in the directory. There is this powerful tool called ```grep```

Following are a few use cases:

#### Searching in a folder you are in 

``` python
grep -rnw  -e 'word1' 
```

#### Searching for two or more words

```grep -rnw 'word1|word2' ```

#### Searching in a directory or folder

```grep -rnw 'word1' ~/folder/ ```

For more options  check out the grep help documentaiton
```grep --help```	