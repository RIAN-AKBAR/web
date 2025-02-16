<!DOCTYPE html>  
<html lang="id">  

<head>  
    <meta charset="UTF-8">  
    <meta name="viewport" content="width=device-width, initial-scale=1.0">  
    <title>Login</title> 
    <link rel="stylesheet" href="styles.css">  
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
