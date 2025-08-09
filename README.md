<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>手机模拟界面</title>
    <link rel="stylesheet" href="style.css">
</head>
<body>
    <div class="phone">
        <!-- 顶部状态栏 -->
        <div class="status-bar">
            <span>12:30</span>
            <span>📶 5G</span>
        </div>

        <!-- 主屏幕 -->
        <div class="home-screen">
            <!-- 导航栏 -->
            <div class="nav-bar">
                <button class="nav-btn active" data-tab="ai-chat">AI聊天</button>
                <button class="nav-btn" data-tab="moments">朋友圈</button>
                <button class="nav-btn" data-tab="music">一起听</button>
                <button class="nav-btn" data-tab="diary">日记</button>
                <button class="nav-btn" data-tab="meetup">面基</button>
                <button class="nav-btn" data-tab="browser">浏览器</button>
                <button class="nav-btn" data-tab="gallery">相册</button>
            </div>

            <!-- 内容区 -->
            <div class="content">
                <!-- AI聊天 -->
                <div id="ai-chat" class="tab-content active">
                    <h2>AI聊天</h2>
                    <div class="chat-box">
                        <div class="message ai-message">你好！我是AI助手，有什么可以帮你的？</div>
                        <div class="message user-message">你好！</div>
                    </div>
                    <input type="text" class="chat-input" placeholder="输入消息...">
                    <button class="send-btn">发送</button>
                </div>

                <!-- 朋友圈 -->
                <div id="moments" class="tab-content">
                    <h2>朋友圈</h2>
                    <div class="post">
                        <p>今天天气真好！🌞</p>
                        <img src="https://via.placeholder.com/150" alt="风景">
                    </div>
                </div>

                <!-- 一起听 -->
                <div id="music" class="tab-content">
                    <h2>一起听</h2>
                    <audio controls>
                        <source src="https://example.com/music.mp3" type="audio/mpeg">
                    </audio>
                </div>

                <!-- 日记 -->
                <div id="diary" class="tab-content">
                    <h2>日记</h2>
                    <textarea placeholder="写下今天的心情..."></textarea>
                    <button class="save-btn">保存</button>
                </div>

                <!-- 线下面基 -->
                <div id="meetup" class="tab-content">
                    <h2>面基</h2>
                    <p>附近的人：</p>
                    <ul class="people-list">
                        <li>张三（1km）</li>
                        <li>李四（2km）</li>
                    </ul>
                </div>

                <!-- 浏览器 -->
                <div id="browser" class="tab-content">
                    <h2>浏览器</h2>
                    <iframe src="https://www.baidu.com" width="100%" height="300"></iframe>
                </div>

                <!-- 相册 -->
                <div id="gallery" class="tab-content">
                    <h2>相册</h2>
                    <div class="photo-grid">
                        <img src="https://via.placeholder.com/100" alt="照片1">
                        <img src="https://via.placeholder.com/100" alt="照片2">
                    </div>
                </div>
            </div>
        </div>
    </div>
    <script src="script.js"></script>
</body>
</html>




<div class="phone">
  <!-- 顶部状态栏 -->
  <div class="status-bar">12:30 | 5G</div>

  <!-- 内容区 -->
  <div class="content">
    <div id="ai-chat" class="tab active">AI聊天内容</div>
    <div id="moments" class="tab">朋友圈内容</div>
    <div id="music" class="tab">一起听内容</div>
  </div>

  <!-- 底部导航栏 -->
  <div class="tab-bar">
    <button class="tab-btn active" data-tab="ai-chat">AI聊天</button>
    <button class="tab-btn" data-tab="moments">朋友圈</button>
    <button class="tab-btn" data-tab="music">一起听</button>
  </div>
</div>