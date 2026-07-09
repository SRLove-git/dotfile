cat > ~/README.md << 'EOF'
# Dotfiles

My macOS dotfiles managed with a bare Git repository.

## 包含的配置

### ~/.config/
- **btop/** - 系统资源监控
- **fastfetch/** - 系统信息工具
- **fish/** - Fish shell 配置
- **git/** - Git 全局配置
- **kitty/** - Kitty 终端模拟器
- **nvim/** - Neovim 编辑器
- **sketchybar/** - macOS 状态栏
- **skhd/** - 快捷键守护进程
- **starship.toml** - Shell 提示符
- **wezterm/** - WezTerm 终端模拟器
- **yabai/** - 平铺窗口管理器
- **zellij/** - 终端复用器
- **pip/** - Python 包管理器配置
- **tree-sitter/** - Tree-sitter 配置

### Home 目录
- .zshrc, .zshenv, .zprofile
- .p10k.zsh - Powerlevel10k 主题
- .aerospace.toml - Aerospace 窗口管理器
- .vimrc - Vim 配置
- .npmrc - npm 配置
- .bashrc, .bash_profile

## 使用方式

```bash
# 克隆到新机器
git clone --bare git@github.com:SRLove-git/dotfile.git $HOME/.dotfiles

# 设置别名
alias dotfiles='git --git-dir=$HOME/.dotfiles --work-tree=$HOME'

# 检出文件
dotfiles checkout

# 隐藏未跟踪文件
dotfiles config status.showUntrackedFiles no
```
EOF
