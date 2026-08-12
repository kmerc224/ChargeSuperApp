# ChargeSuperApp - 超级岛充电监控

适配澎湃OS3焦点通知（超级岛）的电池充电监控应用。

## 功能特性

- **超级岛适配**：在通知栏显示实时充电信息的超级岛
  - 收起态：左侧显示功率(W)，右侧显示温度(°C)（可自定义）
  - 展开态：显示电流(mA)、功率(W)、预计充电时间等（顺序可自定义）
  - 底部进度条：实时电池电量
- **电池信息面板**：实时电池状态 + 电池健康信息
- **充电记录图表**：电量/功率/温度折线图（MPAndroidChart）
- **高级权限支持**：可选 Shizuku / Root 获取更精确的电池数据
- **Material Design 3**：现代化 UI 设计

## 技术栈

- Java
- AndroidX
- Material Design 3 (Material Components)
- MPAndroidChart
- Shizuku API
- SQLite
- 最低适配：Android 15 (API 35)
- 编译版本：Android 16 (API 36)

## 项目结构

```
app/src/main/java/com/chargesuper/app/
├── MainActivity.java              # 主界面
├── BatteryMonitorService.java     # 电池监控前台服务
├── IslandNotificationHelper.java  # 超级岛通知构建
├── SetupWizardActivity.java       # 首次使用向导
├── PermissionHelper.java          # 权限管理
├── PermissionCenterActivity.java  # 权限中心
├── AboutActivity.java             # 关于页面
├── LogViewerActivity.java         # 运行日志
├── BootReceiver.java              # 开机自启
├── ShizukuShellService.java       # Shizuku 服务
├── data/                          # 数据层
├── log/                           # 日志捕获
├── settings/                      # 设置相关
└── ui/                            # UI Fragment
```

## 构建

1. 使用 Android Studio 打开项目
2. Sync Gradle
3. 连接 Android 15+ 设备或模拟器
4. Run

## License

Apache License 2.0
