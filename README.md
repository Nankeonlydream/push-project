# **使用Git命令上传项目**

## 一、设置用户签名（首次执行）

```css
git config --global user.name NanKeOnlyDream

git config --global user.email nankeonlydream@gmail.com
```

## 二、初始化项目（首次执行）

在项目根目录下初始化本地库，命令：

```css
git init
```

## 三、查看仓库状态（非必须）

```css
git status
```

## 四、添加暂存区（重要）

```css
git add
```

### 4.1 删除暂存区内的文件（非必须）

```css
git rm --cached <filename>
```

## 五、将暂存区文件提交到本地库中

```css
git commit -m "first commit" <filename>
```

## 六、查看版本信息日志（用来查看提交次数记录）

```css
git reflog
```

### 6.1 查看详细信息日志（非必须）

```css
git log
```

**注意：如果文件被修改，需要重新提交一遍。（再从第四步开始）**

## 七、版本穿梭（返回指定版本）

```css
git reset --hard version
```

## 八、分支的操作

### 8.1 查看分支

```css
git branch -v
```

### 8.2 创建分支

```css
git branch 分支名
```

### 8.3 切换分支

```css
git checkout 分支名
```

### 8.4 合并分支

```css
git merge 分支名(新内容覆盖旧内容，旧分支内容将保存)。
```

#### 8.4.1 **冲突合并（两个分支在同一个文件同一个位置有两套不同的修改，Git无法替我们决定使用哪一个。必须个人决定新代码内容）。**

## 九、查看别名（方便后期推送拉取项目）

```css
git remote -v
```

### 9.1 创建别名

```css
git remote add 别名+仓库地址
```

## 十、推送项目到Github（重要）

```css
git push 别名 分支
```

## 十一、拉取项目到本地

```css
git pull 别名 分支
```

## 十二、克隆远程仓库到本地

```css
git clone 项目链接
```

## 十三、SSH免密登录

```css
ssh-keygen -t rsa -C 邮箱地址
// 复制C://用户//用户名//.ssh的id_rsa.pub文件中的密钥
找到Github账号设置中SSH and GPG keys，添加一个新的密钥
```

