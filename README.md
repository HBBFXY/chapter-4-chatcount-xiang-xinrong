def count_characters():
    """
    统计输入字符串中英文字符、数字、空格和其他字符的数量
    """
    # 从键盘获取输入
    text = input("请输入一行字符：")
    
    # 初始化计数器
    english_chars = 0  # 英文字符计数
    digits = 0         # 数字计数
    spaces = 0         # 空格计数
    others = 0         # 其他字符计数
    
    # 遍历字符串中的每个字符
    for char in text:
        # 判断是否为英文字符（字母）
        if char.isalpha():
            english_chars += 1
        # 判断是否为数字
        elif char.isdigit():
            digits += 1
        # 判断是否为空格
        elif char.isspace():
            spaces += 1
        # 其他字符
        else:
            others += 1
    
    # 按照要求的格式输出结果
    print(f"英文字符：{english_chars}")
    print(f"数字：{digits}")
    print(f"空格：{spaces}")
    print(f"其他字符：{others}")

# 调用函数执行统计
if __name__ == "__main__":
    count_characters()
