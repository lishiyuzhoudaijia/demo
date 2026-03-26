# UserServiceImpl类

## 类描述

用户服务实现类，实现UserService接口的业务逻辑。

## 字段

| 字段名 | 类型 | 描述 |
|--------|------|------|
| userMapper | UserMapper | 用户Mapper依赖 |

## 方法列表

### getAllUsers()

- 方法描述：获取所有用户
- 起始行：17-19
- 中间步骤描述：A、调用userMapper.selectAll()查询所有用户 B、返回用户列表
- 调用的方法：com.example.demo.mapper.UserMapper#selectAll()

### getUserById(Long id)

- 方法描述：根据ID获取用户
- 起始行：22-24
- 中间步骤描述：A、调用userMapper.selectById(id)查询用户 B、返回用户对象
- 调用的方法：com.example.demo.mapper.UserMapper#selectById(Long)

### createUser(User user)

- 方法描述：创建用户
- 起始行：27-30
- 中间步骤描述：A、调用userMapper.insert(user)插入用户 B、返回用户对象
- 调用的方法：com.example.demo.mapper.UserMapper#insert(User)

### updateUser(Long id, User user)

- 方法描述：更新用户
- 起始行：33-41
- 中间步骤描述：A、先调用userMapper.selectById(id)查询用户是否存在 B、如不存在返回null C、设置用户ID D、调用userMapper.update(user)更新用户 E、返回用户对象
- 调用的方法：com.example.demo.mapper.UserMapper#selectById(Long), com.example.demo.mapper.UserMapper#update(User)

### deleteUser(Long id)

- 方法描述：删除用户
- 起始行：44-46
- 中间步骤描述：A、调用userMapper.deleteById(id)删除用户 B、返回删除是否成功
- 调用的方法：com.example.demo.mapper.UserMapper#deleteById(Long)
