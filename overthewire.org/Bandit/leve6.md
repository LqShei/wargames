<img width="1351" height="517" alt="image" src="https://github.com/user-attachments/assets/876344fc-b9b2-427c-823e-627fcae9fdd4" />

### Login :
```
ssh bandit5@bandit.labs.overthewire.org -p 2220
```

### Passwd :
```
6C7h9GD8M6ai5nr7wo1RonrzFjj9yIrG
```
<img width="961" height="854" alt="image" src="https://github.com/user-attachments/assets/f2942951-ee3b-4548-9a59-71fa8035e864" />

这一关的目标是在 `inhere` 目录下，找到一个同时满足以下三个条件的文件：
1. **人类可读** (human-readable)
2. **大小正好是 1033 字节** (1033 bytes in size)
3. **不可执行** (not executable)


### 使用 find 命令按条件查找
在终端中输入以下命令：
```bash
find . -type f -size 1033c
```
**命令拆解说明：**
* `find .` ：在当前目录（`.`）下开始查找。
* `-type f` ：限定只查找普通**文件**（f 代表 file，排除目录）。
* `-size 1033c` ：限定文件大小**正好是 1033 字节**（c 代表 bytes）。

<img width="1429" height="378" alt="image" src="https://github.com/user-attachments/assets/781d3d3c-b5dc-495b-9a47-5348649b44a7" />

根据题目要求，密码文件满足：

- 在 `inhere` 目录下
- 普通文件（`-f`）
- 大小正好为 **1033 字节** → 使用 `-size 1033c`
- **非可执行** → 使用 `! -executable` 或 `-perm` 判断权限
- **人类可读** → 可用 `file` 命令判断是否为文本文件

------

### 
