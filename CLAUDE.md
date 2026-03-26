整体项目完全由claude自动生成

src下为java代码，src同级的docs为整个项目的spec文档，src里面的每个文件在docs下都有一个同名的md解释性文档；

解释性文档需要遵循以下规则
1、如果是类则介绍下类的描述已经字段和字段描述即可
2、如果是方法类则需要描述每个方法，每个方法需要按顺序包含下面这些元素,方法名(包含参数类型)、方法描述、起始行、中间步骤描述以及调用方法（包含参数类型）的位置
3、如果是调用入口则增加一个url的参数描述
例如：
url:aaaa/ddd/ccc
方法名：Test（String）
方法描述：用来做测试的方法
起始行： 8-15
中间步骤描述：A、测试参数校验  B、测试方法逻辑 C、返回测试结果
调用的方法：com.example.demo.service.impl.UserServiceImpl#getUserById(Long) 