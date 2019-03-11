import random

# 1. 接收用户输入的拳
player = int(input("请出拳 石头(1) 剪刀(2) 布(3):"))

# 2. 让电脑随机出拳 [1，3]随机范围数字
computer = random.randint(1, 3)

print("电脑出拳:", computer)
# 3. 比较胜负

# 补充： 如果判断的条件比较大并且还是一个整体，那么可以把条件判断放到小括号里面， 语意更加明确
if (player == 1 and computer == 2) or (player == 2 and computer == 3) or (player == 3 and computer == 1):
    print("您赢了，电脑输了")
elif player == computer:
    print("平局")
else:
    print("您输了，电脑赢了")
