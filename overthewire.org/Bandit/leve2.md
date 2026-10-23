<img width="1255" height="581" alt="image" src="https://github.com/user-attachments/assets/8d3e9002-f883-4b4a-9463-9b1de577a6a7" />
The password for the next level is stored in a file called - located in the home directory
## Login

```
ssh bandit1@bandit.labs.overthewire.org -p 2220
```
passwd : 6y2kwnwK6grgvwvpvLaa2T1cpFEKOhNR
Solution :
<img width="1186" height="228" alt="image" src="https://github.com/user-attachments/assets/4ca00e29-c6fd-454f-af3a-450afe8438f4" />
‘-’ 是 Linux 中的一个特殊符号。因此，不建议用这个符号作为文件名的开头。
‘-’ 是标准选项字符。我们已经见过它用于为命令添加特定选项的所谓标志（比如 ssh 命令中用于选择端口的 -p 标志）。
标准选项。正因如此，以该符号作为第一个字符的文件不能像其他文件那样直接被引用。
