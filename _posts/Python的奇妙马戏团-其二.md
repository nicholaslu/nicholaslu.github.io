---
layout: post
title: Python的奇妙马戏团 其二
date: 2020-01-10 01:15:59
categories: Python
---

# 向世界问好

有了解释器，我们就开始来写第一行代码了。在学习编程时，有一个有趣的传统，那就是人们在学习一门新语言时，所学习的第一个程序，都是输出一行内容为*Hello, world!*的话~~（严格来说，称为字符串）~~。

在Python中，使用`print()`函数来进行输出文字。在终端中输入`python`进入Python环境，通过输入代码`print("Hello world!")`来输出这段话。之后Python会如实输出引号中包含的这段文字。

```
Microsoft Windows [Version 10.0.18363.535]
(c) 2019 Microsoft Corporation. All rights reserved.

C:\Users\nicho>python
Python 3.7.3 (v3.7.3:ef4ec6ed12, Mar 25 2019, 22:22:05) [MSC v.1916 64 bit (AMD64)] on win32
Type "help", "copyright", "credits" or "license" for more information.
>>> print("Hello world!")
Hello world!
```

这就代表这行代码正确运行了。

通过运行exit()来退出Python环境，回到终端。然后，这个终端就可以安全关闭了。

```
exit()

C:\Users\nicho>
```

# Visual Studio Code的安装

值得注意的是，刚才并没有机会把写出的代码保存下来。虽然说Python~~的解释器~~安装好后，即使是记事本都可以用来编程，但是为了使用的方便，还是安装一个代码编辑器。代码编辑器即编辑代码的软件~~，但一般不包含解释器、编译器等，通常包含这些的称为IDE。~~此处使用现在比较流行的、微软出品的[Visual Studio Code](https://code.visualstudio.com/)。下载并安装对应自己操作系统的Stable版本。

Visual Studio长这样

![VSCode on Windows 10](https://dppfgq.bn.files.1drv.com/y4mN6ezbDTKHBxvsVAc9w1UYKo6IiHyEuJdx3IPgbGBASS1zYfuJ9PvCWrobp1UItKdCTZcDnyksW_SEYqIeXFHDnO-uAulDpyPTDMhTa-daxPth9OmbF3sdkyEhfuWUzGQQLB8qikgcytYPlB2Th5WD9QlAUHzYNzO5afS_VooxvZJVRwxMaChSAUaTWWiGpGrxVUffIjRM32OO66AfWYdvA?width=1727&height=1303&cropmode=none)

Visual Studio Code比较特色的地方是可以安装插件。因为纯粹的编辑器是不带有很多功能的，通过安装插件的方式，可以方便的定制需要的功能。这里搜索并安装名为Python的插件，来完善对Python的支持。点击Install安装。

![install python extension](https://dppegq.bn.files.1drv.com/y4mMLGYdaqeh3vdOcPbCaXoWurQ6oSN8UFRdCtscEGkDtlM_e4_DOYeu_gF21t-imzFPGJ0t3ofTlj2GfFHkh74b5kXxwHhHK8Rjy5BHbEUMVfkRtLxmW38gyni0fMoqUGCo0C_2qwik6yWANIfHei31JsXU6f1fARDt7wdQHXjNj52MNMBDlNNwDdnlwDVbb0jNnKWUL7peCqaioCZmL6DWQ?width=1727&height=1303&cropmode=none)

在安装完成后，就可以开始编写代码了呢。File -> New File， 或者Ctrl+N来新建一个文件，既然是代码编辑器，此处的文件一般就是代码了。通过在这个编辑器，可以做到和刚才终端中一样的事情。虽然什么都没写，先还是把这个文件保存下来，File -> Save， 或者Ctrl+S来保存文件，文件名一般仅使用字母、数字和下划线的组合，扩展名使用.py，如hello_world.py。通过这个.py的扩展名，大家（指编辑器，解释器和人类等）都知道这个文件是段Python代码了。此时Visual Studio Code的右下角会显示你现在编写的代码类型

![bottom bar of VSCode](https://dppcgq.bn.files.1drv.com/y4mD54dr9SNs03FxtATf_Q5ggROCUp6CP25HA136aWgBPsFkj5QaspI_4Q1G81G47xWlFTpxujZ-gbpx7aTwOiaxhxifNeDAQGCzWCTUUyaoWrglDGGO2nFtzCVEzf6s2ISGtMy9v4HIH7k5x5fvfWOHAvol7BUOAVjWiOhPrgESHN5YCg0xi1wq6R6hj8aAYYNzOoiNWQSI5aZ08JZc0RXhg?width=1727&height=35&cropmode=none)

值得注意的是，左下角还显示了Visual Studio Code所检测到的Python版本（Python 3.7.3 64-bit）。在安装了多个Python版本的情况下，可以点击它来切换。

# Try with Code

使用Visual Studio Code，以下简称Code，在刚刚建立的文件中写入

```python
print("Hello world!")
```

保存后，点击右上角绿色三角形的运行键，运行这段代码。记住，不保存代码的话，自从上次保存以来的更改是不会被写入到文件中去的，所以在运行代码之前应当有保存一次代码的习惯。在运行之后，可以看到Code的底端弹出了如下的输出’

```
PS C:\Users\nicho> & C:/Users/nicho/AppData/Local/Programs/Python/Python37/python.exe c:/Users/nicho/Documents/temp/hello_world.py
Helo world!
PS C:\Users\nicho>
```

也就是说，得到了和终端中一致的结果。

至此，对于编辑器Visual Studio Code的大致了解就完成了，也可以自己尝试探索Code所带有的其他强大功能，甚至尝试其他的扩展。

# 附注

本文的快捷键以Windows下的为主，要想知道Linux或者macOS下的快捷键，可以查看Code的菜单。右侧一栏所显示的即是快捷键，记忆几个常用的快捷键对工作效率会有极大的提升。

<img src="https://dppdgq.bn.files.1drv.com/y4mM_77NU9Tx_we9B0j1QFFcdXEtVsBHoMOfrQ__cjBbya_PkkvNaGsYUXkzYgle-bfFiT6gbSEFZp9QnMde6JzIhZrGr_ix13DTjvObTN2mqhFK3_3hX5BH4dz41uFFHWmxOKAyHoeAnpI8c8St8My0bY3ziSNrCAIMKxwOpdSa9sncZS6xJLLm8PYt7FW2aAxtTpltH_I1JlxVqiX2kToqA?width=463&amp;height=813&amp;cropmode=none" alt="Menu of VSCode" style="zoom:50%;" />