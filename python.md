# 基础语法
## 参数
```python
def test(*arg,**args):
    print(arg)
    print("------------------------")
    print(args)
    
test(1,2,a=5,b=6)
# (1, 2)
# ------------------------
# {'a': 5, 'b': 6}
```
## 输出
```python
name = "Alice"
age = 25
print("My name is %s and I am %d years old." % (name, age))  # 使用 % 进行格式化
# My name is Alice and I am 25 years old.
data_i = "a"
name1 = "11"
text = "{%s}:{%s}" %(data_i,name1)
print(text)
# {a}:{11}
print("My name is {} and I am {} years old.".format(name, age))  # 使用 format() 方法进行格式化
# My name is Alice and I am 25 years old.
print(f"My name is {name} and I am {age} years old.")  # 使用 f-string 
# My name is Alice and I am 25 years old.
# \n \t \\ \' \" \r \b \v 
print("Hello,\nWorld!")
# Hello,
# World!
print("Name:\tAlice")
# Name:   Alice
print("This is a backslash: \\")
# This is a backslash: \
print("He said, \"Hello!\"")
# He said, "Hello!"
print('She\'s happy.')
# She's happy.
print("Hello\rWorld!")  # 输出后将光标移至行首
# World!
print("Hello\bWorld!")  # 输出后删除前一个字符
# HellWorld!
print("Hello\vWorld!")  # 输出后垂直制表符
# Hello
#      World!
```

# IDE使用
## vscode
1. JustMyCode设置无用，launch增加"purpose":["debug-in-terminal"]
```python
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: 当前文件",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "console": "integratedTerminal",
            "justMyCode": false,
            "purpose":["debug-in-terminal"]
        }
    ]
}

```