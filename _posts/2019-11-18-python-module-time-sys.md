---
layout: post
title: "Модули sys и time"
categories: python
---


```python
import time

print (time.asctime())

import sys

print(sys.stdin.readline())

def my_age():
	print('how old are you?')
	age = int(sys.stdin.readline())
	if age < 18:
		print('young')
	else:
		print('old')

my_age()

```