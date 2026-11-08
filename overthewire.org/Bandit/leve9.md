<img width="1300" height="570" alt="image" src="https://github.com/user-attachments/assets/013cd5c5-3821-4f20-ac5b-c22a419e35f6" />

### Login :
```
ssh bandit8@bandit.labs.overthewire.org -p 2220
```

### Passwd :
```
VR1ljMayciFxbnUokuQmJFw6QC9VKtub
```
### 命令解释：

| 命令            | 作用                                              |
| --------------- | ------------------------------------------------- |
| `sort data.txt` | 把所有行按字母顺序排序（必须先排序才能用 `uniq`） |
| `uniq -u`       | 只显示**只出现一次**的行（`-u` = unique）         |

> 如果用 `uniq` 而不加 `-u`，它会去掉连续重复的行，但不会告诉你哪条是唯一的。

------

### 
