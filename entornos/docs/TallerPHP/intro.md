# Taller PHP

[DÍA DE INTERNET Enlace](https://www.diadeinternet.org/2025/?)

# Instrucciones

## Reto 1 Preparar

![1747555648300](image/intro/1747555648300.png)

* Descarga los archivos ([enlace descarga](https://drive.google.com/file/d/1NKEyBh2ROHjg_Uj2IQ8xIRNIRs7zaCKh/view?usp=sharing))
* Ubícalos descomprimidos en **XAMPP**/**HTDOCS (C:\xampp\htdocs)**

![1747555716542](image/intro/1747555716542.png)

![1747555751929](image/intro/1747555751929.png)

IMPORTANTE! Extraer en HTDOCS

![1747556168558](image/intro/1747556168558.png)

## Reto 2 Editar

Fichero **index.php**

??? success "Código corregido"

    `<a href="actualizar_usuario.php?id=<?php echo $usuario['id']; ?>">`**Editar** `</a>`

![1747581831176](image/intro/1747581831176.png)


## Reto 3 Add user

Fichero **agregar_usuario.php**

??? success "Código corregido"

    `VALUES (:username, :password, :nombre, :email, :rol)');`


![1747582221860](image/intro/1747582221860.png)


## Reto 4 Redirigir

Fichero **agregar_usuario**.php

??? success "Código"

    `header('Location: index.php'); `




## Reto 5

Fichero **agregar_usuario.php**

??? success "Código corregido"

    `if ($result->fetchArray())`

![1747632767320](image/intro/1747632767320.png)

## Reto 6

Fichero **login.php**

??? success "Código corregido"

    `$cookie_value = "GALLETA_" . bin2hex(random_bytes(3));`

Debes salir y entrar de nuevo, si no se cambia.. ya veremos por qué.

## Reto 7

Fichero **login.php (arriba)**

??? success "Código que necesitas"

    `setcookie("galleta_inventada", "Invent"); `


Fichero **index.php (línea 60 aprox)**

??? success "Código que necesitas"

    `<p><strong>Cookie de visitante:</strong> <?php echo $_COOKIE['galleta_inventada'] ?? 'No disponible'; ?></p> `


## Reto 8

Fichero **index.php**

??? success "Código que necesitas"

    `<p><strong>VARIABLE SERVER PHP SELF:</strong> <?php echo $_SERVER['PHP_SELF']; ?></p> `

## Reto 9

Fichero **index.php**

??? success "Código que necesitas"

    ` <p><strong>Mi sesión:</strong> <?php echo htmlspecialchars($_SESSION['taller']); ?></p>`



Pero anters de lo anterior, necesitarás definir esa variable de sesión en el fichero **login.php**

??? success "Código que necesitas"

    `$_SESSION['taller'] = 'Variable sesión con cadena de texto de nuestro taller PHP'; `

## Reto 10

Fichero **logout.php**

??? success "Código corregido"

    Sólo necesitas descomentar algunos bloques de código (igual que Java /* */)


![1747634004865](image/intro/1747634004865.png)


Buen trabajo!

![1747634046473](image/intro/1747634046473.png)
