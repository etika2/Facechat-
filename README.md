# Facechat-
│<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Face Chat</title>
    <link rel="stylesheet" href="facechat-styles.css">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.0/css/all.min.css">
</head>
<body>
    <!-- Top Navbar -->
    <nav class="top-nav">
        <div class="nav-left">
            <div class="logo">FaceChat</div>
            <div class="search-bar">
                <i class="fas fa-search"></i>
                <input type="text" placeholder="Search FaceChat" id="search-input">
            </div>
        </div>
        <div class="nav-center">
            <a href="#" class="nav-icon active"><i class="fas fa-home"></i></a>
            <a href="#" class="nav-icon"><i class="fas fa-video"></i></a>
            <a href="#" class="nav-icon"><i class="fas fa-store"></i></a>
            <a href="#" class="nav-icon"><i class="fas fa-users"></i></a>
        </div>
        <div class="nav-right">
            <div class="nav-icon" id="messenger-btn"><i class="fas fa-comment-dots"></i></div>
            <div class="nav-icon"><i class="fas fa-bell"></i></div>
            <div class="profile-pic" id="profile-btn">
                <img src="https://via.placeholder.com/40" alt="Profile">
            </div>
            <button id="dark-toggle">🌙</button>
        </div>
    </nav>

    <div class="main-container">
        <!-- Left Sidebar -->
        <aside class="left-sidebar">
            <ul>
                <li><i class="fas fa-user"></i> John Doe</li>
                <li><i class="fas fa-users"></i> Friends</li>
                <li><i class="fas fa-clock"></i> Memories</li>
                <li><i class="fas fa-bookmark"></i> Saved</li>
                <li><i class="fas fa-flag"></i> Pages</li>
            </ul>
        </aside>

        <!-- Main Feed -->
        <main class="feed">
            <!-- Create Post -->
            <div class="create-post">
                <div class="post-header">
                    <img src="https://via.placeholder.com/40" alt="You">
                    <input type="text" placeholder="What's on your mind?" id="post-input">
                </div>
                <div class="post-actions">
                    <button onclick="createPost()"><i class="fas fa-photo-video"></i> Photo/Video</button>
                    <button><i class="fas fa-smile"></i> Feeling/Activity</button>
                </div>
            </div>

            <!-- Sample Posts -->
            <div class="post" id="post-container">
                <!-- Posts added via JS -->
            </div>
        </main>

        <!-- Right Sidebar -->
        <aside class="right-sidebar">
            <h3>Contacts</h3>
            <ul id="online-friends">
                <!-- Added via JS -->
            </ul>
            <h3>Sponsored</h3>
            <p>Ad placeholder</p>
        </aside>
    </div>

    <!-- Messenger Panel -->
    <div class="messenger-panel" id="messenger-panel">
        <div class="messenger-header">
            <h3>Chats</h3>
            <button onclick="toggleMessenger()">✕</button>
        </div>
        <div class="chat-list" id="chat-list">
            <!-- Chat previews -->
        </div>
        <div class="active-chat" id="active-chat">
            <div class="chat-header">Friend Name</div>
            <div class="messages" id="messages"></div>
            <div class="message-input">
                <input type="text" id="chat-input" placeholder="Type a message...">
                <button onclick="sendMessage()">Send</button>
            </div>
        </div>
    </div>

    <script src="facechat-script.js"></script>
</body>
</html>
├── index.html
├── package.json
├── README.md
├── .gitignore
│
├── public/
│   ├── favicon.ico
│   └── images/
│
├── src/
│   ├── index.js
│   ├── App.js
│   ├── components/
│   ├── pages/
│   ├── styles/
│   └── assets/
│
├── server/
│   ├── server.js
│   ├── routes/
│   ├── models/
│   └── controllers/
│
└── database/
    └── schema.sql
