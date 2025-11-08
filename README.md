count = 0
sum = 0
n = int(input("输入高度："))
# 用于存储每次的弹跳高度
bounce_heights = []
while count < 10:
    if count == 0:
        n /= 2
        # 记录第1次弹跳高度
        bounce_heights.append(n)
        count += 1
    else:
        sum += n * 2
        n /= 2
        # 记录每次弹跳高度
        bounce_heights.append(n)
        count += 1
print(f"10次的总路程为{sum}")
# 输出第10次弹跳的高度
print(f"第10次弹跳的高度为{bounce_heights[9]}")
