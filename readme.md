用于存放MCU样例程序源代码的仓库。

瑞萨原厂提供多种集成开发环境和编译器的支持，需要为客户提供不同开发环境下的样例程序。这些样例程序的源代码几乎都是相同的，不同的是项目工程的配置。
以RA MCU为例，项目工程和FSP组件的配置及源代码都由配置工具自动生成，只需在项目下添加用户源代码即可。

由于Git无法保留hardlink，电脑上的单一代码仓库内不使用hardlink，需要将源代码仓库和工程仓库分开处理。

把工程的源代码统一放在一个目录下，然后在编译用的电脑上通过hardlink链接到各个工程项目下，即可实现不同工程下的源代码自动同步。

这个仓库只保留源代码，所有的源代码的修改都会合并到这个仓库里，作为存档。

此外还有另一个样例工程仓库，里面包含了工程设置和用户程序源代码。供客户下载使用。
