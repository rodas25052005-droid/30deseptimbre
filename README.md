<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Ramo Digital Hot Wheels</title>
  <style>
    /* --- ESTILOS PARA LA PANTALLA DE BIENVENIDA --- */
#welcome-screen {
    /* Ocupa toda la pantalla */
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    /* Centra el contenido */
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    /* Fondo y texto */
    background-color: #333; /* Fondo oscuro */
    color: white;
    text-align: center;
    z-index: 100; /* Asegura que esté por encima de todo */
} /* <-- ¡Esta llave de cierre faltaba en tu código! */

.greeting {
    font-size: 3em; /* Tamaño grande para el mensaje principal */
    margin-bottom: 20px;
    font-weight: bold;
}

#reveal-button {
    padding: 15px 30px;
    font-size: 1.2em;
    cursor: pointer;
    background-color: #ff4500; /* Color de botón (Naranja Hot Wheels) */
    color: white;
    border: none;
    border-radius: 8px;
    margin-top: 20px;
    transition: background-color 0.3s;
}

#reveal-button:hover {
    background-color: #e63900; /* Oscurecer al pasar el mouse */
}
/* --- FIN ESTILOS DE BIENVENIDA --- */
<style>

      margin: 0;
      padding: 0;
      display: flex;
      align-items: center;
      justify-content: center;
      height: 100vh;
      background: #111;
      color: #fff;
      overflow: hidden;
      font-family: sans-serif;
    }
    .container {
      text-align: center;
    }
    .bouquet {
      position: relative;
      width: 300px;
      height: 400px;
      margin: auto;
    }
    .car {
      position: absolute;
      width: 80px;
      opacity: 0;
      animation: float 5s infinite ease-in-out;
    }
    /* distintas posiciones iniciales */
    .car:nth-child(1) { left: 10%; animation-delay: 0s; }
    .car:nth-child(2) { left: 40%; animation-delay: 1s; }
    .car:nth-child(3) { left: 70%; animation-delay: 2s; }
    .car:nth-child(4) { left: 25%; animation-delay: 3s; }
    .car:nth-child(5) { left: 55%; animation-delay: 4s; }
    @keyframes float {
      0% { bottom: 0; opacity: 0; transform: translateY(0) scale(0.5); }
      50% { bottom: 150px; opacity: 1; transform: translateY(-30px) scale(1); }
      100% { bottom: 0; opacity: 0; transform: translateY(0) scale(0.5); }
    }
    .message {
      margin-top: 20px;
      font-size: 24px;
    }
  </style>
</head>
<body>
  <div class="container">
    <div id="welcome-screen">
        <p class="greeting">¡Feliz Día 30 de Septiembre!</p>
        <p class="greeting-message">¡Tu regalo digital está esperando! 🎉</p>
        <button id="reveal-button">Haz clic para verlo</button>
    </div>
    <div id="bouquet-content" style="display: none;"> 
        <div class="bouquet">
      <img class="car" src="https://ddkjx5kezodfx.cloudfront.net/Weyop/Libreria%20San%20Pablo/Store/Productos/SAN%20PABLO/1729524552_TUFUVEVMLS0tQXV0b3MtZGUtQ2FycmVyYS1Ib3QtV2hlZWxzLXgtMS1VbmlkYWQtLS1Db2QtNjI0Njg=.webp" alt="Hot Wheels car 1">
      <img class="car" src=https://http2.mlstatic.com/D_705680-MLA84489581853_052025-C.jpgalt="Hot Wheels car 2">
      <img class="car" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ88rj3nRDtWV89jp6ZSkpbTW1B04MDHeEuMg&usqp=CAU" alt="Hot Wheels car 3">
      <img class="car" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT0e0M_YhKViTmsq3wUmgqQvnEYcLtE2y1DeigpJgliNQ&s" alt="Hot Wheels car 4">
      <img class="car" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcSbY4PZJbOV_ckKATwY97dGQXI5y4X5KJktZ3pjwYKklA&s=10" alt="Hot Wheels car 5">
    </div>
    <div class="message">¡Un ramo Hot Wheels para vos! 🚗</div>
  <div class="message"> Te quiero muchísimo nachito🫂💘✨</div>

  <script>
    document.addEventListener('DOMContentLoaded', function() {
        
        // Obtenemos los 3 elementos clave: botón, ramo, y bienvenida
        const button = document.getElementById('reveal-button');
        const bouquet = document.getElementById('bouquet-content');
        
        // **¡AQUÍ ESTÁ LA CORRECCIÓN!**
        const welcome = document.getElementById('welcome-screen'); 

        // Escuchamos el evento de clic en el botón
        button.addEventListener('click', function() {
            // 1. Ocultamos la pantalla de bienvenida
            welcome.style.display = 'none';
            // 2. Mostramos el contenido del ramo
            bouquet.style.display = 'flex';
        });
    });
</script>

</body>
</html>
