# Diets-plan
Special training
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <title>Admin - Recetario</title>
</head>
<body>
    <h1>Panel de Administración</h1>
    <form id="loginForm">
        <label>Usuario: <input type="text" id="username"></label><br>
        <label>Contraseña: <input type="password" id="password"></label><br>
        <button type="submit">Ingresar</button>
    </form>

    <script>
        const adminUser = "admin_william";
        const adminPass = "RecetarioFit2025!";

        document.getElementById("loginForm").addEventListener("submit", function(e) {
            e.preventDefault();
            const user = document.getElementById("username").value;
            const pass = document.getElementById("password").value;

            if (user === adminUser && pass === adminPass) {
                alert("Acceso concedido. Puedes ahora editar el contenido.");
            } else {
                alert("Credenciales incorrectas");
            }
        });
    </script>
</body>
</html>
