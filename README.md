<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Login Simulado BBVA</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
  <style>
    * {
      box-sizing: border-box;
    }

    body {
      margin: 0;
      font-family: 'Open Sans', sans-serif;
      background-color: #f2f2f2;
      color: #072146;
    }

    .header {
      background-color: white;
      color: #0033a0;
      padding: 20px 30px;
      text-align: left;
      font-size: 24px;
      font-weight: 600;
    }

    .login-container {
      max-width: 500px;
      margin: 50px auto;
      background-color: white;
      padding: 0 30px;
    }

    .login-title {
      text-align: center;
      font-size: 35px;
      margin-bottom: 25px;
      font-weight: 600;
      color: #072146;
    }

    label {
      display: block;
      margin-bottom: 6px;
      font-weight: 600;
      font-size: 14px;
      color: #072146;
    }

    input[type="text"],
    input[type="password"] {
      width: 100%;
      padding: 12px;
      margin-bottom: 25px;
      border: none;
      border-bottom: 1px solid #ccc;
      font-size: 16px;
      background-color: transparent;
      color: #072146;
    }

    .login-actions {
      display: flex;
      justify-content: space-between;
      align-items: center;
    }

    .forgot-password {
      background: none;
      border: none;
      color: #0033a0;
      font-size: 14px;
      cursor: pointer;
      text-decoration: none; /* 🔵 Quita subrayado */
      padding: 0;
      font-weight: 600;
    }

    .btn-login {
      padding: 10px 24px;
      background-color: #0033a0;
      color: white;
      border: none;
      border-radius: 4px;
      font-size: 16px;
      font-weight: 600;
      cursor: pointer;
    }

    .btn-login:hover {
      background-color: #002b85;
    }

    .footer {
      text-align: center;
      font-size: 12px;
      color: #6e6e6e;
      margin-top: 50px;
    }
  </style>
</head>
<body>

  <div class="header">BBVA México: Bienvenidos a la Banca en Línea</div>

  <div class="login-container">
    <div class="login-title">¡Bienvenido!</div>
    <form>
      <label for="usuario">Número de Tarjeta</label>
      <input 
        type="text" 
        id="usuario" 
        name="usuario" 
        placeholder="Número de Tarjeta" 
        pattern="\d{16}" 
        minlength="16" 
        maxlength="16" 
        title="Debe contener exactamente 16 números" 
        required>

      <label for="contrasena">Contraseña</label>
      <input 
        type="password" 
        id="contrasena" 
        name="contrasena" 
        placeholder="Ingresa tu contraseña"
        minlength="6" 
        maxlength="10" 
        required>

      <div class="login-actions">
        <button type="button" class="forgot-password">¿Olvidaste tu contraseña?</button>
        <button class="btn-login" type="submit">Entrar</button>
      </div>
    </form>
  </div>

</body>
</html>
