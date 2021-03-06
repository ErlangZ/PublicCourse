# HomeWork1

Great oaks from little acorns. Let's setup our environment and learn about basic tools first.

## Setup environment
You need a PC with [Ubuntu 16.04](http://releases.ubuntu.com/16.04/)
installed. And make sure you have installed [git](https://git-scm.com/),
[bazel](https://bazel.build/). With `apt-get` we can easily get them.
```
sudo apt-get install git bazel
```
Besides, we'll use some more libraries in Cpp, [gtest](https://github.com/google/googletest),
[protobuf](https://github.com/google/protobuf), [glog](https://github.com/google/glog),
[gflags](https://github.com/gflags/gflags). You don't need install them in your system,
`bazel` will download and put them to right path.
Please make sure you've grasped basic usage of them before we've gone deeper.

## Get started
Complete the simple tasks below to warm up.

### 1. Hello World!
1. Clone this repo with `git`.
1. Use `bazel` to build and run `helloworld`.
`bazel run //homework1/helloworld:main`
You can see some build information on screen and then the "Hello World!".
Please add some code yourself to learn about how the build-system works.

### 2. Run Unittest
There is a demo about how to define class and test your code in `/homework1/unittest/`.
Run `bazel test //homework1/unittest:car_test` and you'll see all test cases have passed.
After that please complete the code in car_test.cc.

### 3. Protobuf
`Protobuf` is a very popular extensible mechanism for serializing structured data. It is
language-neutral and platform-neutral, you can generate Cpp code from `proto` files. We'll use
`protobuf` to store simple data structure for sensors message, please be familiar with it. There
is a demo about `protobuf` in /homework1/protobuf, please read about it.

