# liaokangxianv.github.io[yuzhicai-timeline.html](https://github.com/user-attachments/files/24381116/yuzhicai-timeline.html)
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=no">
    <title>预制菜发展时间轴 - iframe适配版</title>
    <style>
        /* 核心重置 & iframe适配 */
        html, body {
            margin: 0;
            padding: 0;
            width: 100%;
            height: 100%;
            overflow: hidden; /* 禁止iframe内滚动 */
            background: transparent; /* iframe背景透明 */
        }
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: -apple-system, BlinkMacSystemFont, "PingFang SC", "Microsoft YaHei", sans-serif;
        }
        .timeline-wrapper {
            width: 100%;
            height: 100%;
            max-width: 900px;
            margin: 0 auto;
            padding: 20px 15px;
            position: relative;
            overflow-y: auto; /* 仅内容区允许纵向滚动 */
            -webkit-overflow-scrolling: touch; /* 移动端顺滑滚动 */
        }
        /* 时间节点容器 */
        .timeline-node {
            position: relative;
            margin: 40px 0;
            display: flex;
            align-items: flex-start;
            cursor: pointer;
        }
        /* 圆点样式 */
        .node-dot {
            width: 32px;
            height: 32px;
            border-radius: 50%;
            background: #fff;
            border: 3px solid;
            position: relative;
            z-index: 2;
            transition: all 0.3s ease;
            flex-shrink: 0;
            margin-right: 20px;
        }
        /* 圆点配色 */
        .dot-1 { border-color: #F198B8; background: #FDF2F8; }
        .dot-2 { border-color: #F59E0B; background: #FEF3C7; }
        .dot-3 { border-color: #EC4899; background: #FCE7F3; }
        .dot-4 { border-color: #94A3B8; background: #E2E8F0; }
        .dot-5 { border-color: #FBBF24; background: #FEF9C3; }
        /* 圆点悬停效果 */
        .timeline-node:hover .node-dot {
            transform: scale(1.15);
            box-shadow: 0 0 12px rgba(0,0,0,0.1);
        }
        /* 节点内容区 */
        .node-content {
            flex: 1;
            position: relative;
        }
        /* 时期标题 */
        .node-title {
            font-size: 16px;
            font-weight: 700;
            color: #1F2937;
            margin-bottom: 6px;
            transition: color 0.3s ease;
            word-break: break-all; /* 防止标题溢出 */
        }
        .timeline-node:hover .node-title {
            color: #EC4899;
        }
        /* 详情文本 */
        .node-detail {
            max-height: 0;
            opacity: 0;
            overflow: hidden;
            transition: all 0.4s ease;
            font-size: 12px;
            line-height: 1.7;
            color: #4B5563;
            padding: 0 12px;
            border-left: 2px solid #E5E7EB;
            margin-top: 8px;
            word-break: break-word; /* 防止文本溢出 */
        }
        .timeline-node:hover .node-detail {
            max-height: 800px;
            opacity: 1;
            padding: 8px 12px;
        }
        /* 移动端适配 */
        @media (max-width: 768px) {
            .node-dot { width: 26px; height: 26px; margin-right: 15px; }
            .node-title { font-size: 14px; }
            .node-detail { font-size: 11px; }
        }
        /* iframe小尺寸适配 */
        @media (max-width: 480px) {
            .timeline-wrapper { padding: 10px 8px; }
            .timeline-node { margin: 20px 0; }
            .node-dot { width: 22px; height: 22px; margin-right: 10px; border-width: 2px; }
        }
    </style>
</head>
<body>
    <div class="timeline-wrapper">
        <!-- 节点1：原始期 -->
        <div class="timeline-node">
            <div class="node-dot dot-1"></div>
            <div class="node-content">
                <div class="node-title">原始期（20世纪80—90年代）</div>
                <div class="node-detail">
                    中国预制菜有着深厚的历史文化渊源，腊肉、腌菜、风干水产等传统食品加工技术构成了预制菜的早期形态；随着现代罐头和速冻技术的引入，上海等地于20世纪80年代开始生产速冻饺子、包子等产品，以出口创汇为主要导向，形成了现代预制菜的雏形。
                </div>
            </div>
        </div>

        <!-- 节点2：孕育期 -->
        <div class="timeline-node">
            <div class="node-dot dot-2"></div>
            <div class="node-content">
                <div class="node-title">孕育期（2000—2015年）</div>
                <div class="node-detail">
                    20世纪80年代到90年代，国际快餐品牌如肯德基、麦当劳进入中国市场，引领了快速食品的潮流，中国也开始出现净菜加工配送工厂，这是中国预制菜的萌芽；2000年前后，部分餐饮企业对肉类、水产等原材料进行加工，预制菜深加工度逐步提高，但受限于冷链技术和消费习惯，发展较为缓慢；2014年前后，外卖行业爆发，推动了预制菜B端需求的激增；餐饮连锁化进程推动了中央厨房模式的兴起，真功夫等中式快餐企业率先建立标准化供应链体系，通过工业化生产实现了中餐的标准化输出。
                </div>
            </div>
        </div>

        <!-- 节点3：加速发展期 -->
        <div class="timeline-node">
            <div class="node-dot dot-3"></div>
            <div class="node-content">
                <div class="node-title">加速发展期（2016—2022年）</div>
                <div class="node-detail">
                    2016年，京东物流首次使用“预制菜货柜”标签对相关品类进行归类，标志着“预制菜”概念的正式出现；2020年，疫情防控催生的居家消费需求与出口企业转内销压力叠加，推动预制菜从B端向C端快速渗透；2021年，广东省湛江市通过“政府+龙头企业+媒体”协同模式，推广水产预制菜，解决了南美白对虾、金鲳鱼等农产品滞销问题；2021年，“预制菜第一股”味知香成功登陆A股，厚生、红杉、高瓴等头部资本开始进入，多家上市企业纷纷布局预制菜产业；2022年，广东省出台《关于加快推进广东预制菜产业高质量发展十条措施》，成为首个省级预制菜专项政策，同期山东烟台推动禽肉预制菜生产线建设、临沂兰陵县打造蔬菜预制菜品类，形成地方特色产业集群。
                </div>
            </div>
        </div>

        <!-- 节点4：规范整合期 -->
        <div class="timeline-node">
            <div class="node-dot dot-4"></div>
            <div class="node-content">
                <div class="node-title">规范整合期（2023年至今）</div>
                <div class="node-detail">
                    2023年，锅圈食品登陆港交所，预制菜市场前景被广泛看好；2024年3月，市场监管总局等六部门联合印发《关于加强预制菜食品安全监管 促进产业高质量发展的通知》，首次在国家层面明确预制菜的定义和范围，规定不使用防腐剂，标志着行业监管框架基本确立；2025年9月，国家卫生健康委主导的《预制菜食品安全国家标准》草案通过审查，将餐饮门店使用预制菜纳入强制信息披露范畴，产业进入规范化、高质量发展新阶段。
                </div>
            </div>
        </div>
    </div>

    <!-- 可选：iframe自适应高度脚本 -->
    <script>
        // 监听内容高度变化，向父窗口发送高度信息（如需自适应iframe高度）
        function sendIframeHeight() {
            const height = document.querySelector('.timeline-wrapper').scrollHeight + 40;
            // 向父窗口发送消息
            if (window.parent !== window) {
                window.parent.postMessage({
                    type: 'iframeHeight',
                    height: height
                }, '*'); // 生产环境建议替换为具体域名
            }
        }

        // 初始加载和窗口大小变化时发送高度
        window.addEventListener('load', sendIframeHeight);
        window.addEventListener('resize', sendIframeHeight);
        
        // 监听节点悬停导致的高度变化
        document.querySelectorAll('.timeline-node').forEach(node => {
            node.addEventListener('mouseenter', sendIframeHeight);
            node.addEventListener('mouseleave', sendIframeHeight);
        });
    </script>
</body>
</html>
