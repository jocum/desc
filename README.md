# 环境文档

## item

### 1. Homebrew  
  > homebrew 是mac 的软件包管理工具可以极大的方便各种软件包的安装 
  > 官方网站 [https://brew.sh/](https://brew.sh/)
  * 安装
  ```
    /bin/zsh -c "$(curl -fsSL https://gitee.com/cunkai/HomebrewCN/raw/master/Homebrew.sh)"
  ```
  >> #官方安装会报443错误 这里用国内镜像安装
### 2. Oh My Zsh
  > Oh My Zsh 是一个令人愉快的开源社区驱动框架，用于管理您的 Zsh 配置。它捆绑了数以千计的有用功能、帮助程序、插件、主题和一些让您大喊大叫的东西.....
  > Oh My Zsh 需要先安装zsh
  > 官方网站 [https://ohmyz.sh/](https://ohmyz.sh/)
  > github  [https://github.com/ohmyzsh/ohmyzsh](https://github.com/ohmyzsh/ohmyzsh)
  * 安装
  ```
    sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
  ```
### 3. powerlevel10k
  > p10k 是oh my zsh 的一个主题可以让你的窗口看起来更合适自己的审美 可以通过命令自己配置
  > github [https://github.com/romkatv/powerlevel10k][https://github.com/romkatv/powerlevel10k]
  * 安装
  ```
    git clone --depth=1 https://gitee.com/romkatv/powerlevel10k.git ~/powerlevel10k echo 'source ~/powerlevel10k/powerlevel10k.zsh-theme' >>~/.zshrc
  ```
  > 这里默认已经安装了 Oh My Zsh  
  * 安装字体库支持
  > 这里使用的是 Nerd fonts   
  > github [https://github.com/ryanoasis/nerd-fonts](https://github.com/ryanoasis/nerd-fonts)
  ```
    #这里只介绍mac 的  brew 安装方式 其他安装请看github
    brew tap homebrew/cask-fonts
    brew install --cask font-hack-nerd-font
  ```
  * 配置字体库
   1. 安装完成后 去命令行窗口 属性配置中 选择 Hack nerd font 字体
      打开窗口-> 选择终端 -> 偏好设置 -> 描述文件 -> 文本 -> 字体  更改      
      运行 p10k  configure 配置你的样式
