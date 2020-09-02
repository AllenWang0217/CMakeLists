# CMakeLists

本工程是一个小的多级目录使用CMakeLists.txt进行编译的事例。

工程组织

```
├── CMakeLists.txt
├── README.md
├── build.sh
├── hello
│   ├── CMakeLists.txt
│   ├── include
│   │   └── hello.h
│   └── source
│       └── hello.cpp
├── main.cpp
├── project
└── world
    ├── CMakeLists.txt
    ├── include
    │   └── world.h
    └── source
        └── world.cpp
```

`project`目录存放的是eclipse工程