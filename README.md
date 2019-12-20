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

