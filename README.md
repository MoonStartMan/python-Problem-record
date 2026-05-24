# python-Problem-record

[![GitHub stars](https://img.shields.io/github/stars/MoonStartMan/python-Problem-record?style=social)](https://github.com/MoonStartMan/python-Problem-record/stargazers)
[![GitHub forks](https://img.shields.io/github/forks/MoonStartMan/python-Problem-record?style=social)](https://github.com/MoonStartMan/python-Problem-record/network)
[![Python Version](https://img.shields.io/badge/python-3.6+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)

> Python 学习过程中的问题记录、踩坑经验与解决方案汇总。

## 项目简介

本仓库记录了在学习 Python 过程中遇到的各种问题、错误以及对应的解决方案。涵盖 Python 基础语法、标准库使用、第三方库集成、性能优化等多个方面。旨在帮助 Python 学习者避开常见陷阱，提高开发效率。

## 学习内容概述

### 计划涵盖的主题

- **基础语法问题**：变量作用域、可变/不可变对象、深浅拷贝等
- **数据结构**：列表、字典、集合的高级用法与陷阱
- **函数与类**：装饰器、闭包、继承、魔术方法等
- **文件操作**：文件读写、编码问题、路径处理
- **异常处理**：异常捕获、自定义异常、最佳实践
- **模块与包**：导入机制、`__init__.py`、相对导入
- **并发编程**：多线程、多进程、异步编程
- **性能优化**：代码优化技巧、Profiling 工具使用
- **第三方库**：常用库的使用问题与解决方案

## 目录结构

```
python-Problem-record/
├── README.md                          # 项目说明文档
├── 基础语法/                           # Python 基础语法问题
│   ├── 变量作用域.md
│   ├── 可变与不可变对象.md
│   └── 深浅拷贝.md
├── 数据结构/                           # 数据结构相关问题
│   ├── 列表操作技巧.md
│   ├── 字典使用陷阱.md
│   └── 集合运算.md
├── 函数与类/                           # 函数和面向对象
│   ├── 装饰器详解.md
│   ├── 闭包与作用域.md
│   └── 类的特殊方法.md
├── 文件与IO/                          # 文件操作
│   ├── 编码问题处理.md
│   └── 路径操作最佳实践.md
├── 异常处理/                           # 异常处理
│   └── 异常处理最佳实践.md
├── 模块与包/                           # 模块系统
│   └── 导入机制详解.md
└── 实用技巧/                           # 实用技巧汇总
    └── Pythonic写法.md
```

## 学习进度

| 模块 | 状态 | 完成度 | 说明 |
|------|------|--------|------|
| 基础语法 | 计划中 | 0% | 待添加 |
| 数据结构 | 计划中 | 0% | 待添加 |
| 函数与类 | 计划中 | 0% | 待添加 |
| 文件与 IO | 计划中 | 0% | 待添加 |
| 异常处理 | 计划中 | 0% | 待添加 |
| 模块与包 | 计划中 | 0% | 待添加 |
| 并发编程 | 计划中 | 0% | 待添加 |
| 性能优化 | 计划中 | 0% | 待添加 |

## 知识点预览

### 可变 vs 不可变对象

```python
# 不可变对象
a = 1
b = a
a = 2
print(b)  # 输出: 1

# 可变对象
list1 = [1, 2, 3]
list2 = list1
list1.append(4)
print(list2)  # 输出: [1, 2, 3, 4]
```

### 深浅拷贝

```python
import copy

# 浅拷贝
shallow = copy.copy(original)

# 深拷贝
deep = copy.deepcopy(original)
```

### 装饰器基础

```python
def my_decorator(func):
    def wrapper(*args, **kwargs):
        print("函数执行前")
        result = func(*args, **kwargs)
        print("函数执行后")
        return result
    return wrapper

@my_decorator
def say_hello():
    print("Hello!")
```

### 列表推导式

```python
# 基本用法
squares = [x**2 for x in range(10)]

# 带条件
evens = [x for x in range(10) if x % 2 == 0]

# 字典推导式
square_dict = {x: x**2 for x in range(5)}
```

## 贡献指南

欢迎提交 Issue 和 Pull Request 来完善本仓库！

### 如何贡献

1. **问题分享**：遇到 Python 相关问题，欢迎记录并分享
2. **方案补充**：对已有问题提供更优解决方案
3. **内容审核**：帮助检查文档中的错误

### 提交规范

- 问题描述清晰，包含环境信息（Python 版本、操作系统）
- 提供最小可复现代码示例
- 解决方案经过验证
- 使用 Markdown 格式编写文档

### 文档格式

```markdown
## 问题描述
简要描述遇到的问题

## 环境信息
- Python 版本: 3.x
- 操作系统: Windows/Linux/macOS

## 代码示例
```python
# 问题代码
```

## 解决方案
```python
# 修复后的代码
```

## 原因分析
解释问题产生的原因

## 参考链接
- [相关文档链接]
```

## 许可证

本项目采用 [MIT](LICENSE) 许可证开源。

## 推荐资源

- [Python 官方文档](https://docs.python.org/zh-cn/3/)
- [Python Cookbook](https://dabeichen.readthedocs.io/)
- [Fluent Python](https://book.douban.com/subject/26278021/)
- [LeetCode Python 题解](https://leetcode.cn/)

## 相关仓库

- [C-Problem-Record](https://github.com/MoonStartMan/C-Problem-Record) - C 语言问题记录
- [JavaScript-data-structures-and-algorithms](https://github.com/MoonStartMan/JavaScript-data-structures-and-algorithms) - JavaScript 算法

## 致谢

- 感谢所有提供问题和解决方案的朋友
- 感谢 Python 社区的优质资源

---

**作者**: [MoonStartMan](https://github.com/MoonStartMan)  
**维护**: 持续更新中
