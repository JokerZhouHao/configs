## IdeaVim配置

### 说明
插件位置C:\Users\Monica\.GoLand2018.2\config\plugins\IdeaVim\，使用的IDEA软件是GoLand 2018.02，[下载](./files/IdeaVim.zip)。

### ideavimrc文件配置
``` java
set showmode
" Insert mode shortcut
"inoremap <C-h> <Left>
"inoremap <C-j> <Down>
"inoremap <C-k> <Up>
"inoremap <C-l> <Right>
inoremap <C-a> <Home>
inoremap <C-e> <End>
inoremap <C-d> <Delete>

" 弹出输入框，可以跳到指定类
nnoremap <Space>gc :action GotoClass<CR>
" 弹出输入框，跳转到指定操作
nnoremap <Space>ga :action GotoAction<CR>
" 跳转到定义
nnoremap <Space>gd :action GotoDeclaration<CR>
" 跳转到实现
nnoremap <Space>gi :action GotoImplementation<CR>
" 跳转到指定的文件
nnoremap <Space>gf :action GotoFile<CR>
" 跳转到方法的声明
nnoremap <Space>gs :action GotoSuperMethod<CR>
" 跳转到测试
nnoremap <Space>gt :action GotoTest<CR>
" 跳转到变量的声明
nnoremap <Space>gS :action GotoSymbol<CR>

" 查找使用
nnoremap <Space>fu :action FindUsages<CR>
" 显示使用
nnoremap <Space>su :action ShowUsages<CR>

" 前进，相当似于eclipse中的alt+方向右键
nnoremap gf :action Forward<CR>
" 后退，相当于eclipse中的alt+方向左键
nnoremap gb :action Back<CR>
```

### idea系列软件设置
* setting > keymap，将上下左右改为Ctrl<k, j, h, l>