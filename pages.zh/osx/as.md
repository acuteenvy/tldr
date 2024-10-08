# as

> 便携式 GNU 汇编程序。
> 主要用于汇编 `gcc` 的输出以供 `ld` 使用。
> 更多信息：<https://keith.github.io/xcode-man-pages/as.1.html>.

- 汇编文件，将输出写入 a.out：

`as {{路径/到/文件.s}}`

- 将输出汇编到给定文件：

`as {{路径/到/文件.s}} -o {{路径/到/输出.o}}`

- 通过跳过空白和注释预处理来更快地生成输出.（应该只用于受信任的编译器）：

`as -f {{路径/到/文件.s}}`

- 在目录列表中包含一个给定路径，以搜索 .include 指令中指定的文件：

`as -I {{目标文件夹}} {{路径/到/文件.s}}`
