## Datainput 第二单元数据投喂程序

#### 程序功能

本 `datainput` 程序用于第二单元三次作业的定时投喂以及结合管道获得相应输出

#### 使用说明

1. 默认的文件以 `stdin.txt` 和 `code.jar` 文件命名，放置在相同路径下。分别是对应的某次输入数据（**包含时间戳**），和这份数据对应的 `java` 代码生成的的 `jar` 包。

2. 以windows为例，利用管道输入获取实时输出，例如：`./datainput_student_win64.exe | java -jar code.jar`  

2. 在命令行中执行二进制文件。

   例：

   对于Linux 64位操作系统：
   
   ```bash
   chmod u+x datainput_student_linux_x86_64
   ./datainput_student_linux_x86_64 | java -jar code.jar
   ```
   
   对于Windows操作系统：
   
   ```powershell
   .\datainput_student_win64.exe | java -jar code.jar
   ```
   
   对于macOS操作系统：
   
   ```sh
   ./datainput_student_darwin_m1 | java -jar code.jar
   ```
   
   仅提供对以上三种三种操作系统的支持。

提示：请根据操作系统使用对应的二进制文件，请在命令提示符(windows等)/终端(Linux, macOS等)中执行。

#### 其他

数据说明：只能连续读入多行请求，遇见空行程序就会中止

本程序仅为方便大家进行本地数据测试，减少不必要测试代码编写

**本程序仅供大家参考**

