<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Teachers' Day Messages</title>
    <style>
        body {
            box-sizing: border-box;
            font-family: 'Georgia', serif;
            background: linear-gradient(135deg, #2c3e50 0%, #34495e 100%);
            color: #ecf0f1;
            margin: 0;
            padding: 20px;
            min-height: 100vh;
        }

        .container {
            max-width: 800px;
            margin: 0 auto;
            background: rgba(52, 73, 94, 0.9);
            border-radius: 20px;
            padding: 40px;
            box-shadow: 0 20px 40px rgba(0, 0, 0, 0.3);
            backdrop-filter: blur(10px);
        }

        .header {
            text-align: center;
            margin-bottom: 40px;
        }

        .header h1 {
            font-size: 2.5rem;
            margin: 0;
            color: #bdc3c7;
            text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.5);
        }

        .header .apple {
            font-size: 3rem;
            margin: 10px 0;
            display: block;
        }

        .header p {
            font-size: 1.1rem;
            color: #95a5a6;
            margin: 10px 0 0 0;
            font-style: italic;
        }

        .message-form {
            background: rgba(44, 62, 80, 0.6);
            padding: 30px;
            border-radius: 15px;
            margin-bottom: 30px;
            border: 2px solid rgba(189, 195, 199, 0.2);
        }

        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: bold;
            color: #bdc3c7;
        }

        input[type="text"], textarea {
            width: 100%;
            padding: 15px;
            border: 2px solid rgba(189, 195, 199, 0.3);
            border-radius: 10px;
            background: rgba(236, 240, 241, 0.1);
            color: #ecf0f1;
            font-size: 1rem;
            font-family: inherit;
            transition: all 0.3s ease;
        }

        input[type="text"]:focus, textarea:focus {
            outline: none;
            border-color: #95a5a6;
            background: rgba(236, 240, 241, 0.15);
            box-shadow: 0 0 10px rgba(149, 165, 166, 0.3);
        }

        textarea {
            resize: vertical;
            min-height: 120px;
        }

        .btn {
            background: linear-gradient(45deg, #7f8c8d, #95a5a6);
            color: #2c3e50;
            border: none;
            padding: 15px 30px;
            border-radius: 25px;
            font-size: 1.1rem;
            font-weight: bold;
            cursor: pointer;
            transition: all 0.3s ease;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .btn:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.3);
            background: linear-gradient(45deg, #95a5a6, #bdc3c7);
        }

        .btn:active {
            transform: translateY(0);
        }

        .messages-section {
            margin-top: 40px;
        }

        .messages-header {
            display: flex;
            align-items: center;
            justify-content: space-between;
            margin-bottom: 20px;
        }

        .messages-header h2 {
            color: #bdc3c7;
            margin: 0;
            font-size: 1.8rem;
        }

        .message-count {
            background: rgba(149, 165, 166, 0.2);
            padding: 8px 16px;
            border-radius: 20px;
            font-size: 0.9rem;
            color: #95a5a6;
        }

        .messages-container {
            display: none;
            animation: fadeIn 0.5s ease-in;
        }

        .messages-container.show {
            display: block;
        }

        @keyframes fadeIn {
            from { opacity: 0; transform: translateY(20px); }
            to { opacity: 1; transform: translateY(0); }
        }

        .message-card {
            background: rgba(44, 62, 80, 0.4);
            border: 1px solid rgba(189, 195, 199, 0.2);
            border-radius: 12px;
            padding: 20px;
            margin-bottom: 15px;
            transition: all 0.3s ease;
        }

        .message-card:hover {
            transform: translateX(5px);
            border-color: rgba(189, 195, 199, 0.4);
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
        }

        .message-header {
            display: flex;
            justify-content: space-between;
            align-items: center;
            margin-bottom: 10px;
        }

        .teacher-name {
            font-weight: bold;
            color: #bdc3c7;
            font-size: 1.1rem;
        }

        .message-date {
            font-size: 0.8rem;
            color: #7f8c8d;
        }

        .message-text {
            color: #ecf0f1;
            line-height: 1.6;
            font-style: italic;
        }

        .empty-state {
            text-align: center;
            padding: 40px;
            color: #7f8c8d;
        }

        .empty-state .book {
            font-size: 4rem;
            margin-bottom: 20px;
            display: block;
        }

        .decorative-line {
            height: 2px;
            background: linear-gradient(90deg, transparent, #7f8c8d, transparent);
            margin: 30px 0;
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="header">
            <span class="apple">🍎</span>
            <h1>Teachers' Day Messages</h1>
            <p>Add your long sweet message</p>
        </div>

        <div class="decorative-line"></div>

        <form class="message-form" id="messageForm">
            <div class="form-group">
                <label for="teacherName">Teacher's Name</label>
                <input type="text" id="teacherName" placeholder="Enter your teacher's name" required>
            </div>
            
            <div class="form-group">
                <label for="message">Your Message</label>
                <textarea id="message" placeholder="Write your heartfelt message here..." required></textarea>
            </div>
            
            <button type="submit" class="btn">📝 Add Message</button>
        </form>

        <div class="messages-section">
            <div class="messages-header">
                <h2>💌 Saved Messages</h2>
                <span class="message-count" id="messageCount">0 messages</span>
            </div>
            
            <button type="button" class="btn" id="viewMessagesBtn" onclick="toggleMessages()">
                👀 View All Messages
            </button>

            <div class="messages-container" id="messagesContainer">
                <div class="empty-state" id="emptyState">
                    <span class="book">📚</span>
                    <p>No messages yet. Start by writing your first heartfelt message!</p>
                </div>
                <div id="messagesList"></div>
            </div>
        </div>
    </div>

    <script>
        let messages = [];
        let messagesVisible = false;

        document.getElementById('messageForm').addEventListener('submit', function(e) {
            e.preventDefault();
            
            const teacherName = document.getElementById('teacherName').value.trim();
            const messageText = document.getElementById('message').value.trim();
            
            if (teacherName && messageText) {
                const newMessage = {
                    id: Date.now(),
                    teacherName: teacherName,
                    message: messageText,
                    date: new Date().toLocaleDateString('en-US', { 
                        year: 'numeric', 
                        month: 'short', 
                        day: 'numeric' 
                    })
                };
                
                messages.push(newMessage);
                updateMessageCount();
                
                // Clear form
                document.getElementById('teacherName').value = '';
                document.getElementById('message').value = '';
                
                // Show success feedback
                const btn = document.querySelector('button[type="submit"]');
                const originalText = btn.innerHTML;
                btn.innerHTML = '✅ Message Added!';
                btn.style.background = 'linear-gradient(45deg, #27ae60, #2ecc71)';
                
                setTimeout(() => {
                    btn.innerHTML = originalText;
                    btn.style.background = 'linear-gradient(45deg, #7f8c8d, #95a5a6)';
                }, 2000);
                
                // If messages are currently visible, refresh the display
                if (messagesVisible) {
                    displayMessages();
                }
            }
        });

        function toggleMessages() {
            const container = document.getElementById('messagesContainer');
            const btn = document.getElementById('viewMessagesBtn');
            
            messagesVisible = !messagesVisible;
            
            if (messagesVisible) {
                container.classList.add('show');
                btn.innerHTML = '🙈 Hide Messages';
                displayMessages();
            } else {
                container.classList.remove('show');
                btn.innerHTML = '👀 View All Messages';
            }
        }

        function displayMessages() {
            const messagesList = document.getElementById('messagesList');
            const emptyState = document.getElementById('emptyState');
            
            if (messages.length === 0) {
                emptyState.style.display = 'block';
                messagesList.innerHTML = '';
            } else {
                emptyState.style.display = 'none';
                messagesList.innerHTML = messages.map(msg => `
                    <div class="message-card">
                        <div class="message-header">
                            <span class="teacher-name">👩‍🏫 ${msg.teacherName}</span>
                            <span class="message-date">${msg.date}</span>
                        </div>
                        <div class="message-text">"${msg.message}"</div>
                    </div>
                `).join('');
            }
        }

        function updateMessageCount() {
            const count = messages.length;
            const countElement = document.getElementById('messageCount');
            countElement.textContent = ${count} message${count !== 1 ? 's' : ''};
        }
    </script>
<script>(function(){function c(){var b=a.contentDocument||a.contentWindow.document;if(b){var d=b.createElement('script');d.innerHTML="window.__CF$cv$params={r:'988b217ab755fee5',t:'MTc1OTQ4MDc4NS4wMDAwMDA='};var a=document.createElement('script');a.nonce='';a.src='/cdn-cgi/challenge-platform/scripts/jsd/main.js';document.getElementsByTagName('head')[0].appendChild(a);";b.getElementsByTagName('head')[0].appendChild(d)}}if(document.body){var a=document.createElement('iframe');a.height=1;a.width=1;a.style.position='absolute';a.style.top=0;a.style.left=0;a.style.border='none';a.style.visibility='hidden';document.body.appendChild(a);if('loading'!==document.readyState)c();else if(window.addEventListener)document.addEventListener('DOMContentLoaded',c);else{var e=document.onreadystatechange||function(){};document.onreadystatechange=function(b){e(b);'loading'!==document.readyState&&(document.onreadystatechange=e,c())}}}})();</script></body>
</html>
