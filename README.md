# 学生成绩管理系统

## 项目简介

学生成绩管理系统是一个基于Qt C++开发的桌面应用程序，旨在为教育机构提供全面的学生成绩管理解决方案。该系统集成了数据管理、成绩分析、AI辅助功能等多种特性。

## 功能特性

### 🎯 核心功能
- **用户认证系统**：支持登录/注册功能，确保数据安全
- **学生信息管理**：完整的学生档案管理
- **成绩管理**：成绩录入、修改、查询功能
- **数据搜索**：快速搜索学生和成绩信息
- **成绩分析**：提供详细的成绩统计和分析报告

### 📊 分析功能
- **成绩分析模块**：统计分析学生成绩分布
- **专业分析模块**：按专业维度进行成绩对比分析
- **图表展示**：使用Qt Charts提供可视化数据展示

### 🤖 AI辅助功能
- **AI聊天窗口**：智能对话功能
- **AI成绩分析**：基于AI的成绩预测和分析
- **智能建议**：为教学提供AI驱动的建议

### ⚙️ 基础设置
- **管理员管理**：系统管理员功能
- **班级设置**：班级信息配置
- **专业设置**：专业信息管理
- **科目设置**：科目信息配置

## 技术栈

- **开发语言**：C++ (C++17标准)
- **UI框架**：Qt 6.x
- **数据库**：SQL数据库支持
- **图表库**：Qt Charts
- **网络功能**：Qt Network

## 项目结构

```
StudentScoreManagement/
├── AIModel/           # AI模型相关功能
├── Analysis/          # 数据分析模块
├── BaseSettings/      # 基础设置模块
├── DataManage/        # 数据管理模块
├── DataObjects/       # 数据对象定义
├── DataSearch/        # 数据搜索功能
├── build/            # 构建输出目录
├── data/             # 数据文件
├── images/           # 图像资源
├── dashboard.cpp/h   # 主面板
├── loginwindow.cpp/h # 登录窗口
├── registerwindow.cpp/h # 注册窗口
├── main.cpp          # 程序入口
└── *.ui              # UI界面文件
```

## 环境要求

### 开发环境
- **Qt版本**：Qt 6.0 或更高版本
- **编译器**：支持C++17的编译器
  - Windows: MSVC 2019+ 或 MinGW
  - Linux: GCC 7+ 或 Clang 6+
  - macOS: Xcode 10+

### 依赖库
- Qt Core
- Qt GUI
- Qt Widgets
- Qt SQL
- Qt Charts
- Qt Network

## 安装与编译

### 1. 克隆项目
```bash
git clone <repository-url>
cd StudentScoreManagement
```

### 2. 使用Qt Creator编译
1. 打开Qt Creator
2. 选择"打开项目"
3. 选择`StudentScoreManagement.pro`文件
4. 配置构建套件
5. 点击"构建"按钮

### 3. 命令行编译
```bash
qmake StudentScoreManagement.pro
make  # Windows上使用 nmake 或 mingw32-make
```

## 使用说明

### 首次运行
1. 启动应用程序
2. 系统会自动初始化数据库
3. 使用注册功能创建管理员账户
4. 登录系统开始使用

### 基本操作
1. **登录系统**：输入用户名和密码
2. **学生管理**：添加、编辑、删除学生信息
3. **成绩录入**：为学生录入各科成绩
4. **数据查询**：搜索和筛选学生及成绩信息
5. **成绩分析**：查看统计分析报告

## 数据库配置

系统默认使用SQLite数据库，数据文件存储在`data/`目录下。如需配置其他数据库，请修改`DataObjects/dataobject.cpp`中的数据库连接设置。

## 开发说明

### 代码结构
- `DataObjects/`：定义了所有数据模型类（学生、成绩、班级等）
- `DataManage/`：数据管理业务逻辑
- `DataSearch/`：搜索功能实现
- `Analysis/`：数据分析和统计功能
- `AIModel/`：AI相关功能模块
- `BaseSettings/`：系统设置和配置

### 扩展开发
- 添加新的数据模型：在`DataObjects/`目录下创建相应的类
- 添加新的功能模块：创建对应的窗口类和UI文件
- 修改数据库结构：更新相应的数据对象类

## 贡献指南

1. Fork 本项目
2. 创建特性分支 (`git checkout -b feature/AmazingFeature`)
3. 提交更改 (`git commit -m 'Add some AmazingFeature'`)
4. 推送到分支 (`git push origin feature/AmazingFeature`)
5. 打开Pull Request

## 许可证

本项目采用开源许可证，具体信息请查看LICENSE文件。

## 联系方式

如有问题或建议，请通过以下方式联系：
- 提交Issue
- 发送邮件至：[your-email@example.com]

## 更新日志

### v1.0.0
- 初始版本发布
- 基本的学生成绩管理功能
- 数据分析和AI辅助功能
- 完整的用户界面

---

感谢使用学生成绩管理系统！ 