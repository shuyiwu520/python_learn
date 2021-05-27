在python使用过程中，在不同的项目里，常常会出现频繁地自定义同一个函数的情况。为了解决这个问题，我们可以选择创建一个自定义的库，并将其添加到系统路径中

具体操作如下：

    在任意位置新建一个项目my_libs，并在其中新建python文件my_lib1和my_lib2，将需要自定义的函数在my_lib1文件中定义
    这里写图片描述

    通过sys.path获取site-packages文件夹的路径
    这里写图片描述

    在site-packages中新建mylibs.pth文件，将my_libs项目的路径写进去并保存。（注意是项目的路径，不是其中的python文件的路径）
    这里写图片描述

接下来，直接导入就可以使用了

from mylib1 import make_path