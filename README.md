# 🚀 Telegram 举报工具

一个支持多账号批量举报的 Telegram 工具。

## 📥 部署教程 (Windows)

### 1. 安装 Python 🐍
- 下载：https://www.python.org/downloads/
- 安装时必须勾选 "Add Python to PATH"
- 点击 "Install Now"

### 2. 安装依赖 📦
- Win+R 输入 `cmd` 回车
- 输入下面代码回车：
```bash
pip install telethon
```

### 3. 创建工作目录 📁
1. 在电脑D盘创建文件夹 `telegram_report`
2. 在里面创建 `sessions` 文件夹
3. 把 `TelegramReportUserScript.py` 放进去
4. 把协议号导入到 `sessions` 文件夹

### 4. 修改API信息 🔑
- 打开 `TelegramReportUserScript.py`
- 找到第57行左右：
```python
client = TelegramClient(s_dir, 2040, "b18441a1ff607e10a989891a5462e627")
```
- 将2040和"b18441a1ff607e10a989891a5462e627"替换为你的api_id和api_hash
- 获取API方法：
  1. 访问：https://my.telegram.org/auth
  2. 登录后点 "API development tools"
  3. 随便填写表单获取api_id和api_hash （如果获取不到，可以联系飞机 @Rfanhui 购买）

## 🎮 使用教程

### 1. 运行程序 ▶️
- Win+R 输入 `cmd` 回车
- 输入下面代码回车：
```bash
cd /d D:\telegram_report
python TelegramReportUserScript.py
```

### 2. 按提示操作 ⌨️
1. 输入要举报的用户名或ID
   - 格式：@username 或数字ID
   - 例如：@test 或 123456789

2. 输入举报次数
   - 输入具体数字：将使用多个账号轮流举报到指定次数
   - 输入0：每个可用账号举报一次

3. 选择举报类型（输入对应数字）：
   1. 👶 虐待儿童
   2. ©️ 版权问题
   3. ❌ 虚假消息
   4. 💊 非法药物
   5. ❓ 其他问题
   6. 👤 非法人员
   7. 🏢 非法组织
   8. 📨 垃圾邮件
   9. 💢 暴力行为

4. 输入举报内容
   - 可以直接输入文字描述
   - 建议详细说明举报原因

### 3. 查看结果 📊
- 程序会显示每个账号的举报状态
- 显示当前举报次数和剩余次数
- 显示举报成功或失败信息

## ❗ 常见问题

1. python不是内部命令
   - 重装Python，记得勾选"Add Python to PATH"

2. 无法连接
   - 需要科学上网

3. 举报失败
   - 检查账号是否正常
   - 确认目标用户名是否正确
   - 尝试更换API

## 📝 更新日志

### v1.0.0 (2024-03-21)
#### ✨ 新增
- 支持多账号批量举报功能
- 支持9种举报类型
- 自动检测账号有效性
- 支持自定义举报次数
- 支持自定义举报内容

#### 🔧 优化
- 自动清理无效会话文件
- 实时显示举报进度
- 支持重复举报功能

#### 📌 说明
1. 协议号相关
   - 支持批量导入协议号
   - 自动检测协议号有效性
   - 无效协议号自动清理

## ⚠️ 免责声明
本工具仅供学习交流使用，请勿用于非法用途。使用本工具所产生的一切后果由使用者自行承担。 
