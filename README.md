# 飞机大战游戏

这是一个基于Java的2D飞机射击游戏，支持单人模式和多人在线模式。玩家可以控制飞机移动、射击敌人，并收集奖励物品以获得更高分数。

## 功能特性

- 单人游戏模式
- 多人在线对战模式
- 精美的游戏界面和音效
- 实时碰撞检测
- 分数管理系统
- 游戏存档功能

## 技术栈

- Java 8+
- Java Swing
- Java Socket编程
- MySQL数据库
- Maven构建工具

## 目录结构

```
src/
├── main/
│   ├── java/
│   │   └── com/ex/airplane/ - Java源代码
│   │       ├── GameObject/ - 游戏对象基类和实现
│   │       ├── UI/ - 用户界面组件
│   │       ├── multiplayer/ - 多人游戏相关类
│   │       ├── Server/ - 游戏服务器实现
│   │       ├── AudioPlayer.java - 音频播放器
│   │       ├── CollisionHandler.java - 碰撞检测处理器
│   │       ├── Main.java - 游戏启动类
│   │       └── ScoreManager.java - 分数管理器
│   │
│   └── resources/ - 资源文件
│       ├── BGM.wav - 背景音乐
│       ├── bullet.png - 子弹图片
│       ├── enemy.png - 敌机图片
│       ├── explosion.wav - 爆炸音效
│       ├── player.png - 玩家飞机图片
│       └── reward.png - 奖励物品图片
```

## 安装与运行

### 单人模式

1. 确保已安装Java 8+和Maven
2. 克隆项目到本地
3. 构建项目:
   ```
   mvn clean package
   ```
4. 运行游戏:
   ```
   java -jar target/example-proj-1.0.0.jar
   ```

### 多人模式

1. 确保已安装Java 8+、Maven和MySQL
2. 在MySQL中创建数据库并导入game.db
3. 修改Server.java中的数据库连接信息
4. 构建项目:
   ```
   mvn clean package
   ```
5. 启动游戏服务器:
   ```
   java -cp target/example-proj-1.0.0.jar com.ex.airplane.Server
   ```
6. 启动客户端:
   ```
   java -jar target/example-proj-1.0.0.jar
   ```

## 使用说明

- 使用方向键控制飞机移动
- 按空格键发射子弹
- 击败敌人获得分数
- 收集奖励物品获得更多分数
- 在多人模式中，可以与其他玩家一起游戏

## 贡献指南

欢迎贡献代码！请遵循以下步骤:

1. Fork项目
2. 创建新分支
3. 提交代码更改
4. 创建Pull Request

## 许可证

本项目采用MIT许可证。详情请查看项目根目录下的LICENSE文件。
