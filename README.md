shy_hardware是一个16位计算机<br>
它包含一个20hz的处理器<br>
63488字节的内存<br>
1920字节的可用存储<br>
剩余128字节的寻址空间用于寄存器等<br>
属于[shy_project](https://github.com/Shyliuli/shy_project/)
下面是地址表：


| 0x00-0x0a     | 寄存器ax，bx，cx.....px |
| --------------- | ------------------------- |
| 0x0a-0x0F     | 保留                    |
| 0x10-0x1F     | 内建命令使用            |
| 0x20-0xF820   | 内存                    |
| 0xF820-0xFFA0 | 存储                    |
| 0xFFA0-0xFFFF | 保留                    |

内建命令（具体内容见shy_language）：


| 命令 | 地址 | 命令  | 地址 |
| ------ | ------ | ------- | ------ |
| add  | 0x10 | mov   | 0x18 |
| sub  | 0x11 | reset | 0x19 |
| sl   | 0x12 | cpe   | 0x1A |
| rl   | 0x13 | in    | 0x1B |
| and  | 0x14 | out   | 0x1C |
| or   | 0x15 | jmp   | 0x1D |
| xor  | 0x16 | equ   | 0x1E |
| nor  | 0x17 | set   | 0x1F |
