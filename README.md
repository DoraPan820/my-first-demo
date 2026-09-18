# 工业车辆（叉车/AGV）物联网产品经理技能
## 简介
本技能面向工业车辆领域产品经理，覆盖电动叉车、内燃叉车、AGV自动导引车的车载物联网终端与配套云平台产品，提供需求分析、功能规划、软硬件方案设计、产品文档输出能力。对标行业品牌：永恒力、林德、丰田等工业车辆。核心业务域包含**资产管理、物联卡管理、设备管理、用户管理、通知推送**，支持从需求调研到PRD交付、项目评审的完整产品工作流程。
> 知识库原始模板来源于消费IoT，所有方法论、文档模板可迁移适配叉车、AGV车载终端与车辆物联网平台场景。

## 核心能力
- **需求分析**：用户需求挖掘、车辆作业场景分析、竞品调研（林德/永恒力/丰田车辆物联网方案对标）
- **功能规划**：车载终端功能定义、云平台模块设计、权限设计、告警与消息推送策略
- **技术方案**：车载通信选型（4G/5G、Cat.1、蓝牙、CAN总线）、车载硬件选型、云端架构设计
- **文档输出**：16章结构PRD撰写、用户故事、硬件规格说明书、平台接口文档

## 文件结构

```
vehicle-iot-pm/
├── SKILL.md                      # 技能主文档（入口）
├── README.md                     # 本文件
├── smart-door-lock-prd.md        # PRD 完整范例（参考模板结构，可改写为 AGV 车载终端 PRD）
├── commands/                     # 工作流文档
│   ├── README.md                 # 工作流使用说明
│   ├── write-prd.md              # PRD 开发工作流（需求发现→方案设计→工程评估→评审）
│   └── discover.md               # 产品发现与验证工作流
├── assets/                       # 静态资源
│   └── device-icons/             # 设备图标目录与规范
│       └── icon-catalog.md       # 图标命名、分类与设计规范
└── references/                   # 参考文档
├── prd-template.md           # PRD 文档模板规范（16 章，含引导问题）
├── smart-home-scenes.md      # 场景联动范例（逻辑可迁移叉车 / AGV 告警联动）
├── tech-stack-guide.md       # 技术栈选型指南（车载通信、CAN、Cat.1、MQTT 等）
├── device-categories.md      # 设备品类文档（可扩展叉车、AGV、车载终端分类）
├── vendor-directory.md       # 厂商名录（工业车辆、车载模组、物联卡供应商）
├── certification-guide.md    # 产品认证指南（车载硬件、EMC、车辆相关标准）
├── product-checklist.md      # PRD 自检、技术评审、上线核对、迭代复盘清单
├── hardware-spec-template.md # 车载硬件需求规格模板
├── communication-protocol-guide.md  # 通信协议设计指南（MQTT、CAN 总线、物联卡上报）
├── firmware-architecture-template.md # 车载固件架构模板、远程 OTA 方案
├── discovery-validation-guide.md  # 产品发现与验证指南
├── prioritization-framework.md    # 需求优先级决策框架（RICE/Kano/MoSCoW）
└── jtbd-and-journey-map.md        # JTBD 与用户旅程地图
```

## 参考文档说明
| 文档 | 内容 | 使用场景 |
|------|------|----------|
| prd-template.md | PRD标准16章模板、用户故事、可量化验收标准 | 撰写叉车/AGV车载终端、车辆物联网平台PRD |
| smart-home-scenes.md | 场景联动逻辑范例，支持条件触发、多阶段联动 | 设计车辆告警、作业事件联动、消息推送场景 |
| tech-stack-guide.md | 通信模组、车载总线、网络方案对比选型 | AGV/叉车车载终端通信方案、物联卡网络选型 |
| device-categories.md | 设备分类框架，可扩展叉车、AGV、车载终端 | 产品规划、设备台账、资产管理模块设计 |
| vendor-directory.md | 工业车辆、车载模组、物联卡服务商名录 | 竞品对标、供应链调研（永恒力、林德、丰田等） |
| certification-guide.md | 国内外硬件、车载EMC、电气安全认证标准 | 车载终端合规评估、量产准入 |
| product-checklist.md | PRD自检、技术评审、上线、迭代复盘检查项 | PRD评审、方案评审、上线前自查 |
| hardware-spec-template.md | 主控、外设、电源、BOM硬件规格模板 | AGV/叉车车载通信终端硬件规格输出 |
| communication-protocol-guide.md | 物模型、MQTT Topic、CAN总线、消息安全设计 | 车辆数据上报、平台指令下发、物联卡通信 |
| firmware-architecture-template.md | RTOS任务划分、状态机、本地缓存、车载OTA | 车载终端固件设计、远程升级策略 |
| discovery-validation-guide.md | 问题定义、假设验证、用户访谈、POC验证 | 新项目立项、车辆物联网产品需求调研 |
| prioritization-framework.md | RICE/Kano/MoSCoW优先级评估框架 | 平台功能排期：资产管理、物联卡、设备、用户、推送 |
| jtbd-and-journey-map.md | JTBD理论、用户触点、用户旅程 | 仓库运维、车队管理员、叉车司机用户分析 |
| icon-catalog.md | 图标命名规范 | 后台管理系统UI图标设计（设备状态、告警、资产台账） |


---

## 使用方式
### 技能触发词
在豆包对话中输入以下类型的提问，将自动调用本知识库模板与方法论：
| 场景 | 触发词示例 |
|------|-----------|
| **产品规划** | "规划一套叉车&AGV车辆物联网平台"、"对标林德/永恒力，做工业车辆物联网产品立项"、"车队资产管理模块产品规划" |
| **PRD撰写** | "基于16章模板，写AGV车载终端PRD"、"输出叉车物联网云平台PRD文档"、"写物联卡管理模块PRD" |
| **功能设计** | "设计叉车设备告警推送功能"、"资产管理模块字段设计"、"平台用户权限与角色管理设计" |
| **技术选型** | "叉车车载终端通信方案选型Cat.1/4G"、"车载CAN总线对接方案"、"工业车辆物联卡方案对比" |
| **竞品分析** | "永恒力/林德/丰田车辆物联网方案对标分析"、"工业车辆车载终端竞品调研" |
| **认证合规** | "叉车车载硬件EMC认证清单"、"车载终端电气安全评估" |
| **硬件规格** | "AGV车载通信终端硬件规格设计"、"车载终端宽温电源方案、BOM评估" |
| **产品发现** | "用JTBD分析仓库车队管理员需求"、"叉车物联网产品需求验证与POC方案" |

### 工作流使用说明
| 工作流 | 说明 | 示例 |
|------|------|------|
| 完整PRD开发流程 | 完整PRD开发流程（需求发现→方案设计→工程评估→文档输出） | 使用16章PRD模板，撰写叉车物联网云平台PRD，包含资产管理、物联卡、设备、用户、推送模块 |
| 产品发现与验证流程 | 产品需求调研、假设验证、JTBD用户分析、用户旅程梳理 | 面向仓库车队管理员，做AGV&叉车物联网产品立项与需求验证 |

> 备注：知识库原始模板来自消费IoT，方法论、文档框架可迁移至叉车、AGV车载终端与车辆物联网平台场景。

### 使用建议
- **PM日常**：直接用自然语言描述需求，自动匹配参考文档
- **深度PRD**：先完成产品发现与需求验证，再按照16章模板撰写完整PRD文档
- **技术评审**：依次使用硬件规格→通信协议→固件架构三套模板开展评审

## 当前范围与限制
- 当前知识库以产品模板、方法论为主，不包含可直接部署的前端/后端源代码
- 模组、物联卡、工业车辆厂商信息具有时效性，正式项目立项前需要二次核实
- 知识库不包含自动化测试脚本，评审时需要人工核对需求、边界场景

## 工作流程
1. **需求收集**：明确目标车辆类型（叉车/AGV）、目标用户（车队管理员、仓库运维、司机）、核心模块（资产管理、物联卡管理、设备管理、用户管理、通知推送）
2. **资料参考**：调用知识库文档，复用产品模板、技术方案、评审清单
3. **方案设计**：功能规划、车辆场景设计、通信方案、权限、告警推送策略
4. **文档输出**：生成PRD、用户故事、硬件规格、接口说明、评审Checklist

---
## 🚀 快速查询表
| 任务 | 推荐顺序 | 优先级 | 时间 |
|------|---------|--------|------|
| **新员工入门** | README.md → SKILL.md → [device-categories.md](references/device-categories.md) | ⭐⭐⭐ | 30分钟 |
| **撰写PRD** | [prd-template.md](references/prd-template.md) → [smart-door-lock-prd.md](smart-door-lock-prd.md) | ⭐⭐⭐⭐ | 20分钟 |
| **产品规划** | [device-categories.md](references/device-categories.md) → [vendor-directory.md](references/vendor-directory.md) | ⭐⭐⭐ | 40分钟 |
| **功能设计** | [smart-home-scenes.md](references/smart-home-scenes.md)（联动逻辑范例，迁移车辆告警推送） + [device-categories.md](references/device-categories.md) | ⭐⭐⭐⭐ | 45分钟 |
| **技术方案** | [tech-stack-guide.md](references/tech-stack-guide.md) → [hardware-spec-template.md](references/hardware-spec-template.md) | ⭐⭐⭐⭐⭐ | 60分钟 |
| **硬件规格** | [hardware-spec-template.md](references/hardware-spec-template.md) → [tech-stack-guide.md](references/tech-stack-guide.md) | ⭐⭐⭐⭐⭐ | 45分钟 |
| **协议设计** | [communication-protocol-guide.md](references/communication-protocol-guide.md) → [tech-stack-guide.md](references/tech-stack-guide.md) | ⭐⭐⭐⭐ | 40分钟 |
| **固件架构** | [firmware-architecture-template.md](references/firmware-architecture-template.md) → [hardware-spec-template.md](references/hardware-spec-template.md) | ⭐⭐⭐⭐ | 40分钟 |
| **竞品分析** | [vendor-directory.md](references/vendor-directory.md) + [smart-door-lock-prd.md](smart-door-lock-prd.md) | ⭐⭐⭐ | 50分钟 |
| **产品发现** | [discovery-validation-guide.md](references/discovery-validation-guide.md) → [jtbd-and-journey-map.md](references/jtbd-and-journey-map.md) | ⭐⭐⭐⭐⭐ | 45分钟 |
| **优先级决策** | [prioritization-framework.md](references/prioritization-framework.md) → [prd-template.md](references/prd-template.md) | ⭐⭐⭐⭐ | 30分钟 |
| **认证合规** | [certification-guide.md](references/certification-guide.md) → [tech-stack-guide.md](references/tech-stack-guide.md) | ⭐⭐⭐⭐ | 30分钟 |
| **项目评审** | [product-checklist.md](references/product-checklist.md) + [prd-template.md](references/prd-template.md) | ⭐⭐⭐ | 15分钟 |
| **原型/UI** | [icon-catalog.md](assets/device-icons/icon-catalog.md) | ⭐⭐ | 20分钟 |

---
## 技能亮点
### 场景联动设计（范例逻辑可迁移叉车/AGV车辆告警）
- 支持多条件事件联动、多阶段延时触发
- 设备状态、传感器信号、时间组合触发（AND/OR条件）
> 叉车/AGV场景使用：复用这套联动逻辑，用于车辆故障告警、超速、电池低电量、维保到期推送通知。

### 技术选型全面
- 车载通信方案：Cat.1、4G/5G、蓝牙、CAN总线、MQTT协议对比
- 车载主控芯片选型（宽温、抗震动工业级）
- 云端物模型、安全加密方案、物联卡网络管理
- 安全设计要点、选型决策树

### 研发工程支持
- 车载硬件规格模板：主控、外设、宽温电源、抗震动BOM设计
- 通信协议模板：物模型、MQTT Topic、车辆数据上报、平台指令下发
- 固件架构模板：RTOS任务拆分、状态机、本地缓存、车载OTA升级策略

### 厂商与供应链资源
- 工业车辆品牌：永恒力、林德、丰田等叉车/AGV厂商对标
- 车载通信模组、物联卡服务商、硬件供应商名录
- 硬件双供应商方案，规避供应链风险

### 原型图标资源
- 车辆资产、设备状态、告警图标规范
- 支持车队管理后台、资产管理系统UI设计

## 依赖
无外部依赖

## 常见问题
### Q：如何快速掌握这套工业车辆物联网产品体系？
> 知识库原始模板来源于消费IoT，方法论可迁移叉车、AGV车载终端与车队物联网平台。
按以下顺序阅读：
1. 本文档（README.md）- 了解项目概况
2. [device-categories.md](references/device-categories.md) - 学习设备分类框架（叉车、AGV、车载终端）
3. [smart-home-scenes.md](references/smart-home-scenes.md) - 学习事件联动设计思路，用于车辆告警、通知推送场景

### Q：需要撰写叉车/AGV物联网平台PRD从哪里开始？
1. 先阅读 [prd-template.md](references/prd-template.md)，熟悉16章标准PRD结构
2. 参考 [smart-door-lock-prd.md](smart-door-lock-prd.md)，学习完整PRD范例结构
3. 在模板基础上，填入资产管理、物联卡管理、设备管理、用户管理、通知推送等业务模块

### Q：叉车车载终端通信方案如何选型？
1. 先评估车辆使用环境：仓库室内、室外、震动、温湿度
   - 固定站点AGV：优先CAN总线+本地局域网
   - 移动叉车：Cat.1/4G物联卡，MQTT上报车辆数据
2. 参考 [tech-stack-guide.md](references/tech-stack-guide.md)，对比通信方案功耗、成本、稳定性
3. 参考厂商名录，评估模组、物联卡供应商交付能力

### Q：工业车辆物联网竞品怎么对标？
1. 查阅 [vendor-directory.md](references/vendor-directory.md)，梳理永恒力、林德、丰田的车辆联网平台能力
2. 对比竞品：资产台账、车辆远程监控、告警推送、维保管理、用户权限功能
3. 参考PRD范例的竞品分析章节，输出对标文档

### Q：如何设计车辆告警、通知推送场景？
1. 打开 [smart-home-scenes.md](references/smart-home-scenes.md)，复用条件联动逻辑
2. 定义触发条件：电池低电量、故障码上报、超速、维保到期
3. 配置推送渠道：平台站内消息、短信、邮件，推送对象：车队管理员、仓库运维

## 更新日志
### v1.3 (2026-05-12)
- 新增PM方法论：产品发现验证、RICE/Kano/MoSCoW优先级框架、JTBD用户旅程
- 场景联动能力升级，支持多条件事件触发，可迁移车辆告警推送场景
- 车载芯片选型库扩充，新增工业宽温、抗震动车载MCU方案
- PRD模板扩充至16章：硬件规格、通信协议、固件OTA、测试方案、量产、合规章节
- 新增产品开发工作流：完整PRD开发流程（5阶段12步）和产品发现验证流程（4阶段8步）
- 参考文档增加：前置校验、风险识别、常见坑（Purpose → Key Concepts → Common Pitfalls）
- 厂商名录扩充工业车辆品牌（永恒力、林德、丰田）、车载模组、物联卡服务商
- 认证指南扩充车载硬件EMC、车辆电气安全相关标准

### v1.2
- 新增MQTT、CAN总线协议方案，扩充Cat.1/4G车载通信选型
- PRD范例增加设备运维、远程监控、故障诊断章节
- vendor-directory.md增加工业车辆物联网服务商信息
- 新增产品评审Checklist，完善硬件、固件、平台功能评审项

### v1.1
- 优化文档目录结构，增加快速查询表
- 补充用户故事、需求优先级落地案例

### v1.0
- 初始版本：16章PRD模板、硬件规格、通信方案、产品评审清单、用户分析框架

## 贡献
欢迎持续迭代完善模板，补充叉车/AGV行业案例、业务模块（资产管理、物联卡管理等）。
**维护者**：产品经理
**许可证**：MIT
