<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>王紫滕的个人主页</title>
    <!-- 引入GitHub Pages默认支持的简易样式（可选，也可删除） -->
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/github-markdown-css@5.5.1/github-markdown.min.css">
    <style>
        /* 核心布局样式 */
        .header-container {
            display: flex;
            align-items: center;
            gap: 2rem; /* 头像和信息的间距 */
            margin: 2rem 0;
            flex-wrap: wrap; /* 移动端自动换行 */
        }
        .avatar {
            width: 160px; /* 头像宽度，可调整 */
            height: 160px; /* 头像高度，可调整 */
            border-radius: 8px; /* 方形头像，想要圆形改为50% */
            object-fit: cover; /* 保持头像比例不拉伸 */
            border: 1px solid #eee; /* 轻微边框，可选 */
            box-shadow: 0 2px 4px rgba(0,0,0,0.1); /* 轻微阴影，可选 */
        }
        .info-container {
            flex: 1; /* 个人信息占满剩余宽度 */
            min-width: 280px; /* 移动端最小宽度，避免太挤 */
        }
        /* 调整标题和列表间距，适配GitHub风格 */
        .info-container h1 {
            margin: 0 0 0.5rem 0;
            font-size: 2rem;
        }
        .info-container ul {
            list-style: none;
            padding: 0;
            margin: 0;
            line-height: 1.8;
        }
        .info-container li::before {
            content: "•"; /* 列表前缀符号，可选 */
            color: #666;
            margin-right: 0.5rem;
        }
        /* 下方内容区域间距 */
        .content-section {
            margin: 2.5rem 0;
            padding-top: 1rem;
            border-top: 1px solid #eee; /* 分隔线，可选 */
        }
        /* 响应式适配手机 */
        @media (max-width: 768px) {
            .header-container {
                justify-content: center; /* 移动端居中 */
                text-align: center;
            }
            .info-container li::before {
                display: none; /* 移动端隐藏列表前缀 */
            }
        }
    </style>
</head>
<body class="markdown-body"> <!-- 继承GitHub Markdown默认样式 -->

<!-- 顶部：左头像 + 右个人信息 -->
<div class="header-container">
    <!-- 头像：替换src为你的头像路径（本地/网络都可） -->
    <img src="https://example.com/your-avatar.jpg" alt="个人头像" class="avatar">
    
    <!-- 个人信息 -->
    <div class="info-container">
        <h1>王紫滕</h1>
        <ul>
            <li>邮箱：<a href="mailto:2233711359@stu.xjtu.edu.cn">2233711359@stu.xjtu.edu.cn</a></li>
            <li>电话/微信：<a href="tel:+8613258905505">+86 13258905505</a>（微信同号）</li>
            <li>学校：西安交通大学 | 软件工程（本科）</li>
            <li>年级：2023级（预计2027年毕业）</li>
            <li>绩点：91.8（排名：6/135）</li>
        </ul>
    </div>
</div>

<!-- 下方：教育经历 -->
<div class="content-section">
    <h2>📚 教育经历</h2>
    <ul>
        <li><strong>西安交通大学</strong> | 本科生 | 软件工程</li>
        <li>时间：2023.09 -- 2027.06（预计）</li>
        <li>大二智育成绩：91.8，排名：6/135</li>
    </ul>
</div>

<!-- 下方：实习经历 -->
<div class="content-section">
    <h2>💼 实习经历</h2>
    <ul>
        <li><strong>华为 2012 实验室 - 编译器实验室</strong> | 软件开发工程师（实习生）</li>
        <li>时间：2025.8 -- 2025.9</li>
        <li><strong>工作职责：</strong>
            <ol>
                <li>参与性能优化项目，针对编译器 SPEC 子项进行性能调优，分析运行瓶颈并优化关键路径；</li>
                <li>通过 Python 脚本实现自动化性能测试（一键构建、执行、数据采集与报告生成）；</li>
                <li>Linux 环境下使用性能分析工具，定位高 CPU 占用、低缓存命中率等问题；</li>
                <li>优化性能数据存储与分析流程，自动生成可视化图表辅助团队评估效果；</li>
                <li>跨团队协作，保障优化版本在多平台的功能正确性与性能稳定性。</li>
            </ol>
        </li>
        <li><strong>工作成果：</strong>参与 dev-19x 项目，x264 子项性能提升 9%，Python 子项性能提升 7%。</li>
    </ul>
</div>

<!-- 下方：项目经历 -->
<div class="content-section">
    <h2>🚀 项目经历</h2>
    
    <h3>基于香橙派的疲劳驾驶检测与预警系统</h3>
    <ul>
        <li>项目类型：国家级大学生创新创业项目 | 角色：项目负责人</li>
        <li>时间：2025.5 -- 2026.5（预计）</li>
        <li><strong>研究背景：</strong>解决传统疲劳检测延迟高、部署成本高的问题，探索低成本嵌入式平台的实时检测方案。</li>
        <li><strong>研究方法：</strong>香橙派部署轻量化 YOLOv5 模型，实时追踪驾驶员面部关键区域；结合语音模块预警，采用公开数据集+迁移学习，ONNX 格式适配嵌入式设备。</li>
        <li><strong>阶段成果：</strong>基于 YOLOv5m 预训练模型完成训练与 ONNX 导出，验证集 mAP@0.5 达 95.96%，当前进行嵌入式部署与性能验证。</li>
        <li><strong>承担工作：</strong>项目总体设计与管理、文献调研、模型改进与训练、实验评估与技术报告撰写。</li>
    </ul>

    <h3>音乐推荐系统</h3>
    <ul>
        <li>项目类型：开发项目 | 角色：核心小组成员</li>
        <li>时间：2025.7 -- 2025.7</li>
        <li><strong>项目简介：</strong>基于 Web 的音乐推荐平台，支持用户管理、歌曲检索/播放/上传，前后端分离架构提升扩展性与维护效率。</li>
        <li><strong>承担工作（全栈开发）：</strong>
            <ol>
                <li>设计实现系统架构（Vue3 + Spring Boot + MySQL）；</li>
                <li>开发用户交互界面与核心后端服务，保障功能稳定与性能优化；</li>
                <li>使用 Git/GitHub 进行代码托管与协作开发。</li>
            </ol>
        </li>
        <li><strong>项目成果：</strong>完成核心模块开发，实现系统全部主要功能。</li>
    </ul>
</div>

<!-- 下方：所获表彰 -->
<div class="content-section">
    <h2>🏆 所获表彰</h2>
    <ul>
        <li>学生荣誉：优秀学生、文治书院团委实践部优秀干事</li>
        <li>奖学金：国家励志奖学金</li>
    </ul>
</div>

<!-- 下方：专业技能 -->
<div class="content-section">
    <h2>🛠️ 专业技能</h2>
    <ul>
        <li><strong>技术栈：</strong>Python, C++, Shell, Java, VUE, Spring Boot, Maven, MySQL</li>
        <li><strong>开发工具与框架：</strong>Git, PyCharm, Kaggle, IntelliJ IDEA, VS Code, MySQL Workbench, Docker</li>
        <li><strong>知识领域：</strong>机器学习（ML）、计算机视觉（CV）、PyTorch、OpenCV、数据结构与算法、操作系统、离散数学</li>
        <li><strong>外语能力：</strong>CET-4 551 分，CET-6 468 分，具备英文文献阅读与撰写能力</li>
    </ul>
</div>

</body>
</html>
