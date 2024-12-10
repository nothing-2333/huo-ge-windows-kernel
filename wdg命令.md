# 查看寄存器
r gdtr

# 查看地址的内存，（物理内存要在最前面加！，虚拟内存不用）
## 注意显示出来的内存全是小端序
db/dw/dd/dq gdtr [l 0x20]
## 竖向查看
dds/dqs gdtr [l 0x20]
## 查看物理内存
!dd 3ab6d000
## 显示内存的unicode
!du 3ab6d000

# 查看反汇编
u nt!DbgPrint

# 查看进程信息
!process 0 0