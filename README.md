# 动车组机械师 - 15天背诵 Android App

> 将 1,517 道动车组机械师题库（Excel + Word）按车型分类，打包为手机 APK，方便随时随地背诵。

## 📱 功能

- **按车型分类**：CRH1/1A、CRH2/2A、CRH5/5A、CRH380A、CR400AF、通用题
- **15天计划**：每天定量学习，逐步覆盖全部题型
- **点击显示答案**：先思考再看答案，强化记忆
- **进度追踪**：标记已掌握题目，进度自动保存（localStorage）
- **离线使用**：全部数据嵌入 APK，无需联网

## 📥 下载 APK

前往 [Actions](https://github.com/whyjes/train-exam-app/actions) 页面，选择最新 Workflow，下载 **动车组机械师-APK** 构件。

Android 安装前需在设置中允许「安装未知来源应用」。

## 🏗️ 本地构建

```bash
git clone https://github.com/whyjes/train-exam-app.git
cd train-exam-app
./gradlew assembleDebug
```

APK 生成在 `app/build/outputs/apk/debug/` 目录下。

## 📊 题库来源

| 来源 | 题型 | 题数 |
|------|------|------|
| Excel题库 | 填空 + 单选 + 多选 + 判断 + 简答 + 论述 | 956 |
| Word题库 | 问答题 | 561 |
| **合计** | | **1,517** |

## 📅 15天学习计划

| 天数 | 内容 | 车型 |
|------|------|------|
| 1-2 | 转向架、车钩、车门、受电弓 | CRH1/1A |
| 3 | 转向架、风挡、高压系统 | CRH2/2A |
| 4-5 | 转向架探伤、轮对、制动、卫生间 | CRH5/5A |
| 6-8 | 填空+判断+单选+多选+问答 | CRH380A |
| 9-10 | 填空+判断+单选+多选+问答 | CR400AF |
| 11-13 | 各题型全覆盖 | 通用基础 |
| 14 | 易错题复习 | 混合 |
| 15 | 全真模拟 | 随机抽题 |

## ⚙️ 技术栈

- **WebView**: 加载离线 HTML（含所有题型 + 交互逻辑）
- **Gradle**: Android 构建系统
- **GitHub Actions**: 自动构建 APK
