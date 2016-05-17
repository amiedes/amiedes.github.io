---
layout: post
title: Install googletest on Mac OS X
published: true
tags: software, c++, testing
---

#### Steps

* Download *googletest* from https://github.com/google/googletest
* Copy to `/Users/amiedes/installed`
* Install *cmake* with:

```bash
brew install cmake
```

* Add the following line to your .bash_profile

```bash
export GTEST_DIR=/Users/amiedes/installed/googletest-master/googletest
```

* Build *gtest*

```bash
cd /Users/amiedes/installed
mkdir mybuild
cd mybuild
cmake $GTEST_DIR
make
```

* Install gtest library

```bash
sudo cp -r $GTEST_DIR/include/gtest /usr/local/include/
sudo cp lib*.a /usr/local/lib
```

#### Sources:

[https://github.com/google/googletest/blob/master/googletest/README.md](https://github.com/google/googletest/blob/master/googletest/README.md)
[http://ysonggit.github.io/system/2015/01/01/install-gtest-on-mac-os-yosemite.html](http://ysonggit.github.io/system/2015/01/01/install-gtest-on-mac-os-yosemite.html)
