<!DOCTYPE html>
<html lang="zh">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Wilson的个人网站</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css">
    <style>
        /* 全局样式 */
        body {
            margin: 0;
            font-family: Arial, sans-serif;
            background: linear-gradient(135deg, #e0eafc, #cfdef3);
        }

        /* 导航栏样式 */
        .navbar {
            background-color: #333;
            padding: 15px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 1000;
        }

        .navbar a {
            color: #ffffff;
            text-decoration: none;
            margin: 0 15px;
            font-weight: bold;
            transition: color 0.3s ease;
        }

        .navbar a:hover {
            color: #f0f0f0;
        }

        /* 成就展示部分样式 */
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

        /* 教育经历部分样式 */
        .education {
            padding: 80px 20px;
            background: linear-gradient(135deg, #e0eafc, #cfdef3);
        }

        .education-card {
            background: white;
            border-radius: 15px;
            padding: 25px;
            margin: 20px auto;
            max-width: 800px;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .education-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        /* 社交媒体部分样式 */
        .social {
            padding: 80px 20px;
            background: linear-gradient(135deg, #e0eafc, #cfdef3);
        }

        .social-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
            gap: 20px;
            max-width: 1000px;
            margin: 0 auto;
        }

        .social-card {
            background: white;
            border-radius: 15px;
            padding: 20px;
            text-align: center;
            box-shadow: 0 5px 15px rgba(0,0,0,0.1);
            transition: all 0.3s ease;
        }

        .social-card:hover {
            transform: translateY(-5px);
            box-shadow: 0 8px 25px rgba(0,0,0,0.15);
        }

        .social-card a {
            text-decoration: none;
            color: inherit;
        }

        .social-card i {
            font-size: 40px;
            margin-bottom: 10px;
            color: #00a1d6;
        }

        .social-card h3 {
            font-family: 'Poppins', sans-serif;
            font-size: 1.2em;
            color: #2c3e50;
        }

        .social-card:nth-child(2) i { color: #e4405f; }
        .social-card:nth-child(3) i { color: #1DA1F2; }
        .social-card:nth-child(4) i { color: #FF0000; }

        @media (max-width: 768px) {
            .achievement-card, .education-card {
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
</head>
<body>
    <!-- 导航栏 -->
    <div class="navbar">
        <a href="#" class="nav-link">首页</a>
        <a href="#achievements" class="nav-link">成就</a>
        <a href="#education" class="nav-link">教育经历</a>
        <a href="#social" class="nav-link">社交媒体</a>
    </div>

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

    <!-- 教育经历部分 -->
    <section class="education" id="education">
        <div class="section-header">
            <h2>教育经历</h2>
            <p class="subtitle">学习成长之路</p>
        </div>

        <div class="education-timeline">
            <!-- 大学 -->
            <div class="education-card">
                <div class="card-header">
                    <i class="fas fa-university"></i>
                    <h3>澳门科技大学</h3>
                    <span class="date">2023-2027</span>
                </div>
                <div class="card-content">
                    <h4>商学院 · 工商管理专业</h4>
                    <p class="preview">本科在读</p>
                    <div class="details">
                        <ul>
                            <li>主修课程
                                <ul>
                                    <li>管理学原理</li>
                                    <li>市场营销</li>
                                    <li>财务管理</li>
                                    <li>组织行为学</li>
                                </ul>
                            </li>
                            <li>在校表现
                                <ul>
                                    <li>龙舟校队主力队员</li>
                                    <li>管弦乐团萨克斯手</li>
                                    <li>参与多个商业实践项目</li>
                                </ul>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- 高中 -->
            <div class="education-card">
                <div class="card-header">
                    <i class="fas fa-school"></i>
                    <h3>东莞市南城开心实验学校</h3>
                    <span class="date">2020-2023</span>
                </div>
                <div class="card-content">
                    <h4>高中部</h4>
                    <p class="preview">高中学习阶段</p>
                    <div class="details">
                        <ul>
                            <li>学习成果
                                <ul>
                                    <li>成功考入澳门科技大学</li>
                                    <li>获得优秀学生称号</li>
                                </ul>
                            </li>
                            <li>课外活动
                                <ul>
                                    <li>参与校园文艺演出</li>
                                    <li>担任班级干部</li>
                                </ul>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>

            <!-- 初中 -->
            <div class="education-card">
                <div class="card-header">
                    <i class="fas fa-school"></i>
                    <h3>东莞市南城阳光实验中学</h3>
                    <span class="date">2017-2020</span>
                </div>
                <div class="card-content">
                    <h4>初中部</h4>
                    <p class="preview">初中学习阶段</p>
                    <div class="details">
                        <ul>
                            <li>学习成果
                                <ul>
                                    <li>顺利升入重点高中</li>
                                    <li>多次获得三好学生称号</li>
                                </ul>
                            </li>
                            <li>课外活动
                                <ul>
                                    <li>参与校园文化活动</li>
                                    <li>开始学习萨克斯</li>
                                </ul>
                            </li>
                        </ul>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 社交媒体部分 -->
    <section class="social" id="social">
        <div class="section-header">
            <h2>社交媒体</h2>
            <p class="subtitle">与我联系</p>
        </div>

        <div class="social-grid">
            <div class="social-card">
                <a href="https://space.bilibili.com/502691438" target="_blank">
                    <i class="fas fa-tv"></i>
                    <h3>Bilibili</h3>
                </a>
            </div>
            <div class="social-card">
                <a href="https://www.instagram.com/hengwzzzzzzzz/" target="_blank">
                    <i class="fab fa-instagram"></i>
                    <h3>Instagram</h3>
                </a>
            </div>
            <div class="social-card">
                <a href="https://x.com/Hwwwzhhh" target="_blank">
                    <i class="fab fa-twitter"></i>
                    <h3>Twitter</h3>
                </a>
            </div>
            <div class="social-card">
                <a href="https://www.youtube.com/feed/you" target="_blank">
                    <i class="fab fa-youtube"></i>
                    <h3>YouTube</h3>
                </a>
            </div>
        </div>
    </section>
</body>
</html>
