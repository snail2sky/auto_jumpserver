# auto connect jumpserver
- 描述: 这是一个比较简单的自动连接到跳板机(堡垒机)的工具或者脚本
- 用法: 
        1. 你需要修改user.cfg配置文件，将用户名和你的MFA sercet修改好，如果你的
        ssh 私钥放在非 ~/.ssh 目录下，那么你需要修改user.cfg中的private_key值
        2. 当你修改完所有的信息之后，可以使用jp -h来查看帮助信息
           (如果是第一次，脚本会做一些初始化的操作，如将当前目录加到环境变量中，并重启shell)
        3. 运行jp命令，将会自动连接到user.cfg中定义的jumpserver上
        4. 其他功能，可以使用 jp mfa 来获取当前的 MFA

        想要获取更多的信息可以使用 jp --help或者查看脚本文件内容。

- description: a easy connect jumpserver tools or scripts
- usage: 
        1. you can modify the `user.cfg` to adapt your jumpserver
        2. run `jp -h` you will get help info and jp script will re-exc a shell
        3. finally, you can run `jp`. will login jumpserver.
        4. other function: `jp mfa` you can get your MFA Code

        get more information `jp --help` or read source code.
