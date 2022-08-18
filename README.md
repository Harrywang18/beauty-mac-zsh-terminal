# beauty-mac-zsh-terminal
### 美化增强mac终端zsh
美化并增强Mac终端后的效果如图所示，对于输入正确的命令会变色，输入命令开头字符，自动提示输入过的命令。实现方式如下：
### 切换默认终端为zsh
从```MacOS Catalina```开始默认终端已经是```zsh```。
使用```echo $SHELL```可以查看当前终端，如果不是```/bin/zsh```，执行以下命令切换到```zsh```，否则跳过此步。
```bash
chsh -s /bin/zsh
```
### 安装
#### 下载oh-my-zsh
```bash
git clone https://github.com/robbyrussell/oh-my-zsh.git ~/.oh-my-zsh
```

#### 创建一个新的配置文件
```bash
cp ~/.oh-my-zsh/templates/zshrc.zsh-template ~/.zshrc
```

#### 授权，如果不授权每次会有警告
```bash
chmod 755 /usr/local/share/zsh
chmod 755 /usr/local/share/zsh/site-functions
