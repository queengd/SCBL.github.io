<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>神川百楽的CTF工具箱</title>
    <style>
        /* 基础变量 */
        :root {
            --primary-color: #4361ee;
            --secondary-color: #3f37c9;
            --accent-color: #4895ef;
            --text-color: #ffffff; /* 改为白色文本以适应黑色背景 */
            --light-text: #f8f9fa;
            --bg-color: #000000; /* 背景改为黑色 */
            --dark-bg: #1a1a2e;
            --border-color: #333333; /* 调整边框颜色以适应黑色背景 */
            --shadow: 0 4px 6px rgba(0, 0, 0, 0.5); /* 阴影加深 */
            --transition: all 0.3s ease;
        }

        /* 基础样式 */
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            font-family: 'Helvetica Neue', Arial, 'PingFang SC', 'Microsoft YaHei', sans-serif;
            line-height: 1.6;
            color: var(--text-color);
            background-color: var(--bg-color);
            overflow-x: hidden;
            position: relative;
        }

        /* 二进制雨效果 */
        #matrix-rain {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            z-index: -1;
            opacity: 0.8; /* 降低不透明度以免影响内容阅读 */
        }

        a {
            text-decoration: none;
            color: inherit;
            transition: var(--transition);
        }

        /* 导航栏 */
        .navbar {
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            background-color: rgba(0, 0, 0, 0.95); /* 改为黑色半透明 */
            backdrop-filter: blur(10px);
            box-shadow: var(--shadow);
            z-index: 1000;
            padding: 1rem 0;
            transition: var(--transition);
        }

        .navbar.scrolled {
            padding: 0.5rem 0;
            background-color: rgba(0, 0, 0, 0.98); /* 改为黑色半透明 */
        }

        .nav-container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 0 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--primary-color);
        }

        .nav-links {
            display: flex;
            gap: 2rem;
        }

        .nav-links a {
            font-weight: 500;
            position: relative;
            padding: 0.5rem 0;
        }

        .nav-links a::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 0;
            width: 0;
            height: 2px;
            background-color: var(--primary-color);
            transition: var(--transition);
        }

        .nav-links a:hover::after,
        .nav-links a.active::after {
            width: 100%;
        }

        /* 英雄区域 */
        .hero {
            min-height: 100vh;
            display: flex;
            align-items: center;
            padding: 8rem 2rem 4rem;
            background: linear-gradient(135deg, rgba(0, 0, 0, 0.8) 0%, rgba(0, 0, 0, 0.9) 100%); /* 改为黑色渐变 */
            position: relative;
            overflow: hidden;
        }

        .hero::before {
            content: '';
            position: absolute;
            top: -50%;
            right: -50%;
            width: 100%;
            height: 200%;
            background: radial-gradient(circle, rgba(67, 97, 238, 0.1) 0%, rgba(67, 97, 238, 0) 70%);
            z-index: 0;
        }

        .hero-content {
            max-width: 1200px;
            margin: 0 auto;
            position: relative;
            z-index: 1;
            width: 100%;
        }

        .hero-text {
            max-width: 600px;
        }

        .hero h1 {
            font-size: 3.5rem;
            font-weight: 700;
            margin-bottom: 1.5rem;
            line-height: 1.2;
            color: var(--text-color);
        }

        .hero p {
            font-size: 1.25rem;
            margin-bottom: 2rem;
            color: var(--text-color);
            opacity: 0.9;
        }

        .btn {
            display: inline-block;
            padding: 0.75rem 1.5rem;
            background-color: var(--primary-color);
            color: white;
            border-radius: 50px;
            font-weight: 500;
            transition: var(--transition);
            border: none;
            cursor: pointer;
            font-size: 1rem;
        }

        .btn:hover {
            background-color: var(--secondary-color);
            transform: translateY(-2px);
            box-shadow: 0 6px 12px rgba(67, 97, 238, 0.2);
        }

        .btn-outline {
            background-color: transparent;
            border: 2px solid var(--primary-color);
            color: var(--primary-color);
            margin-left: 1rem;
        }

        .btn-outline:hover {
            background-color: var(--primary-color);
            color: white;
        }

        /* 项目区域 */
        .section {
            padding: 6rem 2rem;
            background-color: rgba(0, 0, 0, 0.7); /* 半透明黑色背景 */
            position: relative;
            z-index: 1;
        }

        .section-title {
            text-align: center;
            margin-bottom: 4rem;
            position: relative;
        }

        .section-title h2 {
            font-size: 2.5rem;
            font-weight: 700;
            display: inline-block;
            position: relative;
            padding-bottom: 1rem;
        }

        .section-title h2::after {
            content: '';
            position: absolute;
            bottom: 0;
            left: 50%;
            transform: translateX(-50%);
            width: 80px;
            height: 4px;
            background-color: var(--primary-color);
            border-radius: 2px;
        }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fill, minmax(300px, 1fr));
            gap: 2rem;
            max-width: 1200px;
            margin: 0 auto;
        }

        .project-card {
            background-color: rgba(30, 30, 30, 0.8); /* 深灰色半透明背景 */
            border-radius: 10px;
            overflow: hidden;
            box-shadow: var(--shadow);
            transition: var(--transition);
            cursor: pointer;
            border: 1px solid rgba(67, 97, 238, 0.3); /* 添加边框 */
        }

        .project-card:hover {
            transform: translateY(-10px) scale(1.02);
            box-shadow: 0 15px 30px rgba(67, 97, 238, 0.2);
            border-color: var(--primary-color); /* 悬停时边框高亮 */
        }

        .project-image {
            height: 200px;
            background-size: cover;
            background-position: center;
            display: flex;
            justify-content: center;
            align-items: center;
        }

        .tool-icon {
            width: 60px;
            height: 60px;
            transition: transform 0.3s;
        }

        .project-card:hover .tool-icon {
            transform: rotate(15deg) scale(1.1);
        }

        .project-content {
            padding: 1.5rem;
        }

        .project-title {
            font-size: 1.25rem;
            font-weight: 600;
            margin-bottom: 0.5rem;
        }

        .project-description {
            color: #aaa; /* 浅灰色描述文字 */
            margin-bottom: 1rem;
            font-size: 0.95rem;
        }

        .project-tags {
            display: flex;
            flex-wrap: wrap;
            gap: 0.5rem;
            margin-bottom: 1.5rem;
        }

        .tag {
            background-color: rgba(67, 97, 238, 0.2); /* 半透明标签背景 */
            color: #aab7ff; /* 浅蓝色标签文字 */
            padding: 0.25rem 0.75rem;
            border-radius: 50px;
            font-size: 0.75rem;
            font-weight: 500;
        }

        .project-links {
            display: flex;
            gap: 1rem;
        }

        .project-link {
            font-size: 0.9rem;
            font-weight: 500;
            color: var(--primary-color);
            display: flex;
            align-items: center;
            gap: 0.25rem;
        }

        /* 工具模态框 */
        .modal {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(5px);
            z-index: 1001;
            overflow: auto;
        }

        .modal-content {
            background: #111; /* 深色背景 */
            margin: 5% auto;
            padding: 30px;
            width: 90%;
            max-width: 800px;
            border-radius: 15px;
            position: relative;
            animation: modalOpen 0.3s ease-out;
            border: 1px solid rgba(67, 97, 238, 0.3); /* 添加边框 */
        }

        @keyframes modalOpen {
            from { opacity: 0; transform: translateY(-50px) scale(0.9); }
            to { opacity: 1; transform: translateY(0) scale(1); }
        }

        .close {
            position: absolute;
            right: 25px;
            top: 15px;
            color: #aaa;
            font-size: 35px;
            font-weight: bold;
            cursor: pointer;
            transition: color 0.3s;
        }

        .close:hover {
            color: var(--primary-color);
        }

        .decoder-section {
            margin-bottom: 20px;
            padding: 15px;
            background: rgba(30, 30, 30, 0.5); /* 深灰色半透明背景 */
            border-radius: 8px;
            border: 1px solid rgba(67, 97, 238, 0.2); /* 添加边框 */
        }

        .decoder-section h2 {
            color: var(--primary-color);
            margin-top: 0;
        }

        .decoder-section textarea {
            width: 100%;
            height: 100px;
            margin: 10px 0;
            padding: 8px;
            border: 1px solid #333;
            background-color: rgba(0, 0, 0, 0.5);
            color: #fff;
        }

        .result {
            margin-top: 10px;
            padding: 10px;
            background-color: rgba(0, 0, 0, 0.3);
            border: 1px solid #333;
            min-height: 50px;
            color: #fff;
        }

        /* GIF拆解工具特有样式 */
        .gif-upload-area {
            border: 2px dashed #3498db;
            border-radius: 5px;
            padding: 30px;
            text-align: center;
            margin-bottom: 20px;
            background-color: rgba(0, 0, 0, 0.3);
            transition: all 0.3s;
        }

        .gif-upload-area:hover {
            border-color: #2980b9;
            background-color: rgba(0, 0, 0, 0.5);
        }

        .gif-upload-area.dragover {
            border-color: #27ae60;
            background-color: rgba(0, 30, 0, 0.5);
        }

        .gif-file-input {
            display: none;
        }

        .gif-upload-btn {
            background-color: var(--primary-color);
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-size: 16px;
            transition: var(--transition);
        }

        .gif-upload-btn:hover {
            background-color: var(--secondary-color);
        }

        .gif-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 20px;
        }

        .gif-frame {
            margin: 10px;
            text-align: center;
            background: rgba(30, 30, 30, 0.8);
            padding: 10px;
            border-radius: 5px;
            box-shadow: var(--shadow);
        }

        .gif-frame img {
            max-width: 200px;
            max-height: 200px;
            display: block;
            margin-bottom: 5px;
        }

        .gif-download-btn {
            background-color: var(--primary-color);
            color: white;
            padding: 5px 10px;
            border: none;
            border-radius: 3px;
            cursor: pointer;
            font-size: 14px;
            margin: 5px;
            transition: var(--transition);
        }

        .gif-download-btn:hover {
            background-color: var(--secondary-color);
        }

        .gif-download-all {
            background-color: #e67e22;
            display: block;
            margin: 20px auto;
            padding: 10px 20px;
        }

        .gif-download-all:hover {
            background-color: #d35400;
        }

        .gif-info {
            text-align: center;
            margin: 20px 0;
            color: #7f8c8d;
        }

        .gif-progress-container {
            width: 100%;
            background-color: #333;
            border-radius: 5px;
            margin: 10px 0;
            display: none;
        }

        .gif-progress-bar {
            width: 0%;
            height: 20px;
            background-color: var(--primary-color);
            border-radius: 5px;
            text-align: center;
            line-height: 20px;
            color: white;
        }

        /* 端口扫描工具特有样式 */
        .progress-container {
            width: 100%;
            background-color: #333;
            border-radius: 5px;
            margin: 10px 0;
            display: none;
        }

        .progress-bar {
            width: 0%;
            height: 20px;
            background-color: var(--primary-color);
            border-radius: 5px;
            text-align: center;
            line-height: 20px;
            color: white;
        }

        /* 进制转换工具特有样式 */
        .number-input-group {
            display: flex;
            margin-bottom: 10px;
        }

        .number-input-group label {
            width: 100px;
            font-weight: bold;
        }

        .number-input-group input {
            flex: 1;
            padding: 8px;
            border: 1px solid #333;
            border-radius: 4px;
            background-color: rgba(0, 0, 0, 0.5);
            color: #fff;
        }

        /* 摩斯密码工具特有样式 */
        .morse-options {
            margin: 15px 0;
        }

        .morse-options label {
            margin-right: 15px;
            color: #fff;
        }

        /* 二维码扫描工具特有样式 */
        .qr-upload-area {
            border: 2px dashed #3498db;
            border-radius: 5px;
            padding: 30px;
            text-align: center;
            margin-bottom: 20px;
            background-color: rgba(0, 0, 0, 0.3);
            transition: all 0.3s;
        }

        .qr-upload-area:hover {
            border-color: #2980b9;
            background-color: rgba(0, 0, 0, 0.5);
        }

        .qr-upload-area.dragover {
            border-color: #27ae60;
            background-color: rgba(0, 30, 0, 0.5);
        }

        .qr-file-input {
            display: none;
        }

        .qr-upload-btn {
            background-color: var(--primary-color);
            color: white;
            padding: 10px 20px;
            border: none;
            border-radius: 50px;
            cursor: pointer;
            font-size: 16px;
            transition: var(--transition);
        }

        .qr-upload-btn:hover {
            background-color: var(--secondary-color);
        }

        .qr-preview {
            max-width: 300px;
            max-height: 300px;
            margin: 20px auto;
            display: none;
        }

        .qr-preview img {
            max-width: 100%;
            max-height: 100%;
            display: block;
            margin: 0 auto;
        }

        /* 页脚 */
        footer {
            background-color: var(--dark-bg);
            color: var(--light-text);
            padding: 4rem 2rem;
            text-align: center;
        }

        .footer-content {
            max-width: 1200px;
            margin: 0 auto;
        }

        .footer-links {
            display: flex;
            justify-content: center;
            gap: 2rem;
            margin: 2rem 0;
        }

        .footer-links a {
            color: var(--light-text);
            opacity: 0.7;
            transition: var(--transition);
        }

        .footer-links a:hover {
            opacity: 1;
        }

        .social-links {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin: 2rem 0;
        }

        .social-link {
            width: 40px;
            height: 40px;
            border-radius: 50%;
            background-color: rgba(255, 255, 255, 0.1);
            display: flex;
            align-items: center;
            justify-content: center;
            transition: var(--transition);
        }

        .social-link:hover {
            background-color: var(--primary-color);
            transform: translateY(-3px);
        }

        .copyright {
            opacity: 0.6;
            font-size: 0.9rem;
            margin-top: 2rem;
        }

        /* 响应式设计 */
        @media (max-width: 768px) {
            .nav-container {
                padding: 0 1rem;
            }
            
            .nav-links {
                gap: 1rem;
            }
            
            .hero h1 {
                font-size: 2.5rem;
            }
            
            .hero p {
                font-size: 1.1rem;
            }
            
            .section {
                padding: 4rem 1rem;
            }
            
            .projects-grid {
                grid-template-columns: 1fr;
            }
        }

        @media (max-width: 480px) {
            .hero h1 {
                font-size: 2rem;
            }
            
            .btn-group {
                display: flex;
                flex-direction: column;
                gap: 1rem;
            }
            
            .btn-outline {
                margin-left: 0;
            }
        }
    </style>
</head>
<body>
    <!-- 二进制雨效果 -->
    <canvas id="matrix-rain"></canvas>

    <!-- 导航栏 -->
    <nav class="navbar">
        <div class="nav-container">
            <a href="#" class="logo">神川百楽</a>
            <div class="nav-links">
                <a href="#home" class="active">首页</a>
                <a href="#projects">在线工具</a>
                <a href="#blog">其他在线工具</a>
                <a href="#about">关于CTF</a>
                <a href="#contact">联系方式</a>
            </div>
        </div>
    </nav>

    <!-- 首页英雄区域 -->
    <section id="home" class="hero">
        <div class="hero-content">
            <div class="hero-text">
                <h1>成为CTFer，就现在！&nbsp;</h1>
                <p>网络的乐趣你会在此发现，成为CTFer，为网络全站安全做出贡献。</p>
                <div class="btn-group">
                    <a href="#projects" class="btn">在线工具</a>
                    <a href="#contact" class="btn btn-outline">联系我</a>
                </div>
            </div>
        </div>
    </section>

    <!-- 项目作品区域 -->
    <section id="projects" class="section">
        <div class="section-title">
            <h2>在线工具</h2>
        </div>
        <div class="projects-grid">
            <!-- 第一行 -->
            <!-- 三合一解码工具卡片 -->
            <div class="project-card" onclick="showDecoderModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #4361ee 0%, #3f37c9 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M12,6V8H18V6H12M12,12V14H18V12H12M12,18V20H18V18H12M8,17V11H6V7H10V5H4V9H6V11H8V19H10V21H4V17H8Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">三合一解码工具</h3>
                    <p class="project-description">集成Base64、Unicode和凯撒密码的在线解码工具</p>
                    <div class="project-tags">
                        <span class="tag">JavaScript</span>
                        <span class="tag">工具应用</span>
                        <span class="tag">前端开发</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
            
            <!-- 进制转换工具卡片 -->
            <div class="project-card" onclick="showNumberConverterModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #4cc9f0 0%, #4895ef 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M7,11H9A3,3 0 0,0 12,8A3,3 0 0,0 9,5H7V11M15,5H13A3,3 0 0,0 10,8A3,3 0 0,0 13,11H15V5M12,15A3,3 0 0,0 15,18H17V13H19V18H21V20H5V4H19V6H21V4A2,2 0 0,0 19,2H5A2,2 0 0,0 3,4V20A2,2 0 0,0 5,22H19A2,2 0 0,0 21,20V18A2,2 0 0,0 19,16A2,2 0 0,0 21,14V10A2,2 0 0,0 19,8H17V9A2,2 0 0,1 15,11H13A2,2 0 0,1 11,9V8A2,2 0 0,1 13,6H15A2,2 0 0,1 17,8V9H19A2,2 0 0,1 21,11V13A2,2 0 0,1 19,15A2,2 0 0,1 21,17V19A2,2 0 0,1 19,21H5A2,2 0 0,1 3,19V18H5V19H19V17H5V13H7V15H5V11H7V9H5V6H7V7H5V5H7V6H9V5H11V6H13V5H15V6H17V5H19V6H21V5H19V6Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">进制转换工具</h3>
                    <p class="project-description">支持二进制、十进制和十六进制之间的相互转换</p>
                    <div class="project-tags">
                        <span class="tag">JavaScript</span>
                        <span class="tag">数学工具</span>
                        <span class="tag">CTF工具</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
            
            <!-- 摩斯密码工具卡片 -->
            <div class="project-card" onclick="showMorseCodeModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #3a0ca3 0%, #7209b7 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M12,3L2,12H5V20H19V12H22L12,3M12,7.7L16,11.2V18H14V12H10V18H8V11.2L12,7.7M8.22,7.16L6.64,5.18L5.18,6.64L6.16,8.22L8.22,7.16M17.78,7.16L19.36,5.18L20.82,6.64L19.84,8.22L17.78,7.16M12,10.5C11.17,10.5 10.5,11.17 10.5,12C10.5,12.83 11.17,13.5 12,13.5C12.83,13.5 13.5,12.83 13.5,12C13.5,11.17 12.83,10.5 12,10.5Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">摩斯密码工具</h3>
                    <p class="project-description">摩斯密码编码与解码工具，支持文本与摩斯密码互转</p>
                    <div class="project-tags">
                        <span class="tag">加密解密</span>
                        <span class="tag">工具应用</span>
                        <span class="tag">CTF工具</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
            
            <!-- 第二行 -->
            <!-- GIF拆解工具卡片 -->
            <div class="project-card" onclick="showGifSplitterModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #4895ef 0%, #4361ee 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M11,8H13V16H11V8M7.67,8H4.33C3.53,8 3,8.67 3,9.33V14.67C3,15.33 3.53,16 4.33,16H7.67C8.47,16 9,15.33 9,14.67V9.33C9,8.67 8.47,8 7.67,8M21,10V8H15V16H17V14H19.5V12H17V10H21Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">GIF拆解工具</h3>
                    <p class="project-description">将GIF动画逐帧拆解为静态图片</p>
                    <div class="project-tags">
                        <span class="tag">JavaScript</span>
                        <span class="tag">图像处理</span>
                        <span class="tag">前端开发</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
            
            <!-- 端口扫描工具卡片 -->
            <div class="project-card" onclick="showPortScannerModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #3a0ca3 0%, #7209b7 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M4 15V18H7V20H4V23H2V20H0V18H2V15H4M22 18V20H10V18H22M19 10H22V12H19V15H17V12H14V10H17V7H19V10M9 2V4H6V7H4V4H2V2H4V0H6V2H9Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">端口扫描工具</h3>
                    <p class="project-description">快速检测目标主机的开放端口和服务</p>
                    <div class="project-tags">
                        <span class="tag">网络安全</span>
                        <span class="tag">工具应用</span>
                        <span class="tag">CTF工具</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
            
            <!-- 二维码扫描工具卡片 -->
            <div class="project-card" onclick="showQRScannerModal()">
                <div class="project-image" style="background: linear-gradient(135deg, #f72585 0%, #b5179e 100%);">
                    <svg class="tool-icon" viewBox="0 0 24 24">
                        <path fill="white" d="M3,11H5V13H3V11M11,5H13V9H11V5M9,11H13V15H11V13H9V11M15,11H17V13H19V11H21V13H19V15H21V19H19V21H17V19H13V21H11V17H15V15H17V13H15V11M19,19V15H17V19H19M15,3H21V9H15V3M17,5V7H19V5H17M3,3H9V9H3V3M5,5V7H7V5H5M3,15H9V21H3V15M5,17V19H7V17H5Z"/>
                    </svg>
                </div>
                <div class="project-content">
                    <h3 class="project-title">二维码扫描工具</h3>
                    <p class="project-description">扫描图片中的二维码并解码内容</p>
                    <div class="project-tags">
                        <span class="tag">图像处理</span>
                        <span class="tag">解码工具</span>
                        <span class="tag">CTF工具</span>
                    </div>
                    <div class="project-links">
                        <a href="#" class="project-link">立即使用 →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 技术博客区域 -->
    <section id="blog" class="section" style="background-color: rgba(0, 0, 0, 0.7);">
        <div class="section-title">
            <h2>其他在线工具</h2>
        </div>
        <div class="projects-grid">
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">密码字典生成器</h3>
                    <p class="project-description">生成密码猜测</p>
                    <div class="project-tags">
                        <span class="tag">React</span>
                        <span class="tag">密码</span>
                    </div>
                    <div class="project-links">
                        <a href="https://www.shentoushi.top/tools/dict/index.php" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">EXPKU库</h3>
                    <p class="project-description">打造最大的中文exploid库</p>
                    <div class="project-tags">
                        <span class="tag">后端开发</span>
                        <span class="tag">API设计</span>
                    </div>
                    <div class="project-links">
                        <a href="http://www.expku.com/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
            
            <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">IP查询</h3>
                    <p class="project-description">查询IP源地址。</p>
                    <div class="project-tags">
                        <span class="tag">地址搜索</span>
                        <span class="tag">Web</span>
                    </div>
                    <div class="project-links">
                        <a href="https://haoip.cn/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">javascript工具</h3>
                    <p class="project-description">一个在线的java工具</p>
                    <div class="project-tags">
                        <span class="tag">前端开发</span>
                        <span class="tag">软件工程</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/js/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">CSS工具</h3>
                    <p class="project-description">一个在线的CSS工具</p>
                    <div class="project-tags">
                        <span class="tag">前端开发</span>
                        <span class="tag">网页设计</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/css/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                  <h3 class="project-title">python工具</h3>
                  <p class="project-description">一个在线的python工具</p>
                    <div class="project-tags">
                        <span class="tag">软件工程</span>
                        <span class="tag">软件设计</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/pyc/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">HTML在线工具</h3>
                    <p class="project-description">在线美化html网页</p>
                    <div class="project-tags">
                        <span class="tag">PHP前端</span>
                        <span class="tag">网页设计</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/html/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">PHP在线工具</h3>
                    <p class="project-description">PHP实时在线操作</p>
                    <div class="project-tags">
                        <span class="tag">PHP前端</span>
                        <span class="tag">设计</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/php/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">json工具</h3>
                    <p class="project-description">在线编辑json，语法检查</p>
                    <div class="project-tags">
                        <span class="tag">软件工程</span>语法</div>
                    <div class="project-links">
                        <a href="https://tool.lu/json/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">xml工具</h3>
                    <p class="project-description">在线编辑xml，格式化，压缩</p>
                    <div class="project-tags">
                        <span class="tag">开发</span>
                        <span class="tag">软件</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/xml/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">正则测试工具</h3>
                    <p class="project-description">测试正则表达式，还可以在线生成代码</p>
                    <div class="project-tags">
                        <span class="tag">数学</span>
                        <span class="tag">表达式</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/regex/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
			    <div class="project-card">
                <div class="project-content">
                    <h3 class="project-title">图片压缩</h3>
                    <p class="project-description">在线压缩图片，支持多种格式</p>
                    <div class="project-tags">
                        <span class="tag">压缩</span>
                        <span class="tag">实用功能</span>
                    </div>
                    <div class="project-links">
                        <a href="https://tool.lu/tinyimage/" class="project-link">前往 →</a>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <!-- 关于我区域 -->
    <section id="about" class="section">
        <div class="section-title">
            <h2>关于CTF</h2>
        </div>
        <div style="max-width: 800px; margin: 0 auto; text-align: center;">
            <p style="margin-bottom: 1.5rem; font-size: 1.1rem;">
              CTF（Capture The Flag）是一种网络安全竞赛，参赛者通过破解密码、漏洞利用、逆向工程等技术夺取"flag"（一串特定字符）得分。比赛形式多样，包括解题模式（Jeopardy）和攻防模式（Attack-Defense），涵盖Web安全、二进制分析、密码学等领域。CTF旨在提升实战技能，是黑客技术、团队协作与快速学习的综合挑战，也是选拔安全人才的重要平台。
          </p>
        </div>
    </section>

    <!-- 联系方式区域 -->
    <section id="contact" class="section" style="background-color: rgba(0, 0, 0, 0.7);">
        <div class="section-title">
            <h2>联系方式</h2>
        </div>
        <div style="max-width: 800px; margin: 0 auto; text-align: center;">
            <p style="margin-bottom: 2rem; font-size: 1.1rem;">
                如果您有项目合作或工作机会，欢迎随时联系我
            </p>
            <div class="btn-group">
                <a href="mailto:your.email@example.com" class="btn">发送邮件</a>
                <a href="https://github.com/yourusername" class="btn btn-outline">GitHub</a>
            </div>
        </div>
    </section>

    <!-- 三合一解码工具模态框 -->
    <div id="decoder-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeDecoderModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">三合一解码工具</h1>
                
                <!-- Base64 解码 -->
                <div class="decoder-section">
                    <h2>Base64 解码</h2>
                    <textarea id="base64-input" placeholder="请输入Base64编码内容..."></textarea>
                    <button onclick="decodeBase64()" class="btn">解码</button>
                    <div id="base64-result" class="result"></div>
                </div>

                <!-- Unicode 解码 -->
                <div class="decoder-section">
                    <h2>Unicode 解码</h2>
                    <textarea id="unicode-input" placeholder="请输入Unicode转义序列..."></textarea>
                    <button onclick="decodeUnicode()" class="btn">解码</button>
                    <div id="unicode-result" class="result"></div>
                </div>

                <!-- 凯撒密码解码 -->
                <div class="decoder-section">
                    <h2>凯撒密码解码</h2>
                    <textarea id="caesar-input" placeholder="请输入加密文本..."></textarea>
                    <div style="margin: 15px 0;">
                        <label>位移量：</label>
                        <input type="number" id="caesar-shift" min="1" max="25" value="3">
                        <button onclick="decodeCaesar()" class="btn">解码</button>
                    </div>
                    <div id="caesar-result" class="result"></div>
                </div>
            </div>
        </div>
    </div>

    <!-- 进制转换工具模态框 -->
    <div id="number-converter-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeNumberConverterModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">进制转换工具</h1>
                
                <div class="decoder-section">
                    <h2>进制转换</h2>
                    
                    <div class="number-input-group">
                        <label>二进制：</label>
                        <input type="text" id="binary-input" placeholder="例如: 101010" oninput="convertFromBinary()">
                    </div>
                    
                    <div class="number-input-group">
                        <label>十进制：</label>
                        <input type="text" id="decimal-input" placeholder="例如: 42" oninput="convertFromDecimal()">
                    </div>
                    
                    <div class="number-input-group">
                        <label>十六进制：</label>
                        <input type="text" id="hex-input" placeholder="例如: 2A" oninput="convertFromHex()">
                    </div>
                    
                    <div style="margin-top: 20px;">
                        <button onclick="clearNumberInputs()" class="btn btn-outline">清空</button>
                    </div>
                </div>
                
                <div class="decoder-section">
                    <h2>转换说明</h2>
                    <div class="result">
                        <p>1. 在任意一个输入框中输入数值，其他进制会自动转换</p>
                        <p>2. 二进制: 仅包含0和1的数字 (例如: 101010)</p>
                        <p>3. 十进制: 常规数字 (例如: 42)</p>
                        <p>4. 十六进制: 0-9和A-F (例如: 2A)</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 摩斯密码工具模态框 -->
    <div id="morse-code-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeMorseCodeModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">摩斯密码工具</h1>
                
                <div class="decoder-section">
                    <h2>摩斯密码转换</h2>
                    
                    <div class="morse-options">
                        <label>
                            <input type="radio" name="morse-action" value="encode" checked> 编码 (文本 → 摩斯密码)
                        </label>
                        <label>
                            <input type="radio" name="morse-action" value="decode"> 解码 (摩斯密码 → 文本)
                        </label>
                    </div>
                    
                    <textarea id="morse-input" placeholder="请输入要编码或解码的内容..."></textarea>
                    <button onclick="convertMorseCode()" class="btn">转换</button>
                    <div id="morse-result" class="result"></div>
                </div>
                
                <div class="decoder-section">
                    <h2>摩斯密码参考表</h2>
                    <div class="result">
                        <div style="display: flex; flex-wrap: wrap; gap: 15px;">
                            <div>
                                <h4>字母</h4>
                                <p>A: .-<br>B: -...<br>C: -.-.<br>D: -..<br>E: .<br>F: ..-.<br>G: --.<br>H: ....<br>I: ..<br>J: .---<br>K: -.-<br>L: .-..<br>M: --</p>
                            </div>
                            <div>
                                <h4>字母</h4>
                                <p>N: -.<br>O: ---<br>P: .--.<br>Q: --.-<br>R: .-.<br>S: ...<br>T: -<br>U: ..-<br>V: ...-<br>W: .--<br>X: -..-<br>Y: -.--<br>Z: --..</p>
                            </div>
                            <div>
                                <h4>数字</h4>
                                <p>0: -----<br>1: .----<br>2: ..---<br>3: ...--<br>4: ....-<br>5: .....<br>6: -....<br>7: --...<br>8: ---..<br>9: ----.</p>
                            </div>
                            <div>
                                <h4>标点符号</h4>
                                <p>.: .-.-.-<br>,: --..--<br>?: ..--..<br>': .----.<br>!: -.-.--<br>/: -..-.<br>(: -.--.<br>): -.--.-<br>&: .-...<br>:: ---...<br>;: -.-.-.<br>=: -...-<br>+: .-.-.<br>-: -....-<br>_: ..--.-<br>": .-..-.<br>$: ...-..-<br>@: .--.-.</p>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- GIF拆解工具模态框 -->
    <div id="gif-splitter-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeGifSplitterModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">GIF拆解工具</h1>
                
                <div class="decoder-section">
                    <h2>上传GIF文件</h2>
                    <div class="gif-upload-area" id="gifUploadArea">
                        <p>拖放 GIF 文件到此处 或</p>
                        <button class="gif-upload-btn" id="gifUploadBtn">选择 GIF 文件</button>
                        <input type="file" id="gifFileInput" class="gif-file-input" accept="image/gif">
                        <p class="gif-info">支持最大 10MB 的 GIF 文件</p>
                    </div>
                    
                    <div class="gif-progress-container" id="gifProgressContainer">
                        <div class="gif-progress-bar" id="gifProgressBar">0%</div>
                    </div>
                    
                    <div class="gif-container" id="gifContainer"></div>
                    
                    <button class="gif-download-btn gif-download-all" id="gifDownloadAll" style="display: none;">下载全部帧 (ZIP)</button>
                </div>
            </div>
        </div>
    </div>

    <!-- 端口扫描工具模态框 -->
    <div id="port-scanner-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closePortScannerModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">端口扫描工具</h1>
                
                <div class="decoder-section">
                    <h2>目标扫描</h2>
                    <div style="margin-bottom: 15px;">
                        <label>目标主机/IP：</label>
                        <input type="text" id="scan-target" placeholder="example.com 或 192.168.1.1" style="width: 70%; padding: 8px;">
                    </div>
                    <div style="margin-bottom: 15px;">
                        <label>端口范围：</label>
                        <input type="text" id="port-range" placeholder="1-1024 或 80,443,8080" style="width: 70%; padding: 8px;">
                    </div>
                    <div style="margin-bottom: 15px;">
                        <label>扫描类型：</label>
                        <select id="scan-type" style="padding: 8px;">
                            <option value="tcp">TCP扫描</option>
                            <option value="syn">SYN扫描(快速)</option>
                            <option value="udp">UDP扫描</option>
                        </select>
                    </div>
                    <button onclick="startPortScan()" class="btn">开始扫描</button>
                    <button onclick="stopPortScan()" class="btn btn-outline" style="margin-left: 10px;">停止扫描</button>
                </div>

                <div class="decoder-section">
                    <h2>扫描结果</h2>
                    <div class="progress-container" id="scan-progress-container" style="display: none;">
                        <div class="progress-bar" id="scan-progress-bar">0%</div>
                    </div>
                    <div id="scan-results" style="max-height: 300px; overflow-y: auto; margin-top: 15px;">
                        <table style="width: 100%; border-collapse: collapse;">
                            <thead>
                                <tr style="background-color: rgba(30, 30, 30, 0.5);">
                                    <th style="padding: 8px; text-align: left; border-bottom: 1px solid #333;">端口</th>
                                    <th style="padding: 8px; text-align: left; border-bottom: 1px solid #333;">状态</th>
                                    <th style="padding: 8px; text-align: left; border-bottom: 1px solid #333;">服务</th>
                                    <th style="padding: 8px; text-align: left; border-bottom: 1px solid #333;">响应时间</th>
                                </tr>
                            </thead>
                            <tbody id="scan-results-body">
                                <!-- 扫描结果将在这里动态添加 -->
                            </tbody>
                        </table>
                    </div>
                    <button onclick="exportScanResults()" class="btn" id="export-results-btn" style="margin-top: 15px; display: none;">导出结果(CSV)</button>
                </div>

                <div class="decoder-section">
                    <h2>常用端口参考</h2>
                    <div style="display: flex; flex-wrap: wrap; gap: 10px;">
                        <div style="flex: 1; min-width: 150px;">
                            <h4 style="margin-bottom: 5px;">Web服务</h4>
                            <ul style="list-style-type: none; padding: 0; margin: 0;">
                                <li>80 - HTTP</li>
                                <li>443 - HTTPS</li>
                                <li>8080 - HTTP备用</li>
                                <li>8443 - HTTPS备用</li>
                            </ul>
                        </div>
                        <div style="flex: 1; min-width: 150px;">
                            <h4 style="margin-bottom: 5px;">数据库</h4>
                            <ul style="list-style-type: none; padding: 0; margin: 0;">
                                <li>3306 - MySQL</li>
                                <li>5432 - PostgreSQL</li>
                                <li>27017 - MongoDB</li>
                                <li>6379 - Redis</li>
                            </ul>
                        </div>
                        <div style="flex: 1; min-width: 150px;">
                            <h4 style="margin-bottom: 5px;">远程访问</h4>
                            <ul style="list-style-type: none; padding: 0; margin: 0;">
                                <li>22 - SSH</li>
                                <li>3389 - RDP</li>
                                <li>5900 - VNC</li>
                                <li>23 - Telnet</li>
                            </ul>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 二维码扫描工具模态框 -->
    <div id="qr-scanner-modal" class="modal">
        <div class="modal-content">
            <span class="close" onclick="closeQRScannerModal()">&times;</span>
            <div class="decoder-container">
                <h1 style="text-align: center; color: var(--primary-color);">二维码扫描工具</h1>
                
                <div class="decoder-section">
                    <h2>上传包含二维码的图片</h2>
                    <div class="qr-upload-area" id="qrUploadArea">
                        <p>拖放图片到此处 或</p>
                        <button class="qr-upload-btn" id="qrUploadBtn">选择图片文件</button>
                        <input type="file" id="qrFileInput" class="qr-file-input" accept="image/*">
                        <p class="gif-info">支持 JPG, PNG, GIF 等常见图片格式</p>
                    </div>
                    
                    <div class="qr-preview" id="qrPreview">
                        <img id="qrPreviewImage" src="" alt="预览图">
                    </div>
                    
                    <div id="qr-result" class="result" style="display: none;">
                        <h3>扫描结果：</h3>
                        <div id="qr-result-content"></div>
                        <button onclick="copyQRResult()" class="btn" style="margin-top: 10px;">复制结果</button>
                    </div>
                </div>
                
                <div class="decoder-section">
                    <h2>使用说明</h2>
                    <div class="result">
                        <p>1. 上传包含二维码的图片文件</p>
                        <p>2. 系统会自动检测并解码二维码内容</p>
                        <p>3. 解码结果将显示在下方</p>
                        <p>4. 点击"复制结果"按钮可以复制解码内容</p>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <!-- 页脚 -->
    <footer>
        <div class="footer-content">
            <div class="social-links">
                <a href="https://github.com/yourusername" class="social-link">GitHub</a>
                <a href="https://twitter.com/yourusername" class="social-link">Twitter</a>
                <a href="https://linkedin.com/in/yourusername" class="social-link">LinkedIn</a>
                <a href="https://weibo.com/yourusername" class="social-link">微博</a>
            </div>
            <p class="copyright">© <script>document.write(new Date().getFullYear())</script> 2025&nbsp; 许俊渝 保留所有权利.</p>
        </div>
    </footer>

    <!-- 外部库 -->
    <script src="https://cdnjs.cloudflare.com/ajax/libs/jszip/3.7.1/jszip.min.js"></script>
    <script src="https://cdnjs.cloudflare.com/ajax/libs/FileSaver.js/2.0.5/FileSaver.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/omggif@1.0.10/omggif.min.js"></script>
    <script src="https://cdn.jsdelivr.net/npm/jsqr@1.4.0/dist/jsQR.min.js"></script>
    
    <script>
        // 二进制雨效果
        (function() {
            const canvas = document.getElementById('matrix-rain');
            const ctx = canvas.getContext('2d');
            
            // 设置canvas大小为窗口大小
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
            
            // 字符集 - 使用日文片假名和一些数字增加黑客感
            const chars = "01アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲン0123456789";
            
            // 字体大小
            const fontSize = 16;
            
            // 计算列数
            const columns = Math.floor(canvas.width / fontSize);
            
            // 初始化Y坐标
            const drops = [];
            for(let i = 0; i < columns; i++) {
                drops[i] = Math.random() * -100; // 随机初始位置
            }
            
            // 绘制函数
            function draw() {
                // 半透明黑色背景 - 产生拖尾效果
                ctx.fillStyle = 'rgba(0, 0, 0, 0.05)';
                ctx.fillRect(0, 0, canvas.width, canvas.height);
                
                // 设置字体和颜色
                ctx.fillStyle = '#0f0'; // 绿色
                ctx.font = fontSize + 'px monospace';
                
                // 绘制字符
                for(let i = 0; i < drops.length; i++) {
                    const text = chars.charAt(Math.floor(Math.random() * chars.length));
                    
                    // 绘制字符
                    ctx.fillText(text, i * fontSize, drops[i] * fontSize);
                    
                    // 随机重置Y坐标
                    if(drops[i] * fontSize > canvas.height && Math.random() > 0.975) {
                        drops[i] = 0;
                    }
                    
                    // 下移Y坐标
                    drops[i]++;
                }
            }
            
            // 窗口大小调整时重置canvas
            window.addEventListener('resize', function() {
                canvas.width = window.innerWidth;
                canvas.height = window.innerHeight;
            });
            
            // 每33毫秒绘制一次 (~30fps)
            setInterval(draw, 33);
        })();

        // 导航栏滚动效果
        window.addEventListener('scroll', function() {
            const navbar = document.querySelector('.navbar');
            if (window.scrollY > 50) {
                navbar.classList.add('scrolled');
            } else {
                navbar.classList.remove('scrolled');
            }
        });

        // 平滑滚动
        document.querySelectorAll('a[href^="#"]').forEach(anchor => {
            anchor.addEventListener('click', function(e) {
                e.preventDefault();
                
                const targetId = this.getAttribute('href');
                const targetElement = document.querySelector(targetId);
                
                window.scrollTo({
                    top: targetElement.offsetTop - 80,
                    behavior: 'smooth'
                });
                
                // 更新导航栏活动状态
                document.querySelectorAll('.nav-links a').forEach(link => {
                    link.classList.remove('active');
                });
                this.classList.add('active');
            });
        });

        // 页面加载时高亮当前部分
        window.addEventListener('load', function() {
            const sections = document.querySelectorAll('section');
            const navLinks = document.querySelectorAll('.nav-links a');
            
            function highlightNav() {
                let current = '';
                
                sections.forEach(section => {
                    const sectionTop = section.offsetTop;
                    const sectionHeight = section.clientHeight;
                    
                    if (window.scrollY >= (sectionTop - 100)) {
                        current = section.getAttribute('id');
                    }
                });
                
                navLinks.forEach(link => {
                    link.classList.remove('active');
                    if (link.getAttribute('href') === `#${current}`) {
                        link.classList.add('active');
                    }
                });
            }
            
            window.addEventListener('scroll', highlightNav);
            highlightNav();
        });

        // 解码工具功能
        function decodeBase64() {
            const input = document.getElementById('base64-input').value.trim();
            try {
                const decoded = atob(input);
                document.getElementById('base64-result').innerHTML = decoded;
            } catch {
                document.getElementById('base64-result').innerHTML = "解码错误：请输入有效的Base64编码";
            }
        }

        function decodeUnicode() {
            const input = document.getElementById('unicode-input').value.trim();
            const decoded = input.replace(/\\u[\dA-Fa-f]{4}/g, match => 
                String.fromCharCode(parseInt(match.replace(/\\u/g, ''), 16))
            );
            document.getElementById('unicode-result').textContent = decoded;
        }

        function decodeCaesar() {
            const input = document.getElementById('caesar-input').value.trim();
            const shift = parseInt(document.getElementById('caesar-shift').value);
            let result = '';
            
            for (let char of input) {
                if (/[A-Z]/.test(char)) {
                    result += String.fromCharCode((char.charCodeAt(0) - 65 - shift + 26) % 26 + 65);
                } else if (/[a-z]/.test(char)) {
                    result += String.fromCharCode((char.charCodeAt(0) - 97 - shift + 26) % 26 + 97);
                } else {
                    result += char;
                }
            }
            document.getElementById('caesar-result').textContent = result;
        }

        // 解码工具模态框控制
        function showDecoderModal() {
            document.getElementById('decoder-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
        }

        function closeDecoderModal() {
            document.getElementById('decoder-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // 进制转换工具功能
        function convertFromBinary() {
            const binaryInput = document.getElementById('binary-input').value.trim();
            if (!binaryInput) {
                clearNumberInputs();
                return;
            }
            
            // 验证二进制输入
            if (!/^[01]+$/.test(binaryInput)) {
                document.getElementById('decimal-input').value = '无效二进制';
                document.getElementById('hex-input').value = '无效二进制';
                return;
            }
            
            const decimal = parseInt(binaryInput, 2);
            document.getElementById('decimal-input').value = decimal;
            document.getElementById('hex-input').value = decimal.toString(16).toUpperCase();
        }

        function convertFromDecimal() {
            const decimalInput = document.getElementById('decimal-input').value.trim();
            if (!decimalInput) {
                clearNumberInputs();
                return;
            }
            
            // 验证十进制输入
            if (!/^\d+$/.test(decimalInput)) {
                document.getElementById('binary-input').value = '无效十进制';
                document.getElementById('hex-input').value = '无效十进制';
                return;
            }
            
            const decimal = parseInt(decimalInput, 10);
            document.getElementById('binary-input').value = decimal.toString(2);
            document.getElementById('hex-input').value = decimal.toString(16).toUpperCase();
        }

        function convertFromHex() {
            const hexInput = document.getElementById('hex-input').value.trim();
            if (!hexInput) {
                clearNumberInputs();
                return;
            }
            
            // 验证十六进制输入
            if (!/^[0-9A-Fa-f]+$/.test(hexInput)) {
                document.getElementById('binary-input').value = '无效十六进制';
                document.getElementById('decimal-input').value = '无效十六进制';
                return;
            }
            
            const decimal = parseInt(hexInput, 16);
            document.getElementById('binary-input').value = decimal.toString(2);
            document.getElementById('decimal-input').value = decimal;
        }

        function clearNumberInputs() {
            document.getElementById('binary-input').value = '';
            document.getElementById('decimal-input').value = '';
            document.getElementById('hex-input').value = '';
        }

        // 进制转换工具模态框控制
        function showNumberConverterModal() {
            document.getElementById('number-converter-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            clearNumberInputs();
        }

        function closeNumberConverterModal() {
            document.getElementById('number-converter-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // 摩斯密码工具功能
        const morseCodeMap = {
            // 字母
            'A': '.-', 'B': '-...', 'C': '-.-.', 'D': '-..', 'E': '.', 'F': '..-.',
            'G': '--.', 'H': '....', 'I': '..', 'J': '.---', 'K': '-.-', 'L': '.-..',
            'M': '--', 'N': '-.', 'O': '---', 'P': '.--.', 'Q': '--.-', 'R': '.-.',
            'S': '...', 'T': '-', 'U': '..-', 'V': '...-', 'W': '.--', 'X': '-..-',
            'Y': '-.--', 'Z': '--..',
            // 数字
            '0': '-----', '1': '.----', '2': '..---', '3': '...--', '4': '....-',
            '5': '.....', '6': '-....', '7': '--...', '8': '---..', '9': '----.',
            // 标点符号
            '.': '.-.-.-', ',': '--..--', '?': '..--..', "'": '.----.', '!': '-.-.--',
            '/': '-..-.', '(': '-.--.', ')': '-.--.-', '&': '.-...', ':': '---...',
            ';': '-.-.-.', '=': '-...-', '+': '.-.-.', '-': '-....-', '_': '..--.-',
            '"': '.-..-.', '$': '...-..-', '@': '.--.-.', ' ': '/'
        };

        // 反转摩斯密码映射，用于解码
        const reverseMorseCodeMap = {};
        for (const key in morseCodeMap) {
            reverseMorseCodeMap[morseCodeMap[key]] = key;
        }

        function convertMorseCode() {
            const input = document.getElementById('morse-input').value.trim();
            const action = document.querySelector('input[name="morse-action"]:checked').value;
            let result = '';
            
            if (action === 'encode') {
                // 编码：文本 → 摩斯密码
                result = input.toUpperCase().split('').map(char => {
                    return morseCodeMap[char] || char;
                }).join(' ');
            } else {
                // 解码：摩斯密码 → 文本
                result = input.split(' ').map(code => {
                    return reverseMorseCodeMap[code] || code;
                }).join('');
            }
            
            document.getElementById('morse-result').textContent = result;
        }

        // 摩斯密码工具模态框控制
        function showMorseCodeModal() {
            document.getElementById('morse-code-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            document.getElementById('morse-input').value = '';
            document.getElementById('morse-result').textContent = '';
        }

        function closeMorseCodeModal() {
            document.getElementById('morse-code-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // GIF拆解工具功能
        function showGifSplitterModal() {
            document.getElementById('gif-splitter-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            document.getElementById('gifContainer').innerHTML = '';
            document.getElementById('gifDownloadAll').style.display = 'none';
            document.getElementById('gifProgressContainer').style.display = 'none';
        }

        function closeGifSplitterModal() {
            document.getElementById('gif-splitter-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // 端口扫描工具功能
        let scanInProgress = false;
        let scanResults = [];

        function showPortScannerModal() {
            document.getElementById('port-scanner-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            document.getElementById('scan-results-body').innerHTML = '';
            document.getElementById('export-results-btn').style.display = 'none';
            document.getElementById('scan-progress-container').style.display = 'none';
            scanResults = [];
        }

        function closePortScannerModal() {
            document.getElementById('port-scanner-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        function startPortScan() {
            const target = document.getElementById('scan-target').value.trim();
            const portRange = document.getElementById('port-range').value.trim();
            const scanType = document.getElementById('scan-type').value;
            
            if (!target) {
                alert('请输入目标主机/IP');
                return;
            }
            
            if (!portRange) {
                alert('请输入端口范围');
                return;
            }
            
            // 清空之前的结果
            document.getElementById('scan-results-body').innerHTML = '';
            document.getElementById('export-results-btn').style.display = 'none';
            scanResults = [];
            
            // 显示进度条
            document.getElementById('scan-progress-container').style.display = 'block';
            document.getElementById('scan-progress-bar').style.width = '0%';
            document.getElementById('scan-progress-bar').textContent = '0%';
            
            // 模拟扫描过程
            scanInProgress = true;
            simulatePortScan(target, portRange, scanType);
        }

        function stopPortScan() {
            scanInProgress = false;
            document.getElementById('scan-progress-bar').textContent = '已停止';
        }

        function simulatePortScan(target, portRange, scanType) {
            // 解析端口范围
            let ports = [];
            if (portRange.includes('-')) {
                // 范围格式 1-100
                const [start, end] = portRange.split('-').map(Number);
                for (let i = start; i <= end; i++) {
                    ports.push(i);
                }
            } else if (portRange.includes(',')) {
                // 逗号分隔格式 80,443,8080
                ports = portRange.split(',').map(Number);
            } else {
                // 单个端口
                ports.push(Number(portRange));
            }
            
            const totalPorts = ports.length;
            let scannedPorts = 0;
            
            // 常见端口对应的服务
            const commonServices = {
                20: 'FTP数据',
                21: 'FTP控制',
                22: 'SSH',
                23: 'Telnet',
                25: 'SMTP',
                53: 'DNS',
                80: 'HTTP',
                110: 'POP3',
                143: 'IMAP',
                443: 'HTTPS',
                3306: 'MySQL',
                3389: 'RDP',
                5432: 'PostgreSQL',
                8080: 'HTTP备用'
            };
            
            // 模拟扫描每个端口
            const scanInterval = setInterval(() => {
                if (!scanInProgress || scannedPorts >= totalPorts) {
                    clearInterval(scanInterval);
                    scanInProgress = false;
                    document.getElementById('export-results-btn').style.display = 'block';
                    document.getElementById('scan-progress-bar').textContent = '完成';
                    return;
                }
                
                const port = ports[scannedPorts];
                scannedPorts++;
                
                // 更新进度
                const progress = Math.floor((scannedPorts / totalPorts) * 100);
                document.getElementById('scan-progress-bar').style.width = progress + '%';
                document.getElementById('scan-progress-bar').textContent = progress + '%';
                
                // 模拟端口状态 (随机开放或关闭)
                const isOpen = Math.random() > 0.7; // 30%几率端口开放
                const responseTime = Math.floor(Math.random() * 100) + 1;
                const service = commonServices[port] || '未知';
                
                if (isOpen) {
                    const result = {
                        port: port,
                        status: '开放',
                        service: service,
                        responseTime: responseTime + 'ms'
                    };
                    scanResults.push(result);
                    
                    // 添加到结果表格
                    const row = document.createElement('tr');
                    row.innerHTML = `
                        <td style="padding: 8px; border-bottom: 1px solid #333;">${port}</td>
                        <td style="padding: 8px; border-bottom: 1px solid #333; color: #27ae60;">开放</td>
                        <td style="padding: 8px; border-bottom: 1px solid #333;">${service}</td>
                        <td style="padding: 8px; border-bottom: 1px solid #333;">${responseTime}ms</td>
                    `;
                    document.getElementById('scan-results-body').appendChild(row);
                }
            }, 100); // 每100ms扫描一个端口
        }

        function exportScanResults() {
            if (scanResults.length === 0) {
                alert('没有可导出的扫描结果');
                return;
            }
            
            // 创建CSV内容
            let csvContent = "端口,状态,服务,响应时间\n";
            scanResults.forEach(result => {
                csvContent += `${result.port},${result.status},${result.service},${result.responseTime}\n`;
            });
            
            // 创建下载链接
            const blob = new Blob([csvContent], { type: 'text/csv;charset=utf-8;' });
            const url = URL.createObjectURL(blob);
            const link = document.createElement('a');
            link.setAttribute('href', url);
            link.setAttribute('download', `端口扫描结果_${new Date().toISOString().slice(0,10)}.csv`);
            link.style.visibility = 'hidden';
            document.body.appendChild(link);
            link.click();
            document.body.removeChild(link);
        }

        // 二维码扫描工具功能
        function showQRScannerModal() {
            document.getElementById('qr-scanner-modal').style.display = 'block';
            document.body.style.overflow = 'hidden';
            document.getElementById('qrPreview').style.display = 'none';
            document.getElementById('qr-result').style.display = 'none';
            document.getElementById('qrFileInput').value = '';
        }

        function closeQRScannerModal() {
            document.getElementById('qr-scanner-modal').style.display = 'none';
            document.body.style.overflow = 'auto';
        }

        // 二维码扫描工具事件监听
        document.addEventListener('DOMContentLoaded', function() {
            const qrUploadArea = document.getElementById('qrUploadArea');
            const qrUploadBtn = document.getElementById('qrUploadBtn');
            const qrFileInput = document.getElementById('qrFileInput');
            const qrPreview = document.getElementById('qrPreview');
            const qrPreviewImage = document.getElementById('qrPreviewImage');
            const qrResult = document.getElementById('qr-result');
            const qrResultContent = document.getElementById('qr-result-content');
            
            // 点击上传按钮
            qrUploadBtn.addEventListener('click', function() {
                qrFileInput.click();
            });
            
            // 文件选择处理
            qrFileInput.addEventListener('change', function(e) {
                if (e.target.files.length > 0) {
                    handleQRFile(e.target.files[0]);
                }
            });
            
            // 拖放处理
            qrUploadArea.addEventListener('dragover', function(e) {
                e.preventDefault();
                qrUploadArea.classList.add('dragover');
            });
            
            qrUploadArea.addEventListener('dragleave', function() {
                qrUploadArea.classList.remove('dragover');
            });
            
            qrUploadArea.addEventListener('drop', function(e) {
                e.preventDefault();
                qrUploadArea.classList.remove('dragover');
                
                if (e.dataTransfer.files.length > 0) {
                    handleQRFile(e.dataTransfer.files[0]);
                }
            });
            
            // 处理二维码图片文件
            function handleQRFile(file) {
                if (!file.type.match('image.*')) {
                    alert('请上传图片文件');
                    return;
                }
                
                const reader = new FileReader();
                reader.onload = function(e) {
                    // 显示预览图
                    qrPreviewImage.src = e.target.result;
                    qrPreview.style.display = 'block';
                    
                    // 解码二维码
                    decodeQRCode(e.target.result);
                };
                reader.readAsDataURL(file);
            }
            
            // 解码二维码
            function decodeQRCode(imageData) {
                const img = new Image();
                img.onload = function() {
                    // 创建画布
                    const canvas = document.createElement('canvas');
                    canvas.width = img.width;
                    canvas.height = img.height;
                    const ctx = canvas.getContext('2d');
                    ctx.drawImage(img, 0, 0, canvas.width, canvas.height);
                    
                    // 获取图像数据
                    const imageData = ctx.getImageData(0, 0, canvas.width, canvas.height);
                    
                    // 使用jsQR解码
                    const code = jsQR(imageData.data, imageData.width, imageData.height, {
                        inversionAttempts: 'dontInvert',
                    });
                    
                    // 显示结果
                    if (code) {
                        qrResultContent.textContent = code.data;
                        qrResult.style.display = 'block';
                    } else {
                        qrResultContent.textContent = '未检测到二维码或解码失败';
                        qrResult.style.display = 'block';
                    }
                };
                img.src = imageData;
            }
            
            // 复制二维码结果
            window.copyQRResult = function() {
                const resultText = qrResultContent.textContent;
                navigator.clipboard.writeText(resultText).then(() => {
                    alert('已复制到剪贴板');
                }).catch(err => {
                    console.error('复制失败:', err);
                    alert('复制失败，请手动选择文本复制');
                });
            };
        });

        // GIF拆解工具事件监听
        document.addEventListener('DOMContentLoaded', function() {
            const gifUploadArea = document.getElementById('gifUploadArea');
            const gifUploadBtn = document.getElementById('gifUploadBtn');
            const gifFileInput = document.getElementById('gifFileInput');
            const gifContainer = document.getElementById('gifContainer');
            const gifDownloadAllBtn = document.getElementById('gifDownloadAll');
            const gifProgressContainer = document.getElementById('gifProgressContainer');
            const gifProgressBar = document.getElementById('gifProgressBar');
            
            // 点击上传按钮
            gifUploadBtn.addEventListener('click', function() {
                gifFileInput.click();
            });
            
            // 文件选择处理
            gifFileInput.addEventListener('change', function(e) {
                if (e.target.files.length > 0) {
                    handleGifFile(e.target.files[0]);
                }
            });
            
            // 拖放处理
            gifUploadArea.addEventListener('dragover', function(e) {
                e.preventDefault();
                gifUploadArea.classList.add('dragover');
            });
            
            gifUploadArea.addEventListener('dragleave', function() {
                gifUploadArea.classList.remove('dragover');
            });
            
            gifUploadArea.addEventListener('drop', function(e) {
                e.preventDefault();
                gifUploadArea.classList.remove('dragover');
                
                if (e.dataTransfer.files.length > 0) {
                    handleGifFile(e.dataTransfer.files[0]);
                }
            });
            
            // 处理GIF文件
            function handleGifFile(file) {
                if (!file.type.match('image/gif')) {
                    alert('请上传GIF文件');
                    return;
                }
                
                if (file.size > 10 * 1024 * 1024) {
                    alert('文件大小超过10MB限制');
                    return;
                }
                
                const reader = new FileReader();
                reader.onload = function(e) {
                    processGif(e.target.result);
                };
                reader.readAsArrayBuffer(file);
            }
            
            // 解析GIF并提取帧
            function processGif(arrayBuffer) {
                gifProgressContainer.style.display = 'block';
                gifProgressBar.style.width = '0%';
                gifProgressBar.textContent = '0%';
                
                try {
                    const gifReader = new GifReader(new Uint8Array(arrayBuffer));
                    const frames = [];
                    const width = gifReader.width;
                    const height = gifReader.height;
                    
                    // 创建画布用于渲染帧
                    const canvas = document.createElement('canvas');
                    canvas.width = width;
                    canvas.height = height;
                    const ctx = canvas.getContext('2d');
                    
                    // 创建图像数据
                    const imageData = ctx.createImageData(width, height);
                    
                    // 提取每一帧
                    const frameCount = gifReader.numFrames();
                    let framesProcessed = 0;
                    
                    for (let i = 0; i < frameCount; i++) {
                        const frameInfo = gifReader.frameInfo(i);
                        gifReader.decodeAndBlitFrameRGBA(i, imageData.data);
                        
                        // 更新画布
                        ctx.putImageData(imageData, 0, 0);
                        
                        // 将画布转换为图像URL
                        const frameUrl = canvas.toDataURL('image/png');
                        frames.push({
                            url: frameUrl,
                            delay: frameInfo.delay * 10, // 转换为毫秒
                            index: i
                        });
                        
                        // 更新进度
                        framesProcessed++;
                        const progress = Math.floor((framesProcessed / frameCount) * 100);
                        gifProgressBar.style.width = progress + '%';
                        gifProgressBar.textContent = progress + '%';
                        
                        // 显示前几帧以避免UI冻结
                        if (i < 10) {
                            displayGifFrame(frameUrl, i);
                        }
                    }
                    
                    // 处理完成后显示所有帧
                    setTimeout(() => {
                        gifContainer.innerHTML = '';
                        frames.forEach((frame, index) => {
                            displayGifFrame(frame.url, index);
                        });
                        
                        gifProgressContainer.style.display = 'none';
                        gifDownloadAllBtn.style.display = 'block';
                        
                        // 设置下载全部按钮事件
                        gifDownloadAllBtn.onclick = function() {
                            downloadAllGifFrames(frames);
                        };
                    }, 100);
                    
                } catch (error) {
                    console.error('解析GIF出错:', error);
                    alert('解析GIF文件时出错，请尝试其他GIF文件');
                    gifProgressContainer.style.display = 'none';
                }
            }
            
            // 显示单帧
            function displayGifFrame(frameUrl, index) {
                const frameDiv = document.createElement('div');
                frameDiv.className = 'gif-frame';
                
                const img = document.createElement('img');
                img.src = frameUrl;
                img.alt = `帧 ${index + 1}`;
                
                const downloadBtn = document.createElement('button');
                downloadBtn.className = 'gif-download-btn';
                downloadBtn.textContent = '下载此帧';
                downloadBtn.onclick = function() {
                    downloadGifFrame(frameUrl, index);
                };
                
                frameDiv.appendChild(img);
                frameDiv.appendChild(downloadBtn);
                gifContainer.appendChild(frameDiv);
            }
            
            // 下载单帧
            function downloadGifFrame(frameUrl, index) {
                const link = document.createElement('a');
                link.href = frameUrl;
                link.download = `gif-frame-${index + 1}.png`;
                link.click();
            }
            
            // 下载全部帧为ZIP
            function downloadAllGifFrames(frames) {
                gifProgressContainer.style.display = 'block';
                gifProgressBar.style.width = '0%';
                gifProgressBar.textContent = '准备中...';
                
                const zip = new JSZip();
                const imgFolder = zip.folder("gif-frames");
                let processed = 0;
                
                // 提取base64数据并添加到ZIP
                frames.forEach((frame, index) => {
                    const base64Data = frame.url.replace(/^data:image\/png;base64,/, "");
                    imgFolder.file(`frame-${index + 1}.png`, base64Data, {base64: true});
                    
                    processed++;
                    const progress = Math.floor((processed / frames.length) * 100);
                    gifProgressBar.style.width = progress + '%';
                    gifProgressBar.textContent = progress + '%';
                });
                
                // 生成ZIP文件
                zip.generateAsync({type: "blob"}).then(function(content) {
                    saveAs(content, "gif-frames.zip");
                    gifProgressContainer.style.display = 'none';
                });
            }
        });

        // 点击模态框外部关闭
        window.onclick = function(event) {
            if (event.target.classList.contains('modal')) {
                closeDecoderModal();
                closeNumberConverterModal();
                closeMorseCodeModal();
                closeGifSplitterModal();
                closePortScannerModal();
                closeQRScannerModal();
            }
        }

        // ESC键关闭
        document.addEventListener('keydown', (e) => {
            if (e.key === 'Escape') {
                closeDecoderModal();
                closeNumberConverterModal();
                closeMorseCodeModal();
                closeGifSplitterModal();
                closePortScannerModal();
                closeQRScannerModal();
            }
        });
    </script>
</body>
</html>
