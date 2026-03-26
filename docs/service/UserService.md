# UserService接口

## 类描述

用户服务接口，定义用户业务逻辑。

## 方法列表

### getAllUsers()

- 方法描述：获取所有用户
- 起始行：8
- 返回类型：List<User>
- 调用方法：无

### getUserById(Long id)

- 方法描述：根据ID获取用户
- 起始行：10
- 参数：id (Long) - 用户ID
- 返回类型：User
- 调用方法：无

### createUser(User user)

- 方法描述：创建用户
- 起始行：12
- 参数：user (User) - 用户对象
- 返回类型：User
- 调用方法：无

### updateUser(Long id, User user)

- 方法描述：更新用户
- 起始行：14
- 参数：id (Long) - 用户ID, user (User) - 用户对象
- 返回类型：User
- 调用方法：无

### deleteUser(Long id)

- 方法描述：删除用户
- 起始行：16
- 参数：id (Long) - 用户ID
- 返回类型：boolean
- 调用方法：无
