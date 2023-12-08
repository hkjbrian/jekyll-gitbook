---
title: Contact
author: AttendSejong
date: 2023-12-08
category: Jekyll
layout: post
---

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Contact Us</title>
</head>
<body>
    <h1>Contact Us</h1>

    <form id="contactForm">
        <label for="name">이름:</label>
        <input type="text" id="name" name="name" required>

        <label for="email">이메일 주소:</label>
        <input type="email" id="email" name="email" required>

        <label for="message">메시지:</label>
        <textarea id="message" name="message" required></textarea>

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
        }
    </script>
</body>
</html>

