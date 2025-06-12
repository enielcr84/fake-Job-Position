<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Formulario de Oferta de Trabajo</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background-color: #f2f2f2;
      padding: 20px;
    }
    .container {
      background-color: #fff;
      max-width: 500px;
      margin: auto;
      padding: 30px;
      border-radius: 10px;
      box-shadow: 0 0 10px rgba(0,0,0,0.1);
      text-align: center;
    }
    h2 {
      text-align: center;
    }
    input[type="text"], input[type="email"] {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border-radius: 5px;
      border: 1px solid #ccc;
    }
    input[type="submit"] {
      background-color: #007BFF;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
    }
    .message {
      margin-top: 20px;
      padding: 15px;
      background-color: #ffdddd;
      border-left: 6px solid #f44336;
    }
    .logo {
      width: 150px;
      margin-bottom: 20px;
    }
  </style>
</head>
<body>
  <div class="container">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4e/Microsoft_logo.svg/512px-Microsoft_logo.svg.png" alt="Company Logo" class="logo">
    <h2>Postúlate a Nuestra Oferta</h2>
    <form onsubmit="mostrarMensaje(); return false;">
      <label>Nombre:</label>
      <input type="text" name="nombre" required>

      <label>Correo Electrónico:</label>
      <input type="email" name="correo" required>

      <label>Teléfono:</label>
      <input type="text" name="telefono" required>

      <input type="submit" value="Enviar">
    </form>

    <div id="mensaje" class="message" style="display:none;">
      <strong>¡Atención!</strong> Esta fue una simulación de ataque por código QR. Nunca escanees códigos de fuentes no verificadas. Este formulario no recopiló ninguna información.
    </div>
  </div>

  <script>
    function mostrarMensaje() {
      document.getElementById('mensaje').style.display = 'block';
    }
  </script>
</body>
</html>

