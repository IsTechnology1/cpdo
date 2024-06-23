Cpdo

> cpdo 是一个 Bash 脚本，旨在简化将文件复制到指定目录并执行的过程。它支持使用 screen 执行文件，并提供可选项在执行后删除复制的文件。
> 
> tips:开发目标是为了在termux中执行非私有目录下的程序
> 
你可以使用下面的一键配置指来配置cpdo到系统内:
不加速:
```
curl -o /usr/bin/cpdo https://raw.githubusercontent.com/IsTechnology1/cpdo/main/lasted/cpdo && chmod +x /usr/bin/cpdo && [ -x /usr/bin/cpdo ] && echo -e "\e[32m下载成功\e[0m 使用cpdo命令继续" || echo -e "\e[31m下载失败！\e[0m"
```
中国加速链接1:
```
curl -o /usr/bin/cpdo https://github.moeyy.xyz/https://raw.githubusercontent.com/IsTechnology1/cpdo/main/lasted/cpdo && chmod +x /usr/bin/cpdo && [ -x /usr/bin/cpdo ] && echo -e "\e[32m下载成功\e[0m 使用cpdo命令继续" || echo -e "\e[31m下载失败！\e[0m"
```
中国加速链接2:
```
curl -o /usr/bin/cpdo https://gitdl.cn/https://raw.githubusercontent.com/IsTechnology1/cpdo/main/lasted/cpdo && chmod +x /usr/bin/cpdo && [ -x /usr/bin/cpdo ] && echo -e "\e[32m下载成功\e[0m 使用cpdo命令继续" || echo -e "\e[31m下载失败！\e[0m"
```

特性:
复制和执行：将指定文件复制到预设目录（默认为 /root/cpdo/）并执行。
支持 screen：使用 -s 选项可以在 screen 环境中执行文件，适合长时间运行或需要保持终端会话的任务。
文件删除：使用 -d 选项可选择在执行完成后删除复制的文件，保持环境整洁。
帮助和版本信息：使用 -h 选项显示帮助信息，展示可用选项、使用说明和当前版本号。
使用方法
```
cpdo <文件名> [-s] [-d] [-h]
<文件名>：要复制和执行的文件路径。
-s：使用 screen 执行文件。
-d：执行完成后删除复制过来的文件。
-h：显示帮助信息和版本号。
```
安装和配置
下载 cpdo 脚本到本地。
确保脚本具有执行权限：
bash
复制代码
chmod +x cpdo
可选地，将 cpdo 脚本移动到系统的可执行路径下，以便全局使用。
注意事项
确保要执行的文件存在且具有执行权限。
使用 -s 和 -d 选项时，请谨慎操作，以避免意外删除或影响重要文件。
版本信息
当前版本：2.7

许可证
本项目使用 GNU General Public License v3.0 许可。详细信息请查看 LICENSE 文件。

作者：IsTechnology


