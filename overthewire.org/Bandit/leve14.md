<img width="2188" height="694" alt="image" src="https://github.com/user-attachments/assets/67ee61c5-8fd1-4195-b421-4ea4ec8fff9e" />

### Login :

```
ssh bandit13@bandit.labs.overthewire.org -p 2220
```

### Passwd :

```
qQYQiHOBPR8zR61qxYqX45quvihF2uzk
```


```
# 下载密钥
scp -P 2220 bandit13@bandit.labs.overthewire.org:sshkey.private .
```

```
# 使用密钥登录
ssh -i sshkey.private bandit14@bandit.labs.overthewire.org -p 2220
```

```
# 查看密钥
```

<img width="842" height="99" alt="image" src="https://github.com/user-attachments/assets/67b480c1-93d9-4a5f-a218-c86b8ddd5996" />
