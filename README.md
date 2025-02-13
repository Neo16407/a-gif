<!DOCTYPE html>
<html>
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>A gift for you.</title>
<style>
body {
font-family: Arial, sans-serif;
background-image: url('https://i.pinimg.com/originals/51/0b/9e/510b9e17faac6df15673e42e534f9d57.gif');
background-size: cover;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
margin: 0;}
#login-box {
border: 2px solid #f9f5fa;
border-radius: 120px;
width: 450px;
padding: 60px;
background-color: #e7d6d6;
box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
}
input[type="text"], input[type="password"] {
width: calc(100% - 30px);
padding: 10px;
margin-top: 20px;
border: 1px solid #ddd;
border-radius: 20px;
}
button {
padding: 10px 15px;
border: none;
border-radius: 12px;
background-color: #835b8d;
color: white;
cursor: pointer;
margin-top: 20px;
width: 100%;
}
button:hover {
background-color: #4b4c6d;
padding: 10px 15px;
border: none;
border-radius: 5px;
background-color: #835b8d;
color: white;
cursor: pointer;
margin-top: 20px;
width: 100%;
}
img {
display: block;
margin-left: auto;
margin-right: auto;
width: 55%;
}
h1 {
color: #332894; 
font-family: cursive; text-align: center;
}
</style>
</head>
<body>
	<div id="login-box">
<h1 id="font-color"> Happy Valentine's Day</h1>
<script>
var colors = ["#9ac394", "#ac7778", "#94c2c3", "#8277ac", "#ac77a5"];
var currentColor = 0;
setInterval(function() {
document.getElementById("font-color").style.color = colors[currentColor];
currentColor = (currentColor + 1) % colors.length;
}, 1000);
</script>
<img src="https://i.pinimg.com/originals/60/2a/79/602a790cbc18bb037721a9d12c13b59a.gif" alt="Ảnh lỗi òi." center>
<input type="text" id="username" placeholder="Yêu em không?">
<input type="password" id="password" placeholder="Valentine được tổ chức vào ngày nào?">
<button onclick="verifyUser()">Xác minh</button>
<p id="message" style="color: red;"></p>
</div>
<script>
function verifyUser() {
const username = document.getElementById('username').value;
const password = document.getElementById('password').value;
const message = document.getElementById('message');

// Điều kiện xác minh đơn giản
if (username === 'Có' && password === '1402') {
message.style.color = 'green';
message.textContent = 'Đăng nhập thành công!';
setTimeout(() => {
window.location.href = 'm.html'; 
}, 1000);
} else {
message.style.color = 'red';
message.textContent = 'Tên đăng nhập hoặc mật khẩu sai!';
}
}
</script>
</body>
</html>
