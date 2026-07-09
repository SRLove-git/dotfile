∙ # Dotfiles
∙ 
∙ 我的 macOS 开发环境配置，使用 Bare Git Repository 管理。
∙ 
∙ > 仓库地址：https://github.com/SRLove-git/dotfile
∙ 
∙ ## 目录
∙ 
∙ - [窗口管理](#窗口管理)
∙ - [终端模拟器](#终端模拟器)
∙ - [Shell 环境](#shell-环境)
∙ - [编辑器](#编辑器)
∙ - [状态栏](#状态栏)
∙ - [系统工具](#系统工具)
∙ - [开发工具配置](#开发工具配置)
∙ - [使用方式](#使用方式)
∙ 
∙ ---
∙ 
∙ ## 窗口管理
∙ 
∙ ### yabai — 平铺窗口管理器
∙ 
∙ yabai 是一个 macOS 上的平铺窗口管理器，本配置使用 **bsp（二叉空间分
割）** 布局。
∙ 
∙ **配置文件：** `~/.config/yabai/yabairc`
∙ 
∙ **核心特性：**
∙ - BSP 平铺布局，自动管理窗口位置和大小
∙ - 窗口间隙 10px，内边距 8px
∙ - 窗口透明度：聚焦窗口 1.0，非聚焦窗口 0.8
∙ - 动画持续时间 0.5s，缓动函数 `ease_out_quint`
∙ - 聚焦窗口边框高亮色 `#9dd274`
∙ 
∙ **窗口排除规则：**
∙ >....                                                              
**配置文件：** `~/.config/fish/config.fish`

**配置内容：**
- Conda 初始化（Anaconda 环境支持）

---

### Starship — 跨 Shell 提示符

Starship 是一个轻量级、高度可定制的 Shell 提示符，支持所有 Shell。

**配置文件：** `~/.config/starship.toml`

**提示符布局（Catppuccin Mocha 色系）：**
∙ >....                                                              
**配置文件：** `~/.config/pip/pip.conf`

```ini
[global]
index-url = https://mirrors.ustc.edu.cn/pypi/web/simple
```

配置了 USTC 镜像源，加速 Python 包下载。

### Git 全局配置

**配置文件：** `~/.config/git/ignore`

配置了全局 Git 忽略规则：
∙ >....                                                              
# 提交更改
dotfiles commit -m "Update btop config"

# 推送
dotfiles push
```

### 注意

- 执行 `dotfiles checkout` 时，如果当前系统已有同名配置文件会被覆盖，建议先备份
- `.ssh/` 等敏感目录不纳入版本控制
- `.gitconfig` 不上传（个人信息）
