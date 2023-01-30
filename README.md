# DevOps

## 软件工程

```mermaid
  graph LR
  破坏者>"破坏者:自治权 生物计算 计算潜能 多文化巨大系统?"]
  subgraph "全局集成<br>2010年迄今"
    企业级架构("合法方法 基础设施 环境<br>企业级架构<br>由用户构建系统")
  end
  subgraph "敏捷:价值<br>21世纪初"
    集成系统与软件工程("集成系统与软件工程")
    混合式("混合式:融合敏捷与计划驱动方法")
    面向服务的体系结构("面向服务的体系结构 模型驱动的开发")
  end
  敏捷方法("敏捷方法")
  快速组合("快速组合 演化环境")
  subgraph "并发过程<br>20世纪90年代"
    并发的风险驱动过程("并发的风险驱动过程")
    特定领域的软件体系结构产品线复用("特定领域的软件体系结构产品线复用")
  end
  subgraph "生产率<br>20世纪80年代"
    面向对象方法("面向对象方法")
    标准的成熟度方法("标准的成熟度方法")
    软件工厂("软件工厂")
    用户编程("商业4GLs GAD/CAM 用户编程")
  end
  subgraph "生产率<br>20世纪80年代"
    面向对象方法("面向对象方法")
    标准的成熟度方法("标准的成熟度方法")
    软件工厂("软件工厂")
    用户编程("商业4GLs GAD/CAM 用户编程")
  end
  subgraph "形式:瀑布<br>20世纪70年代"
    结构化方法("结构化方法")
    瀑布过程("瀑布过程")
    形式化方法("形式化方法")
    领域理解("领域理解")
  end
  subgraph "工艺<br>20世纪60年代"
    软件工艺("软件工艺<br>code-and-fix<br>英雄主义的调试")
  end
  subgraph "硬件工程<br>20世纪50年代"
    硬件工程方法("硬件工程方法<br>SAGE<br>硬件效能")
    需求增长>"需求增长,差异性"]
    技能缺失>"技能缺失"]
  end

  硬件工程方法 -- "软件差异" --> 软件工艺
  需求增长 --> 软件工艺
  技能缺失 --> 软件工艺
  软件工艺 -- "意大利面条式代码" --> 结构化方法
  软件工艺 -- "项目越大,计划和控制越弱" --> 瀑布过程
  软件工艺 -- "许多缺陷" --> 形式化方法
  结构化方法 -- "可演化性<br>可复用性" --> 面向对象方法
  瀑布过程 -- "不兼容" --> 标准的成熟度方法
  瀑布过程 --> 软件工厂
  技能缺失 --> 用户编程
  领域理解 --> 用户编程
  瀑布过程 -- "HCI COTS 突发性" --> 并发的风险驱动过程
  形式化方法 -- "缺乏可伸缩性" --> 并发的风险驱动过程
  用户编程 -- "缺乏可伸缩性" --> 特定领域的软件体系结构产品线复用
  瀑布过程 -- "缓慢执行" --> 快速组合
  面向对象方法 -- "人为因素" --> 敏捷方法
  标准的成熟度方法 -- "过程管理的官僚机构" --> 敏捷方法
  软件工厂 -- "快速变化" --> 快速组合
  并发的风险驱动过程 -- "快速变化" --> 敏捷方法
  特定领域的软件体系结构产品线复用 -- "快速变化" --> 快速组合
  面向对象方法 -- "企业集成<br>人为因素" --> 集成系统与软件工程
  并发的风险驱动过程 -- "快速变化" --> 混合式
  特定领域的软件体系结构产品线复用 --> 面向服务的体系结构
  敏捷方法 -- "烟囱式系统" --> 集成系统与软件工程
  敏捷方法 -- "缺乏可伸缩性" --> 混合式
  快速组合 --> 混合式
  快速组合 --> 面向服务的体系结构
  集成系统与软件工程 -- "全局连通性<br>商业实用性<br>安全性风险<br>巨大的系统之系统" --> 企业级架构
  混合式 --> 企业级架构
  快速组合 -- "规模<br>Scale" --> 企业级架构
  面向服务的体系结构 -- "模型冲突" --> 企业级架构
  企业级架构 --> 破坏者
```

  + 软件工程发展趋势

<br>

## DevOps概述

$$\begin{gather*}
  \begin{drcases}
  \text{敏捷} \\
  \text{精益}
  \end{drcases}
  \to DevOps
  \begin{dcases}
  \text{价值观} \\
  \text{原则} \\
  \text{方法} \\
  \text{实践} \\
  \text{工具}
  \end{dcases} \\
  \begin{drcases}
  \text{敏捷价值观} \\
  \text{精益价值观}
  \end{drcases}
  \to DevOps \text{价值观} \\
  \begin{drcases}
  \text{敏捷原则} \\
  \text{精益原则}
  \end{drcases}
  \to DevOps \text{原则} \\
  \end{gather*}$$
  + 价值观
    + $$\begin{align*}
        \text{个体和互动} & > \text{流程和工具} \\
        \text{工作的系统} & > \text{详尽的文档} \\
        \text{客户以及程序员合作} & > \text{合同谈判} \\
        \text{响应变化} & > \text{遵循计划} 
        \end{align*}$$
  + ~~原则~~
  + 方法
    + $$\begin{gather*}
        DevOps \text{方法} \gets \text{敏捷方法}
        \begin{dcases}
        Scrum & \text{迭代式增量软件开发过程} \\
        XP & \text{极限编程} \\
        Kanban & \text{看板} \\
        \cdots
        \end{dcases}
        \end{gather*}$$ 
  + 实践
    + $$\begin{gather*}
        DevOps \text{实践}
        \begin{dcases}
        \cancel{\text{管理实践}} \\
        \text{技术实践}
        \end{dcases}
        \end{gather*}$$ 
  + **工具**

<br>

## DevOps研究现状

$$\begin{gather*}
  DevOps \xrightarrow{\text{支持}}
  \begin{dcases}
  \text{微服务} \\
  \text{容器} \\
  \text{持续集成} \\
  \text{持续交付} \\
  \cdots
  \end{dcases}
  \end{gather*}$$ 

<br>

## DevOps流程

$$\begin{gather*}
  \text{需求} \to \text{计划} \to \overbrace{\overbrace{\text{开发} \to \text{构建} \to \text{测试}}^{集成} \to \text{发布}}^{DevOps\text{核心流程}} \to \text{运营} \\
  \begin{align*}
  \text{开发} &
  \begin{dcases}
  \text{协同开发工具} \\
  \text{版本管理工具} \\
  \text{编译工具} \\
  \text{单元测试工具}
  \end{dcases} \\
  \text{测试} & \ \text{自动化测试工具} \\
  \text{集成} & \ \text{持续集成工具} \\
  \text{发布} & \ \text{配置管理工具} \\
  \text{运营} & \ \text{监控工具}
  \end{align*} 
  \end{gather*}$$
  
<br>

## DevOps工具集

+ 协同开发工具
  + JIRA
  + Kanboard
  + Rally
+ 版本管理工具
  + Git
  + GitHub
  + GitLab
  + Subversion
  + Mercurial
+ 编译工具
  + Ant
  + Maven
  + Gradle
  + MSBuild
+ 单元测试工具
  + JUnit
+ 自动化测试工具
  + Selenium
  + Cucumber
  + FitNesse
+ 持续集成工具
  + Jenkins
  + Bamboo
  + Travis CI
+ 配置管理工具
  + Chef
  + Puppet
  + Ansible
+ 监控工具
  + Nagios
  + Zabbix
