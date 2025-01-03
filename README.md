# 能源监控系统 (Energy Monitoring System)

## 项目介绍
这是一个基于Vue3的能源监控系统前端项目，主要用于监控和展示工业设备的各项能源指标，包括电压、电流、温度和特征气体浓度等数据。系统提供实时监控、历史数据查询和告警管理等功能。

### 主要功能
1. **总览页面**
   - 设备状态统计
   - 实时监控数据展示
   - 关键指标趋势图
   - 气体浓度监测

2. **实时监控**
   - 电压、电流、温度实时仪表盘
   - 特征气体浓度实时趋势图
   - 数据实时更新（5秒间隔）

3. **历史数据**
   - 实时范围国数据查询
   - 多指标数据联动对比
   - 图表数据导出功能
   - 数据导出和打印

4. **告警管理**
   - 告警统计分析
   - 告警类型分布
   - 告警处理和确认

## 技术栈
- **前端框架**: Vue 3
- **构建工具**: Vite
- **UI组件库**: Element Plus
- **图表库**: ECharts 5
- **状态管理**: Vue Composition API
- **HTTP客户端**: Axios
- **开发语言**: JavaScript/TypeScript

## 安装和运行
### 环境要求
- Node.js >= 16.0.0
- npm >= 7.0.0

### 安装步骤
1. 克隆项目
```bash
git clone [项目地址]
cd EnergyMonitor
```

2. 安装依赖
```bash
npm install
```

3. 运行开发服务器
```bash
npm run dev
```

4. 构建生产版本
```bash
npm run build
```

## 项目结构
```
EnergyMonitor/
├── frontend/ # 前端项目目录
│   ├── src/ # 源代码
│   │   ├── views/ # 页面组件
│   │   ├── components/ # 通用组件
│   │   ├── router/ # 路由配置
│   │   ├── store/ # 状态管理
│   │   └── assets/ # 静态资源
│   ├── public/ # 公共资源
│   ├── package.json # 项目配置
│   └── README.md # 项目说明
```

## 使用说明
1. **总览页面** - 访问 `/dashboard` 查看系统总览
2. **实时监控** - 访问 `/realtime` 查看实时监控数据
3. **历史数据** - 访问 `/history` 查看历史数据
4. **告警管理** - 访问 `/alerts` 查看告警信息

## 开发说明
### 模拟数据
目前系统使用模拟数据进行展示，数据生成逻辑位于各个组件中：
- 实时数据：`generateMockData()`
- 历史数据：`generateMockHistoricalData()`
- 告警数据：`generateMockAlerts()`

### 配置文件
1. **图表配置**
   - 修改 `initGaugeChart()` 自定义仪表盘样式
   - 修改 `initGasChart()` 自定义气体监测图表

2. **告警配置**
   - 自定义告警类型和规则
   - 自定义告警阈值和优先级

## 注意事项
1. 确保Node.js和npm版本符合要求
2. 开发时注意观察浏览器兼容性
3. 生产环境部署前请修改相关配置
4. 建议使用Chrome或Firefox浏览器访问

## 后续开发计划
1. 添加用户认证和权限管理
2. 优化数据加载性能
3. 添加更多数据分析功能
4. 支持自定义仪表盘
5. 添加设备管理功能

## 贡献指南
1. Fork 项目
2. 创建功能分支
3. 提交更改
4. 推送到分支
5. 创建 Pull Request

## 许可证
[MIT License](LICENSE)

# EnergyMonitor