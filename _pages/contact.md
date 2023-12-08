---
title: Contact
author: AttendSejong
date: 2023-12-08
category: Jekyll
layout: post
---

<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
    <style>
        /* 추가된 CSS 스타일 */
        form {
            display: flex;
            flex-direction: column;
            max-width: 300px;
            margin: auto;
        }

        label {
            margin-bottom: 8px;
        }

        input, textarea {
            margin-bottom: 16px;
            width: 100%;
        }

        button {
            margin-top: 8px;
        }
    </style>
</head>
<body>

    <form id="contactForm">
        <label for="name">Name:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">email address:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">message:</label>
        <textarea id="message" name="message" required rows="5"></textarea>

        <button type="button" onclick="sendEmail()">Send</button>
    </form>

    <script>
        function sendEmail() {
            var name = document.getElementById('name').value;
            var email = document.getElementById('email').value;
            var message = document.getElementById('message').value;

            // 여기에 실제로 이메일을 보내는 로직을 추가해야 합니다.
            // 이 예제에서는 간단히 브라우저 콘솔에 출력합니다.
            console.log('Name: ' + name);
            console.log('Email: ' + email);
            console.log('Message: ' + message);

            // 알림창 띄우기
            alert('확인되었습니다.');

            // 입력 내용 초기화
            document.getElementById('name').value = '';
            document.getElementById('email').value = '';
            document.getElementById('message').value = '';
        }
    </script>
</body>
</html>

