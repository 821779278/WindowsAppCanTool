# Cantool Windows APP 项目需求文档

> 小组成员：胡庆庆，张德胜，李耀，王杰

## 图表分析
![用例图](http://om0ttwn6c.bkt.clouddn.com/%E4%BE%8B%E5%9B%BEcantool.png)

## 详细需求分析

### 基本设置

- 在 windows 平台下建立可视化的带有 GUI 界面的Windows app , 能够很好的完成展示用户要求的信息

- 在弹出式的 ComBox 中实现以下功能
  - 以下拉列表形式选择本机可用 COM 口
  - 设定相应 COM 口的波特率 115200, 数据位数 8, 停止位数 1 , 保存在设定文件中

### CAN 信息接收

- 实现 CAN 装置的速率设置 , 工作状态 (open) 设置 , 初始化状态 (Close) 设置, 保存在设定文件中

- 对接收到的 CAN 信息进行及 CAN 信号数据库进行解析 ,  并将 CAN 信息原始数据进行显示

- CAN 信息显示要求有仪表盘 , LED 等自制控件 , 保存用户选择显示方式到设定文件中

- 绘制 CAN 信号实时变化物理值

- 能够将 CAN 信息数据实时保存为 csv 数据文件

### CAN 信息发送

- 允许用户指定要发送 CAN 信息中的 CAN 信号物理值和 CAN 信息发送周期

- app 能够将用户设定的 CAN 物理值整合为 CAN 信息发送给CANTOOL 装置

### 加载信息

- 在 GUI 界面显示用户提供的 CAN 信号和信息数据库

- CAN 信息和 CAN 信号数据库可以存为 xml 和 JSON 格式也可从 JSON 和 xml 格式转换为 CAN 信息和信号数据库

### 远程数据共享

- 通过 WEB API 方式将 CAN 信息更新到远程数据库 , CanTool App 能够与远程 Web Api 进行数据交换。（此功能本学期不做）

### 功能变更

- 最好变更管理