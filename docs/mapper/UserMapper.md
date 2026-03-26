# UserMapper接口

## 类描述

MyBatis Mapper接口，提供用户数据的数据库操作。

## 方法列表

### selectAll()

- 方法描述：查询所有用户
- 起始行：11
- 返回类型：List<User>
- 调用方法：无

### selectById(Long id)

- 方法描述：根据ID查询用户
- 起始行：13
- 参数：id (Long) - 用户ID
- 返回类型：User
- 调用方法：无

### insert(User user)

- 方法描述：插入用户
- 起始行：15
- 参数：user (User) - 用户对象
- 返回类型：int
- 调用方法：无

### update(User user)

- 方法描述：更新用户
- 起始行：17
- 参数：user (User) - 用户对象
- 返回类型：int
- 调用方法：无

### deleteById(Long id)

- 方法描述：根据ID删除用户
- 起始行：19
- 参数：id (Long) - 用户ID
- 返回类型：int
- 调用方法：无
