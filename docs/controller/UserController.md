# UserController类

## 类描述

用户控制器，提供用户相关的RESTful API接口。

## 字段

| 字段名 | 类型 | 描述 |
|--------|------|------|
| userService | UserService | 用户服务依赖 |

## 方法列表

### getAllUsers()

- url: /api/users
- 方法名：getAllUsers()
- 方法描述：获取所有用户
- 起始行：16-19
- 中间步骤描述：A、调用userService.getAllUsers()获取所有用户 B、返回用户列表
- 调用的方法：com.example.demo.service.UserService#getAllUsers()

### getUserById(Long id)

- url: /api/users/{id}
- 方法名：getUserById(Long id)
- 方法描述：根据ID获取用户
- 起始行：21-24
- 中间步骤描述：A、调用userService.getUserById(id)查询用户 B、返回用户对象
- 调用的方法：com.example.demo.service.UserService#getUserById(Long)

### createUser(User user)

- url: /api/users
- 方法名：createUser(User user)
- 方法描述：创建用户
- 起始行：26-29
- 中间步骤描述：A、调用userService.createUser(user)创建用户 B、返回创建的用户对象
- 调用的方法：com.example.demo.service.UserService#createUser(User)

### updateUser(Long id, User user)

- url: /api/users/{id}
- 方法名：updateUser(Long id, User user)
- 方法描述：更新用户
- 起始行：31-34
- 中间步骤描述：A、调用userService.updateUser(id, user)更新用户 B、返回更新后的用户对象
- 调用的方法：com.example.demo.service.UserService#updateUser(Long, User)

### deleteUser(Long id)

- url: /api/users/{id}
- 方法名：deleteUser(Long id)
- 方法描述：删除用户
- 起始行：36-39
- 中间步骤描述：A、调用userService.deleteUser(id)删除用户 B、返回删除是否成功
- 调用的方法：com.example.demo.service.UserService#deleteUser(Long)
