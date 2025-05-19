# vscode debug(Attach to Procoess)
Run and Debug ==> create a launch.json file ==> CMake Debugger ==> Attach ==> 创建配置文件
```
# 配置文件参考
{
    // Use IntelliSense to learn about possible attributes.
    // Hover to view descriptions of existing attributes.
    // For more information, visit: https://go.microsoft.com/fwlink/?linkid=830387
    "version": "0.2.0",
    "configurations": [
        {
            "name": "(gdb) 附加",
            "type": "cppdbg",
            "request": "attach",
            "processId":"${command:pickProcess}", 
            "program": "/opt/xxx/Agent/xxx",
            "MIMode": "gdb",
            "setupCommands": [
                {
                    "description": "为 gdb 启用整齐打印",
                    "text": "-enable-pretty-printing",
                    "ignoreFailures": true
                },
                {
                    "description": "将反汇编风格设置为 Intel",
                    "text": "-gdb-set disassembly-flavor intel",
                    "ignoreFailures": true
                }
            ]
        }

    ]
}
```
