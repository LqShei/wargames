<img width="1659" height="453" alt="image" src="https://github.com/user-attachments/assets/809603cc-9904-4a1f-9061-c07ecb7d27f3" />

### Login :
```
ssh bandit4@bandit.labs.overthewire.org -p 2220
```
### Passwd :
```
xzTXq1rDJQVVAzdv5cHq1TQytTWufAMq
```

<img width="1341" height="533" alt="image" src="https://github.com/user-attachments/assets/680a9e36-a5c5-4860-a55a-f6dafb244398" />


这些文件看起来名字都差不多，如果直接用 `cat` 一个个看，有些文件里是乱码（二进制数据）。

题目的提示说密码在一个**“人类可读（human-readable）”**的文件里。在 Linux 中，我们可以使用 `file` 命令来查看文件的真实类型，而不是被文件名迷惑。

请按照以下步骤操作：

### 查看文件类型
在终端中输入以下命令：
```bash
file ./*
```
**运行结果：**
你会发现大部分文件显示为 `data`（二进制数据），只有其中一个文件会显示为 **`ASCII text`**。

<img width="756" height="436" alt="image" src="https://github.com/user-attachments/assets/35651547-8e06-4096-bb59-e352d3126fab" />


