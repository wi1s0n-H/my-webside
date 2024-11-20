<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wilson的个人网站</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        /* 这里放入之前的所有CSS样式 */
    </style>
</head>
<body>
    <!-- 导航栏 -->
    <div class="navbar">
        <a href="#" class="nav-link">首页</a>
        <a href="#achievements" class="nav-link">成就</a>
        <a href="#education" class="nav-link">教育经历</a>
        <a href="#social" class="nav-link">社交媒体</a>
    </div>

    <!-- 其他部分的HTML内容 -->
</body>
</html>
<!-- 成就展示部分 -->
<section class="achievements" id="achievements">
    <div class="section-header">
        <h2>主要成就</h2>
        <p class="subtitle">我的成长历程</p>
    </div>

    <!-- 体育成就 -->
    <div class="achievement-card" data-category="sports">
        <div class="card-header">
            <i class="fas fa-trophy"></i>
            <h3>体育成就</h3>
            <span class="date">2023</span>
        </div>
        <div class="card-content">
            <h4>龙舟校队主力队员</h4>
            <p class="preview">澳门科技大学龙舟队</p>
            <div class="details">
                <ul>
                    <li>2023年澳门科技大学龙舟队
                        <ul>
                            <li>参与澳门科技大学龙舟队训练</li>
                            <li>代表学校参加多项赛事</li>
                            <li>展现出色的团队协作能力</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </div>

    <!-- 音乐成就 -->
    <div class="achievement-card" data-category="music">
        <div class="card-header">
            <i class="fas fa-music"></i>
            <h3>音乐成就</h3>
            <span class="date">2023</span>
        </div>
        <div class="card-content">
            <h4>管弦乐团萨克斯手</h4>
            <p class="preview">校园音乐会首席萨克斯演奏者</p>
            <div class="details">
                <ul>
                    <li>全国业余萨克斯九级证书
                        <ul>
                            <li>展现专业的演奏技巧</li>
                            <li>获得评委的高度认可</li>
                        </ul>
                    </li>
                    <li>2023年澳门科技大学管弦乐团
                        <ul>
                            <li>担任萨克斯独奏表演嘉宾</li>
                            <li>演奏曲目获得观众热烈好评</li>
                        </ul>
                    </li>
                    <li>2018年全国青少年才艺大赛
                        <ul>
                            <li>萨克斯演奏项目一等奖</li>
                            <li>展现出色的音乐表现力和技巧</li>
                        </ul>
                    </li>
                </ul>
            </div>
        </div>
    </div>
</section>

<style>
    .achievements {
        padding: 80px 20px;
        background: linear-gradient(135deg, #e0eafc, #cfdef3);
    }

    .section-header {
        text-align: center;
        margin-bottom: 40px;
    }

    .section-header h2 {
        font-size: 2.5em;
        color: #2c3e50;
        margin-bottom: 10px;
    }

    .section-header .subtitle {
        color: #666;
        font-size: 1.2em;
    }

    .achievement-card {
        background: white;
        border-radius: 15px;
        padding: 25px;
        margin: 20px auto;
        max-width: 800px;
        box-shadow: 0 5px 15px rgba(0,0,0,0.1);
        transition: all 0.3s ease;
    }

    .achievement-card:hover {
        transform: translateY(-5px);
        box-shadow: 0 8px 25px rgba(0,0,0,0.15);
    }

    .card-header {
        display: flex;
        align-items: center;
        margin-bottom: 20px;
    }

    .card-header i {
        font-size: 2em;
        color: #3498db;
        margin-right: 15px;
    }

    .card-header h3 {
        font-size: 1.5em;
        color: #2c3e50;
        margin: 0;
    }

    .card-header .date {
        margin-left: auto;
        color: #666;
    }

    .card-content h4 {
        color: #2c3e50;
        font-size: 1.2em;
        margin-bottom: 10px;
    }

    .card-content .preview {
        color: #666;
        margin-bottom: 15px;
    }

    .card-content .details {
        background: #f8f9fa;
        border-radius: 10px;
        padding: 20px;
    }

    .card-content ul {
        margin: 0;
        padding-left: 20px;
    }

    .card-content ul li {
        margin-bottom: 10px;
        color: #2c3e50;
    }

    .card-content ul ul {
        margin-top: 5px;
    }

    .card-content ul ul li {
        color: #666;
        margin-bottom: 5px;
    }

    @media (max-width: 768px) {
        .achievement-card {
            margin: 20px;
        }
        
        .card-header {
            flex-direction: column;
            text-align: center;
        }
        
        .card-header i {
            margin: 0 0 10px 0;
        }
        
        .card-header .date {
            margin: 10px 0 0 0;
        }
    }
</style>
