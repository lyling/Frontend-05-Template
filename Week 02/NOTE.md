# 学习笔记

## 绘制地图

- 生成100x100(个单元格)地图
- 绘制路线
  - 单元格捕捉mousemove事件
  - 如果当前鼠标左键为按下状态
    - 设置当前单元格在数组中的值为1
    - 设置当前单元格元素背景颜色
  - 如果当前鼠标右键为按下状态
    - 设置当前单元格在数组中的值为0
    - 清除当前单元格元素背景颜色

## 寻路(广度优先)

- 从起点开始(出列) 寻找有路径的(值为1)相邻(8向)单元格,并移动
- 将相邻(8向)可移动的单元格的加入队列(入列)
- 从队列中取出第一个, 继续重复上述步骤, 直到队列为空
- 深度优先这使用堆栈

## 查找路径

- 标记前驱节点

## 启发式函数优化(A*)

- 添加优先级计算函数(启发式函数)