# Vim Config
# 插件安装
# 1.下载Vundle
        git clone https://github.com/VundleVim/Vundle.vim.git ~/.vim/bundle/Vundle.vim
# 2.配置Vundle
        创建 ~/.vimrc 文件，以通知 Vim 使用新的插件管理器。安装、更新、配置和移除插件需要这个文件。

        touch ~/.vimrc
        在此文件顶部，加入如下若干行内容：
	
# 3.安装
        打开vim:
        vim
        键入下列命令安装插件：
        :PluginInstall
        或者在终端使用如下命令:
	vim +PluginInstall +qall

#####version2.0
# 步骤1   安装vundle
git clone https://github.com/gmarik/vundle.git ~/.vim/bundle/vundle

# 步骤2:  .vimrc 配置文件
filetype off
set rtp+=~/.vim/bundle/vundle/
call vundle#rc()
 
if filereadable(expand("~/.vimrc.bundles"))
  source ~/.vimrc.bundles
endif

# 步骤3:   .vimrc.bundles 配置文件
为了方便管理插件安装插件代码放置在这个文件中，首先创建 .vimrc.bundles 配置文件

if &compatible
  set nocompatible
end
 
filetype off
set rtp+=~/.vim/bundle/vundle/
call vundle#rc()
 
" Let Vundle manage Vundle
Bundle 'gmarik/vundle'
 
" Define bundles via Github repos
" 标签导航
Bundle 'majutsushi/tagbar'
Bundle 'vim-scripts/ctags.vim'
" 静态代码分析
Bundle 'scrooloose/syntastic'
" 文件搜索
Bundle 'kien/ctrlp.vim'
" 目录树导航
Bundle "scrooloose/nerdtree"
" 美化状态栏
Bundle "Lokaltog/vim-powerline"
" 主题风格
Bundle "altercation/vim-colors-solarized"
" python自动补全
Bundle 'davidhalter/jedi-vim'
Bundle "klen/python-mode"
" 括号匹配高亮
Bundle 'kien/rainbow_parentheses.vim'
" 可视化缩进
Bundle 'nathanaelkane/vim-indent-guides'
if filereadable(expand("~/.vimrc.bundles.local"))
  source ~/.vimrc.bundles.local
endif
 
filetype on

# 步骤4:   安装插件
shell中输入vim，进入命令模式输入 BundleInstall
1.shell中输入 vim
2.vim命令模式输入 BundleInstall


# 步骤5:   插件配置
.vimrc文件中插入代码在同目录下：


# 步骤6:   运行配置
在～/.vimrc最后一行追加如下代码：

" 运行文件
map <F5> :w<cr>:r!python3 %<cr>

