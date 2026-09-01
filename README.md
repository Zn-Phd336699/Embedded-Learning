# 嵌入式软件开发全栈知识库

> **从编程基础到 SoC / RTOS / Android / 协议全栈实战**
>
> 一条覆盖「编程基础 → 调试工具 → 单片机 → SoC → RTOS → 嵌入式 Linux → Android 底层 → 通信协议」的完整成长路线，以**可复现的命令、可运行的代码、可落地的排故表**支撑实战，并以 6 个综合项目 + 主流开源项目源码解析收束。

本项目是一个**单文件、纯前端、零依赖、可离线使用**的嵌入式学习知识库，共约 1.35MB / 18700+ 行，包含 **13 篇正篇 + 5 大附录、140+ 章节**，覆盖从 C 语言指针到 ZYNQ 异构 SoC 的完整技术栈。

---

## ✨ 功能特性

- **单文件离线可用**：整个知识库封装在 `index.html` 中，双击即可在浏览器打开，无任何外部依赖
- **全库搜索**：内置客户端全文索引，输入关键词即可跨章节检索（180ms 防抖）
- **学习进度追踪**：左侧目录每章前的圆圈可勾选已完成，进度自动保存在浏览器 `localStorage`，刷新不丢失
- **深色/浅色主题**：一键切换，护眼阅读
- **滚动高亮**：Scrollspy 自动高亮当前章节，随阅读进度定位
- **代码一键复制**：所有代码块带「复制」按钮
- **响应式布局**：移动端自动折叠为汉堡菜单
- **结构化的章节设计**：每章包含「学习目标 → 正文命令/代码 → 常见故障排故表 → FAQ 避坑 → 思考题」

---

## 📚 内容大纲

| 篇章 | 主题 | 章节 | 内容亮点 |
|------|------|------|----------|
| 第一篇 | 编程基础与提升 | 第 1~9A 章 | C 指针与内存模型、C++ 嵌入式子集与 RAII、ARM 汇编反汇编排障（HardFault/Oops）、链接器与 ld 脚本、环形缓冲/对象池/状态机、模块化架构、MISRA C + Unity 单测、AI 辅助开发边界 |
| 第二篇 | 开发调试工具链 | 第 10~20 章 | GCC 交叉编译、Makefile/CMake/Kconfig、GDB 深度实战、OpenOCD/J-Link/ST-Link/probe-rs、RTT 日志、Canary/ASan 内存排查、perf/ftrace 火焰图、Wireshark、示波器、逻辑分析仪、频谱仪 |
| 第三篇 | 单片机开发（Cortex-M 与 ESP32） | 第 21~33 章 | Cortex-M 架构/NVIC/MPU、STM32F407 外设全家桶（GPIO/RCC/定时器/DMA/ADC/串口/低功耗）、Bootloader/IAP/OTA、ESP-IDF 与 WiFi/BLE、环境监测终端实战 |
| 第四篇 | SoC 开发 | 第 34~44C 章 | i.MX6ULL / RK3568·3588 / 全志 H3 平台、启动链 BootROM→SPL→ATF→U-Boot→Kernel、设备树、Buildroot/Yocto、NPU/GPU 应用、边缘网关/AI 视觉工作站实战 |
| 第五篇 | RTOS | 第 45~53 章 | RMS/EDF 调度理论、FreeRTOS 源码三级精读（任务/上下文切换/IPC/内存/tickless）、FreeRTOS-SMP、RT-Thread 与 Zephyr 对比、Tracealyzer/SystemView、seL4 微内核、云台控制器实战 |
| 第六篇 | 嵌入式 Linux | 第 54~66 章 | 发行版抉择与 QEMU 学习路线、启动流程、rootfs 构建、字符/Platform/子系统驱动、中断下半部、epoll 与网络编程、Oops 调试/kgdb/kdump、性能优化、USB 摄像头实战 |
| 第七篇 | Android 底层开发 | 第 67~73 章 | AOSP 编译、init→Zygote→SystemServer、HAL/AIDL、Binder 原理、DTB/sepolicy/vendor blobs、A/B OTA、Perfetto/logcat/adb |
| 第八篇 | 嵌入式协议开发 | 第 74~86 章 | UART/Modbus RTU、I2C、SPI/QSPI、CAN/CAN FD、USB、以太网与 lwIP、MQTT/CoAP、WiFi、BLE、LoRa/LoRaWAN + ChirpStack、NB-IoT/Cat.1、PCIe、无线共存排障 |
| 第九篇 | 综合实战项目集 | 第 87~92 章 | **6 个开源项目对照解析**：STM32 环境监测终端、ESP32-S3 桌面信息站、MCUboot 双分区 OTA、LoRa 网关 + ChirpStack、RK3568 边缘 AI 盒子、OpenWrt 定制路由器 |
| 第十篇 | 安全、测试与量产工程 | S1~S4 | Secure Boot 实战、密钥管理与安全元件 ATECC608、HIL 测试台架 + Renode 仿真、产测工装/烧录/可靠性老化 |
| 第十一篇 | 工程常用算法 | A0~A11 | 数字滤波七件套、卡尔曼族谱（KF/EKF/UKF）、姿态解算、PID 全集（抗饱和/自整定）、LQR/串级/前馈、SVPWM 与无感 FOC、S 曲线轨迹、CRC 族谱、FFT/Goertzel、轻量加密、机器人导航概览 |
| 第十二篇 | 系统性能工程 | SO1~SO5 + SE | USE 法/火焰图方法论、MCU 系统优化、RTOS 多任务调优、三大优化战役复盘、Linux 内核调参与容器治理、专家技能地图 |
| 第十三篇 | ZYNQ 异构 SoC 开发 | Z1~Z5 | ZYNQ7020 架构全景、Verilog 精要与 Vivado 七步流程、PS 裸机与 PS-PL 协同、数据采集系统实战 |
| 附录 | 题库与速查 | A~E | 面试题库（五专项）、工具命令速查卡、芯片/模块/仪器选型对照表、术语表、Obsidian × LLM 知识管理工作流 |

---

## 🚀 使用方法

1. 将仓库克隆到本地：

   ```bash
   git clone https://github.com/Zn-Phd336699/Embedded-Learning.git
   ```

2. 直接用浏览器打开 `index.html`（推荐 Chrome / Edge）：

   ```bash
   start index.html        # Windows
   open index.html         # macOS
   ```

   或在本地起一个静态服务：

   ```bash
   # 任意静态服务器，例如 Python
   python -m http.server 8080
   # 然后浏览器访问 http://localhost:8080
   ```

3. 按左侧目录顺序学习，勾选章节圆圈记录进度。

---

## 🧠 正确的学习姿势

> ① 每章先看「学习目标」，跟做正文命令与代码；
> ② 每章末尾的「常见故障排故表」「FAQ 避坑」「思考题」是精华，务必过一遍；
> ③ 左侧目录章节前的圆圈可标记已完成，进度自动保存在浏览器；
> ④ 出问题时先翻本章排故表自查 30 分钟，再求助搜索引擎/AI —— 把报错原文作为关键词。

**三条铁律**：

1. **工具链版本一致**：同一项目内 GCC、CubeMX 生成代码、SDK 版本不要混用；
2. **先测供电再上电**：新焊接/新接线先用万用表确认无短路，调试仪器地线共地；
3. **改动要留痕**：所有实验用 Git 管理，每次成功后 commit，出问题可 diff 回溯。

---

## 🧩 硬件锚点清单

所有引脚号、寄存器地址、命令示例均以下表硬件为基准书写，没有对应板卡时可用同主控的其他板卡平移（改引脚宏），部分实验提供 QEMU 模拟替代。

| 领域 | 主锚点硬件 | 平替建议 |
|------|-----------|----------|
| 单片机 ARM-M | 正点原子 探索者 STM32F407ZGT6 | 战舰 F103、野火挑战者、立创天空星 F407 |
| ESP32 | 正点原子 ESP32-S3 开发板 | ESP32-S3-DevKitC-1、安信可 ESP32-S3 |
| Linux 入门 SoC | 正点原子 I.MX6U-ALPHA（i.MX6ULL） | 野火 EBF6ULL、韦东山 JZ2440 |
| RK 平台 | 正点原子 ATK-DLRK3568 | Luckfox Pico、香橙派 RK3566/3588 系 |
| 全志 H3 | Orange Pi Zero / NanoPi NEO | Orange Pi PC、NanoPi Duo2 |
| 示波器 | 普源 DS1054Z 或 FNIRSI-1014D | 任意 ≥2 通道数字示波器 |
| 逻辑分析仪 | 24MHz 8 通道 Saleae 兼容 + PulseView | DSLogic Plus / U3Pro16 |
| 频谱仪 | TinySA Ultra + NanoVNA-F V2 | 频谱功能较强的手持综测仪 |

---

## 📁 目录结构

```
Embedded_Learn/
├── index.html    # 单文件知识库（全部内容，含 CSS / HTML / JS）
└── README.md     # 本说明文件
```

## 🛠️ 技术栈

- 纯原生 HTML / CSS / JavaScript，零依赖、零构建
- 内容以语义化 `<section class="chapter">` 组织，样式变量支持深/浅主题
- `localStorage` 持久化学习进度
- 原生 JS 实现全文检索、Scrollspy、代码复制、进度统计

---

## 📄 License

本项目内容仅供学习交流使用。文中引用的开源项目（FreeRTOS、lwIP、MCUboot、LoRaMac-node、OpenWrt 等）版权归其各自作者所有。
