<!DOCTYPE html>  
<html lang="id">  

<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Login</title>  
    <style>
        body {  
            font-family: Arial, sans-serif;  
            display: flex;  
            justify-content: center;  
            align-items: center;  
            height: 100vh;  
            background-color: #f4f4f4;  
        }
        .login-container {  
            background: #fff;  
            padding: 20px;  
            border-radius: 10px;  
            box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);  
            width: 300px; /* Menetapkan lebar untuk konsistensi */  
        }  
        h2 {  
            text-align: center;  
        }  
        label {  
            display: block;  
            margin: 10px 0 5px;  
        }  
        input[type="text"],  
        input[type="password"] {  
            width: 100%;  
            padding: 10px;  
            margin: 5px 0 15px;  
            border: 1px solid #ccc;  
            border-radius: 5px;  
        }  
        button {  
            width: 100%;  
            padding: 10px;  
            background-color: #5cb85c;  
            color: #fff;  
            border: none;  
            border-radius: 5px;  
            cursor: pointer;  
        }  
        button:hover {  
            background-color: #4cae4c;  
        }  
        .error-message {  
            color: red;  
            text-align: center;  
        }  
    </style>  
</head>  

<body>  
    <div class="login-container">  
        <h2>Login</h2>  
        <form id="loginForm">  
            <label for="username">Username:</label>  
            <input type="text" id="username" required>  
            <label for="password">Password:</label>  
            <input type="password" id="password" required>  
            <button type="submit">Masuk</button>  
        </form>  
        <p id="error-message" class="error-message"></p>  
    </div> 
</body> 
    <script>  
        document.getElementById('loginForm').addEventListener('submit', function(event) {  
            event.preventDefault();  
            const username = document.getElementById('username').value;  
            const password = document.getElementById('password').value;  
            // Gantilah ini dengan username dan password yang diinginkan  
            const validUsername = 'rian';  
            const validPassword = '032008';  
            if (username === validUsername && password === validPassword) {  
                // Redirect ke halaman baru  
                window.location.href = 'dasbor.html'; // Ganti dengan halaman yang ingin dituju  
            } else {  
                document.getElementById('error-message').innerText = 'Username atau password salah';  
            }  
        });  
    </script>  
 

</html>
