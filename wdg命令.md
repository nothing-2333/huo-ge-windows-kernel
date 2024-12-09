# 查看寄存器
r gdtr

# 查看地址的内存
## 注意显示出来的内存全是小端序
db/dw/dd/dq gdtr [l 0x20]
## 竖向查看
dds/dqs gdtr [l 0x20]

# 查看反汇编
u nt!DbgPrint