<img width="2191" height="579" alt="image" src="https://github.com/user-attachments/assets/151cbb24-67d3-48ff-a3b1-9c331cbd5da0" />
### Login :
```
ssh bandit12@bandit.labs.overthewire.org -p 2220
```

### Passwd :
```
GROozWPO8QyN0mGrjUkID0WCYkZiQxrN
```

```sh
# 2. 使用 xxd -r 将 hexdump 转为二进制
xxd -r data.txt > re.txt

# 3. 查看文件类型
file re.txt
# 输出：gzip compressed data → 是个 .gz 文件

# 4. 改名为 .gz 后缀再解压
mv re.txt re.gz
gzip -d re.gz

# 5. 此时得到 re，查看类型：
file re
# 输出：bzip2 compressed data → 是个 .bz2 文件

# 6. 改名并解压 bzip2
mv re re.bz2
bzip2 -d re.bz2

# 7. 又得到 re，再看类型：
file re
# 输出：gzip compressed data → 又是 .gz！

# 8. 继续改名解压
mv re re.gz
gzip -d re.gz

# 9. 再看：
file re
# 输出：POSIX tar archive → 是个 .tar 包

# 10. 解包
tar -xvf re
# 得到 data5.bin

# 11. 继续查看和解包（因为 file 显示仍是 tar）
file data5.bin
# 输出：POSIX tar archive
tar -xvf data5.bin
# 得到 final.txt 或类似文件

# 12. 查看内容
cat <最终文件>
FO5dwFsc0cbaIiH0h8J2eUks2vdTDwAn
```
<img width="1256" height="1515" alt="image" src="https://github.com/user-attachments/assets/61e6eb7c-cbf8-4373-8140-6d789ac49ec7" />

<img width="1258" height="1126" alt="image" src="https://github.com/user-attachments/assets/556d9c2a-d935-432a-a41e-9468eb8ce36e" />
