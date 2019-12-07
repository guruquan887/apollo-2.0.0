# modules/common

```
Contains code that is not module-specific.
```

## apollo_app
```
The "apollo_app" build target defines the abstract class ApolloApp,
which is implemented by all modules, as well as the macro APOLLO_MAIN,
used to launch each module.
```

## log
```
The "log" build target wraps the Google Log system into project-specific macros,
allowing for more refined control over the levels of logging.
```

## macro
```
The "macro" build target defines a few commonly used class-specific macros.
```

## adapters \\数据交互的抽象接口
```
Adapters are used by the different modules to communicate with one another.
The AdapterManager class hosts all the specific adapters and manages them.
Adapters need to be registered with the macro REGISTER_ADAPTER.
The Adapter class serves as a layer of abstraction between
Apollo modules and I/O mechanisms (e.g. ROS).
```


## configs/data  \\配置文件加载
```
These specify the vehicle configuration.
```

## math \\提供了数学几何api接口
```
Implements a number of useful mathematical libraries.
```

## monitor \\提供监控log信息
```
Defines a logging system.
```

## proto
```
Defines a number of project-wide protocol buffers.
```

## status \\提供各个模块工作状态
```
Used for determining whether certain functions were performed successfully,
providing helpful error messages otherwise.
```

## time \\提供计时类
```
Helper functions related to time.
```

## util \\提供文件io管理功能
```
Contains an implementation of a factory design pattern with registration,
a few string parsing functions, and some utilities for parsing
protocol buffers from files.
```

## vehicle_state \\提供车辆状态信息与预期状态估计
```
This class specifies the current state of the vehicle (e.g. position, velocity,
heading, etc.).
```
