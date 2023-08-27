## 回声显示
```
echo hello world
```
## 创建文件
```
touch file
echo Hello world > hello.txt  -- 把内容写进文件里，输出内容会覆盖之前的内容
echo Hello world >> hello.txt -- 输出内容添加到文件内容的末尾，不会覆盖之前的内容
```
## 查看文件内容
```
cat hello.txt
cat -b main.js  -- 查看的文件内容显示行号
```

## 删除文件
```
rm textA.txt
```
批量删除
```
rm *.txt
rm a*  -- 删除都是以a开头的文件
```
## 重命名/移动文件
```
mv old_file_name new_file_name
mv abc.txt/   -- 将abc.txt移到根目录下
mv abc.txt/cd.txt   -- 将abc.txt移到根目录下并改名成cd.txt
```
## 创建/删除目录
```
mkdir text
rmdir text
```
删除/创建多级目录
```
mkdir -p workspace/demo/test
rmdir workspace/demo/test  -- 只会删掉test
rmdir -p workspace/demo/test  -- 如果这些目录中有任何一个目录不为空,那么删除操作就会停止在第一个不为空的目录上,不会继续往上递归删除
rmdir -rf workspace -- 强制递归删除workspace
```
