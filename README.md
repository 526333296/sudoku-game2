# 小朋友数独游戏

## 游戏介绍
专为5岁儿童设计的趣味数独游戏，使用可爱的动物表情符号代替数字，让孩子在游戏中培养逻辑思维能力！

## 游戏特点
- 🎮 **4x4简化网格**：适合儿童的难度设计
- 🐶 **可爱的动物符号**：狗、猫、老鼠、兔子
- 📱 **触屏友好**：大按钮，容易点击
- 📺 **支持电视**：遥控器导航支持
- 🎯 **50关挑战**：难度逐步递增
- 💡 **提示功能**：帮助孩子学习

## 关卡设计
- 第1-10关：预设6个符号
- 第11-20关：预设5个符号
- 第21-30关：预设4个符号
- 第31-40关：预设3-4个符号
- 第41-50关：预设3个符号

## 如何编译APK

### 方法1：使用GitHub Actions（推荐）

1. 在GitHub创建新仓库（例如：`sudoku-game`）
2. 上传本项目所有文件
3. 等待GitHub Actions自动编译（约5-10分钟）
4. 进入Actions页面，下载编译好的APK

### 方法2：本地编译

**前提条件：**
- 安装Android Studio
- 安装Android SDK (API 34)
- 配置JAVA_HOME环境变量

**编译步骤：**
```bash
cd sudoku-game
gradle assembleDebug
```

APK文件位置：`app/build/outputs/apk/debug/app-debug.apk`

## 项目结构
```
sudoku-game/
├── app/
│   └── src/main/
│       ├── java/com/sudoku/
│       │   └── MainActivity.java
│       ├── res/
│       │   ├── layout/
│       │   ├── values/
│       │   └── mipmap-*/
│       ├── AndroidManifest.xml
│       └── assets/
│           └── index.html
├── build.gradle
├── settings.gradle
└── .github/workflows/
    └── build.yml
```

## 游戏操作说明
1. 点击空白格子选中
2. 点击下方动物符号填入
3. 点击"检查"按钮验证答案
4. 点击"提示"获取帮助
5. 完成一关后自动进入下一关

## 技术支持
- 使用Android WebView加载HTML5游戏
- 支持Android 5.0 (API 21)及以上版本
- 适配各种屏幕尺寸

## 授权
MIT License - 可自由使用和修改
