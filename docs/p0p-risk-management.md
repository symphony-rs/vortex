# 风险控制 - 全面的交易风险管理系统，确保交易安全合规

- 易前风控 - 在订单提交前进行风险检查，防止有风险的交易执行和潜在损失
  - [❌] [合规检查](./risk/pre-trade/compliance.md) - 确保交易符合监管和内部政策的检查机制，防范合规风险和法律责任
    - [❌] [限制名单检查](./risk/pre-trade/compliance/restricted-list.md) - 检查交易证券是否在限制或禁止交易名单上，防止违规交易活动
    - [❌] [交易限额检查](./risk/pre-trade/compliance/trading-limits.md) - 验证交易是否符合交易规模和频率限制，避免过度交易和市场操纵行为
    - [❌] [反洗钱检查](./risk/pre-trade/compliance/aml.md) - 识别可能违反反洗钱规定的交易模式和行为，确保合规性和风险控制
    - [❌] [内幕交易筛查](./risk/pre-trade/compliance/insider-trading.md) - 检测可能涉及内幕交易的可疑交易活动，防范内幕交易风险
    - [❌] [跨市场合规检查](./risk/pre-trade/compliance/cross-market.md) - 确保跨不同市场的交易符合各自监管规则，应对多市场交易的合规挑战
  - [❌] [风险限额管理](./risk/pre-trade/limits.md) - 设置和监控各类风险限额的系统，防止过度风险暴露和控制损失幅度
    - [❌] [订单规模限制](./risk/pre-trade/limits/order-size.md) - 根据流动性和风险偏好限制单笔订单规模，避免市场冲击和执行风险
    - [❌] [持仓集中度限制](./risk/pre-trade/limits/concentration.md) - 控制对特定证券、行业或市场的敞口集中度，确保投资多元化
    - [❌] [波动性敞口限制](./risk/pre-trade/limits/volatility-exposure.md) - 限制对高波动性资产的敞口，降低市场剧烈波动时的潜在损失
    - [❌] [杠杆使用限制](./risk/pre-trade/limits/leverage.md) - 控制账户和策略的杠杆率，防止过度风险和放大亏损
    - [❌] [损失限制](./risk/pre-trade/limits/loss.md) - 设置账户和策略的最大可接受损失阈值，保护投资资本和控制风险水平
  - [❌] [订单验证](./risk/pre-trade/validation.md) - 验证订单参数和合法性的流程，防止错误交易或失误执行造成的损失
    - [❌] [价格合理性检查](./risk/pre-trade/validation/price.md) - 验证订单价格是否在合理范围内，防止误单导致的价格冲击和异常交易
    - [❌] [参数完整性检查](./risk/pre-trade/validation/parameters.md) - 确保订单包含所有必要参数且格式正确，避免交易执行错误
    - [❌] [重复订单检测](./risk/pre-trade/validation/duplicates.md) - 识别和防止可能的重复订单提交，避免非预期的头寸和执行风险
    - [❌] [拼写和符号检查](./risk/pre-trade/validation/symbols.md) - 验证证券代码和指令的准确性，防止因输入错误导致的错误交易
    - [❌] [算法参数验证](./risk/pre-trade/validation/algo-parameters.md) - 验证算法交易参数的合理性和一致性，确保算法正确执行
  - [❌] [信用风险控制](./risk/pre-trade/credit.md) - 管理交易对手信用风险的机制，防止因交易对手违约导致的损失和风险传导
    - [❌] [交易对手风险评估](./risk/pre-trade/credit/counterparty-assessment.md) - 评估交易对手的信用状况和违约风险，建立风险评级系统
    - [❌] [信用额度管理](./risk/pre-trade/credit/credit-limits.md) - 设置和监控交易对手的信用额度，控制单一交易对手风险暴露
    - [❌] [保证金要求管理](./risk/pre-trade/credit/margin-requirements.md) - 计算和监控交易所需的保证金要求，确保充足的资金支持
    - [❌] [抵押品管理](./risk/pre-trade/credit/collateral.md) - 管理用于支持交易的抵押品价值和质量，确保充分的风险缓冲
    - [❌] [信用风险调整估值](./risk/pre-trade/credit/credit-valuation.md) - 根据交易对手信用风险调整交易估值，反映潜在违约成本

- 交易中风控 - 实时监控和控制交易执行中的风险，确保交易执行符合预期和风控要求

  - 价格异常监控 - 实时监控和响应价格异常波动的系统，防止执行质量问题和异常成交
    - [突发价格变动检测](./core/risk/in-trade/price/sudden-moves.md) - 识别和响应市场中的突发价格变动
    - [错单价格检测](./core/risk/in-trade/price/fat-finger.md) - 识别可能由错误输入导致的异常价格
    - [价格偏离度监控](./core/risk/in-trade/price/deviation.md) - 测量和监控执行价格与参考价格的偏离程度
    - [价格操纵检测](./core/risk/in-trade/price/manipulation.md) - 识别可能的市场价格操纵行为
    - [做市价差监控](./core/risk/in-trade/price/market-making-spread.md) - 监控做市活动中的买卖价差变化

  - 实时敞口监控 - 动态跟踪和控制交易过程中的风险敞口，确保风险水平可控并防止敞口超限
    - [持仓变化跟踪](./core/risk/in-trade/exposure/position-tracking.md) - 实时监控持仓规模和结构的变化
    - [敞口限额监控](./core/risk/in-trade/exposure/limit-monitoring.md) - 确保各类风险敞口保持在预设限额内
    - [风险因子暴露](./core/risk/in-trade/exposure/factor-exposure.md) - 分析和监控对各种风险因子的敞口
    - [集中度变化监控](./core/risk/in-trade/exposure/concentration.md) - 追踪投资组合集中度的动态变化
    - [敏感性分析](./core/risk/in-trade/exposure/sensitivity.md) - 实时评估组合对市场因素变化的敏感性

  - 动态限额调整 - 根据市场条件和交易表现动态调整风险限额的机制，适应变化的市场环境和风险状况
    - [波动率感知限额](./core/risk/in-trade/dynamic-limits/volatility-aware.md) - 根据市场波动性自动调整风险限额
    - [流动性感知限额](./core/risk/in-trade/dynamic-limits/liquidity-aware.md) - 根据市场流动性状况调整交易限额
    - [绩效触发调整](./core/risk/in-trade/dynamic-limits/performance-triggered.md) - 基于交易绩效自动调整风险限额
    - [市场情绪适应](./core/risk/in-trade/dynamic-limits/sentiment-adaptive.md) - 根据市场情绪指标调整风险参数
    - [多层级限额系统](./core/risk/in-trade/dynamic-limits/multi-tier.md) - 实施基于不同触发条件的多层级限额结构

  - 执行质量监控 - 实时监控交易执行质量的系统，确保最佳执行并防止执行风险和成本超支
    - [滑点监控](./core/risk/in-trade/execution/slippage.md) - 测量和控制价格滑点，确保执行符合预期
    - [订单填充率监控](./core/risk/in-trade/execution/fill-rate.md) - 追踪订单填充情况，识别执行质量问题
    - [市场影响评估](./core/risk/in-trade/execution/market-impact.md) - 估计和控制交易对市场价格的影响
    - [执行速度监控](./core/risk/in-trade/execution/speed.md) - 监控订单执行速度，确保及时执行关键交易
    - [流动性寻源监控](./core/risk/in-trade/execution/liquidity-sourcing.md) - 评估和优化流动性寻源策略的有效性

- 风险度量 - 全面的风险度量指标和分析工具，支持风险评估和决策

  - VaR计算模型 - 计算和分析风险价值(Value at Risk)的工具，量化潜在损失风险和投资组合风险暴露
    - [历史模拟法](./core/risk/measurement/var/historical.md) - 使用历史数据模拟的VaR计算方法
    - [参数法](./core/risk/measurement/var/parametric.md) - 基于统计分布假设的VaR计算方法
    - [蒙特卡洛模拟](./core/risk/measurement/var/monte-carlo.md) - 使用随机模拟的VaR计算方法
    - [条件风险价值(CVaR)](./core/risk/measurement/var/conditional.md) - 计算超过VaR阈值的预期损失
    - [组件VaR](./core/risk/measurement/var/component.md) - 分解投资组合VaR至各个组成部分的贡献

  - 压力测试框架 - 评估极端市场条件下投资组合表现的工具，识别尾部风险和极端情境下的脆弱性
    - [历史情景分析](./core/risk/measurement/stress-test/historical.md) - 使用历史极端事件数据的压力测试
    - [假设情景分析](./core/risk/measurement/stress-test/hypothetical.md) - 基于假设极端情景的压力测试
    - [敏感性分析](./core/risk/measurement/stress-test/sensitivity.md) - 测试投资组合对特定风险因子变化的敏感性
    - [反向压力测试](./core/risk/measurement/stress-test/reverse.md) - 确定可能导致特定损失水平的市场情景
    - [流动性压力测试](./core/risk/measurement/stress-test/liquidity.md) - 评估市场流动性急剧下降时的组合表现

  - 风险归因分析 - 识别和量化不同风险来源的工具，深入理解风险结构和组成因素
    - [因子风险分解](./core/risk/measurement/attribution/factor.md) - 将组合风险分解到各个风险因子的贡献
    - [行业风险分析](./core/risk/measurement/attribution/sector.md) - 分析不同行业和板块的风险贡献
    - [地域风险分析](./core/risk/measurement/attribution/geographic.md) - 评估不同地域和市场的风险贡献
    - [策略风险分析](./core/risk/measurement/attribution/strategy.md) - 分析不同交易策略的风险贡献
    - [特异风险分析](./core/risk/measurement/attribution/idiosyncratic.md) - 评估非系统性或特异性风险的来源和影响

  - 相关性与波动率分析 - 分析资产间相关性和波动率特征的工具，优化风险分散和投资组合结构
    - [相关性矩阵](./core/risk/measurement/correlation/matrix.md) - 计算和可视化资产间相关性结构
    - [波动率表面](./core/risk/measurement/correlation/volatility-surface.md) - 构建和分析波动率随价格和时间的变化
    - [相关性稳定性分析](./core/risk/measurement/correlation/stability.md) - 评估相关性结构随时间的稳定性
    - [条件相关性分析](./core/risk/measurement/correlation/conditional.md) - 分析特定市场条件下的相关性变化
    - [隐含相关性提取](./core/risk/measurement/correlation/implied.md) - 从期权价格提取市场隐含的相关性预期

- 风险管理策略 - 系统性管理和应对不同类型风险的策略框架，提供全面风险解决方案

  - 资金风险管理 - 管理资金使用和流动性风险的策略，确保资金安全和可用性，优化资本配置
    - [资金使用预算](./core/risk/strategies/capital/budget.md) - 为不同策略和交易活动分配资金预算
    - [流动性储备管理](./core/risk/strategies/capital/liquidity-reserves.md) - 维持适当的流动性储备以应对突发需求
    - [现金流预测](./core/risk/strategies/capital/cash-flow.md) - 预测和管理交易活动产生的现金流
    - [资金效率优化](./core/risk/strategies/capital/efficiency.md) - 优化资金使用效率，最大化资本回报
    - [资金应急计划](./core/risk/strategies/capital/contingency.md) - 为资金紧急情况准备的预案和响应机制

  - 风险分类框架 - 系统性分类和管理不同类型风险的框架，提供结构化风险管理方法和全面防护
    - [市场风险管理](./core/risk/strategies/classification/market.md) - 管理价格、利率、汇率等市场风险的策略
    - [信用风险管理](./core/risk/strategies/classification/credit.md) - 管理交易对手和债务人信用风险的策略
    - [流动性风险管理](./core/risk/strategies/classification/liquidity.md) - 管理资产变现和资金流动风险的策略
    - [操作风险管理](./core/risk/strategies/classification/operational.md) - 管理系统故障、人为错误等操作风险的策略
    - [声誉风险管理](./core/risk/strategies/classification/reputational.md) - 管理可能影响商业声誉的风险因素

  - 对冲策略 - 使用金融工具对冲和中和风险的策略，减少不必要的风险暴露和保护投资价值
    - [直接对冲](./core/risk/strategies/hedging/direct.md) - 使用对应资产或衍生品直接对冲特定风险
    - [交叉对冲](./core/risk/strategies/hedging/cross.md) - 使用相关资产间接对冲风险，适用于缺乏直接对冲工具的情况
    - [动态对冲](./core/risk/strategies/hedging/dynamic.md) - 根据市场变化动态调整对冲头寸的策略
    - [宏观对冲](./core/risk/strategies/hedging/macro.md) - 对冲宏观经济风险因素的策略
    - [事件风险对冲](./core/risk/strategies/hedging/event.md) - 针对特定事件风险的对冲策略

  - 风险优化模型 - 数学优化方法平衡风险和回报的模型，实现风险调整后的最优决策和效率配置
    - [均值方差优化](./core/risk/strategies/optimization/mean-variance.md) - 基于收益率和波动率的经典投资组合优化
    - [风险平价模型](./core/risk/strategies/optimization/risk-parity.md) - 平衡各资产风险贡献的资产配置方法
    - [条件风险优化](./core/risk/strategies/optimization/conditional.md) - 考虑尾部风险和极端情况的优化方法
    - [多目标风险优化](./core/risk/strategies/optimization/multi-objective.md) - 同时考虑多个风险和回报目标的优化
    - [鲁棒性优化](./core/risk/strategies/optimization/robust.md) - 对参数估计不确定性具有抵抗力的优化方法

- 风险监控与报告 - 全面风险监控和报告系统，提供风险透明度和决策支持

  - 风险仪表盘 - 集中展示关键风险指标的界面，提供风险状况的直观视图和实时监测
    - [实时风险监控](./core/risk/monitoring/dashboard/real-time.md) - 显示当前实时风险指标和警报的仪表盘
    - [历史趋势对比](./core/risk/monitoring/dashboard/historical.md) - 展示风险指标历史变化和趋势的视图
    - [多维风险视图](./core/risk/monitoring/dashboard/multi-dimensional.md) - 从多个维度展示风险状况的综合视图
    - [阈值与警报显示](./core/risk/monitoring/dashboard/thresholds.md) - 显示风险阈值和当前警报状态的界面
    - [风险热图](./core/risk/monitoring/dashboard/heatmap.md) - 使用热图直观展示风险分布和集中度

  - 风险报告体系 - 生成各类风险报告的系统，满足内部管理和外部监管需求，支持透明决策
    - [定期风险报告](./core/risk/monitoring/reporting/periodic.md) - 按日、周、月等周期生成的标准风险报告
    - [特殊事件报告](./core/risk/monitoring/reporting/event-driven.md) - 针对特定风险事件生成的深度分析报告
    - [监管合规报告](./core/risk/monitoring/reporting/regulatory.md) - 满足监管要求的专业风险报告
    - [管理层摘要报告](./core/risk/monitoring/reporting/executive.md) - 为高管层提供的简明风险摘要和见解
    - [客户风险报告](./core/risk/monitoring/reporting/client.md) - 为客户提供的风险评估和投资组合分析报告

  - 预警机制 - 自动识别和通知风险预警信号的系统，支持主动风险管理和及时干预
    - [阈值预警](./core/risk/monitoring/alerts/threshold.md) - 基于预设阈值触发的风险预警机制
    - [趋势预警](./core/risk/monitoring/alerts/trend.md) - 基于风险指标变化趋势触发的预警
    - [相对预警](./core/risk/monitoring/alerts/relative.md) - 基于与基准或历史数据比较触发的预警
    - [复合条件预警](./core/risk/monitoring/alerts/compound.md) - 基于多个条件组合触发的高级预警
    - [预警升级机制](./core/risk/monitoring/alerts/escalation.md) - 根据风险严重程度自动升级通知级别的机制

  - 风险数据分析 - 深入分析风险数据的工具，提供高级风险洞察和决策支持，挖掘潜在风险模式
    - [风险趋势分析](./core/risk/monitoring/analytics/trends.md) - 分析风险指标随时间的变化趋势和模式
    - [异常检测](./core/risk/monitoring/analytics/anomalies.md) - 识别风险数据中的异常模式和事件
    - [风险集中度分析](./core/risk/monitoring/analytics/concentration.md) - 分析风险在不同维度的集中情况
    - [情景模拟](./core/risk/monitoring/analytics/scenarios.md) - 模拟不同市场情景下的风险变化和影响
    - [风险因子分析](./core/risk/monitoring/analytics/factors.md) - 识别和量化影响风险的主要因子和驱动力 
