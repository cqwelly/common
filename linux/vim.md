## 分屏
vim的分屏功能
总结起来，基本都是ctrl+w然后加上某一个按键字母，触发一个功能。
- 在shell里打开几个文件并且分屏:
  - vim -On file1 file2 ...
  - vim -on file1 file2 ...
    大O表示垂直分割(vertical)，小o表示水平分割（默认horizontal），后面的n表示分几个屏，实际上我觉得不用写，默认按后面要分割的文件数来决定分几个屏。
- 在vim里打开一个分屏:
  - 创建空白分屏：
  - :new 打开任意文件：
  - :vsplit(:vsp) filename
  - :sp(split) filename
  - 打开当前文件：ctrl+w 和 s(split) ctrl+w 和 v(vsplit)
- 关闭一个分屏:
  - :only 或者 ctrl+w 和 o取消其它分屏，只保留当前分屏
  - ctrl+w 和 c(close)
  - 只剩最后一个分屏以后推出： ctrl+w 和 q(quit)
- 移动光标，也就是切换分屏；也可以移动分屏，比如将左分屏移动到右边。
  - ctrl+w 和 w（各种切换，只有两个分屏的时候还是比较方便的）
  - ctrl+w 和 h(H) 左
  - ctrl+w 和 j(J) 下
  - ctrl+w 和 k(K) 上
  - ctrl+w 和 l(L) 右
- 最后就是改变分屏尺寸的操作了。
  - ctrl+w 和 < 左
  - ctrl+w 和 > 右
  - ctrl+w 和 + 上
  - ctrl+w 和 - 下
  - ctrl+w 和 = 恢复均等
  
