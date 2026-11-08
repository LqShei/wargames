<img width="1305" height="561" alt="image" src="https://github.com/user-attachments/assets/52d2164b-b138-4da4-a8d0-a679d03ca7d9" />

### Login : 
```
ssh bandit2@bandit.labs.overthewire.org -p 2220
```

### passwd :
```
PK8fYLZg2hnHSz83plBL1iEPKdD3QToB
```

<img width="1414" height="384" alt="image" src="https://github.com/user-attachments/assets/005c247a-1edd-4fbf-961a-fa784822afb9" />
<img width="1028" height="154" alt="image" src="https://github.com/user-attachments/assets/19c85136-4b2b-4427-bf6e-285245a1cdfb" />

这里文件名非常特殊，直接输入会导致 Shell 解析出错。

文件实际名称是 --spaces in this filename--。这里有双重障碍：
文件名中间有空格，必须用引号括起来。
文件名以 -- 开头，在 Linux 命令中，-- 通常被当作选项（参数）的标志，所以 cat 以为你要传一个选项给它。

要成功读取这个文件，需要使用命令中的选项分隔符 --，并且结合引号包裹文件名。

在终端输入以下命令：
```
cat -- "--spaces in this filename--"
```
