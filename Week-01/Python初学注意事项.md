# Python初学的注意事项

> **作者**：长行
>
> **时间**：2020.05.10

首先，我们在写代码之前应该明白我们写代码的初衷。总体来说，我们的代码大概分为两类，一类是作为产品，让用户来用的，此时我们假定的用户是不了解产品，更不了解编程的，所以我们应当尽可能做好交互，让用户尽可能用的方便；另一类是作为工具，让其他协作者来用着，此时我们应该提高代码的可读性，让其他协作者更方便地理解代码，使用代码。

无论是哪种情况，我们首先最需要注意的就是代码的稳定，尤其是在对代码还不熟悉的初学阶段。我们应该对自己写出的每一段代码都认真调试，确保在各种情况下代码不会报错。

```python
USER_LIST = {"AAA":123456, "BBB":123456, "CCC":123456}
username = input("用户名:")
password = input("密码:")
if password == USER_LIST[username]:
    print('登录成功')
else:
    print('登录失败')
```

请大家看一看以上的代码，这段代码当用户输入的用户名不在users的key的列表中时，会报KeyError的错误；此外，即使用户输入了正确的代码，

除外，我们还需要注意代码的可读性，代码的可读性一方面是方便其他协作者，一方面也是方便将来的自己。虽然在初学阶段注意代码的可读性有些困难，但是还是建议大家在学习之初就能养成一些好习惯。

之前我在一本书里看到过一个关于代码可读性的定理：代码的写法应当使别人理解它的所需的事件最小化。

从实践角度来说看，我们主要需要注意一下几点：
* 如何命名
* 如何使用变量
* 如何简化表达式
* 如何让代码更具美感
* 如何使用注释

下面我们结合

