# KariPic

Blog de fotos creado en rails para el Bootcamp RoR g8.
[visitanos](https://vast-basin-97486-8e6733531a36.herokuapp.com/)

## Descripción

Esta página funciona principalmente mediante el uso de un CRUD para el manejo de los post asi como comentarios dejados por otros usuarios y su gestión a través de una base de datos, en este caso PostgreSQL. ademas y su principal novedad es el uso de aws para poder trabajar con tanto fotos de perfil y fotos en los posts, entre sus características se encuentra:

- Subir un post con una foto, titulo y leyenda para que los usuarios lo vean (solo lo administradores podrán hacer post, los usuarios pueden comentar los post).
- Editar los post y comentarios creados con un solo clic.
- Borrar un post si no te gusta su contenido o piensas que no es lo mejor lo cual borrara también los comentarios que tuviera asi como las fotos.
- Mostrar en su índice todos los post creados, mostrando siempre los últimos al comienzo.
- Muestra los comentarios de cada post.
- Ingresa con tu cuenta o crea una propia.
- Los comentarios y publicaciones solo podrán ser borradas por administradores o el mismo usuario que creo la publicación y/o comentario.
- Visitantes podrán dejar sus comentarios en las publicaciones.
- Solo los administradores y los creadores de los comentarios podrán borrar o editar comentarios dejados por visitantes.

## Importante

Solo para prueba de este proyecto se dejo la opción de crear un usuario administrador o usuario, esto debiera ser cambiado.

## Empezando 🚀

Estas instrucciones te guiarán para obtener una copia de este proyecto en funcionamiento en tu máquina local con fines de desarrollo y pruebas.

### Pre-requisitos 📋

- Sistema Operativo: Windows, Ubuntu o macOS
- Lenguaje de programación: Ruby 3.2.2
- Framework Rails: 7.0.6
- PostgreSQL: 14.8

### Instalación 🔧

Clona el repositorio con el siguiente comando:

```bash
git clone https://github.com/Delky91/KariPic
```

En la terminal, accede a la carpeta donde se encuentra el repositorio y ejecuta (recuerda que para que esto funcione, debes tener instalado Ruby y la gema bundle):

```bash
bundle install
```

Inicia la base de datos con el siguiente comando:

```bash
rails db:create db:migrate
```

Finalmente, ejecuta el proyecto con el siguiente comando y ve a la dirección IP que aparecerá en la consola:

```bash
rails s
```

## Despliegue 📦

Instrucciones para desplegar en Heroku:

asegúrate de tener instalado [Heroku](https://devcenter.heroku.com/articles/heroku-cli#install-the-heroku-cli)

1: En la terminal, inicia sesión en Heroku:

```bash
heroku login
```

2: Crea una aplicación en Heroku:

```bash
heroku create
```

- Es importante copiar el nombre de la aplicación proporcionado por Heroku, ya que se utilizará en el siguiente paso. Por ejemplo: rocky-everglades-49672.

3: Ahora conectaremos el proyecto con nuestra aplicación en Heroku:

```bash
heroku git:remote -a nombre-proyecto-dado_por_heroku
```

4: Realiza un push a Heroku:

```bash
git push heroku main
```

Importante:

Recuerda que Heroku utiliza Git, así que en tu proyecto debes haber iniciado Git. Si clonaste este repositorio, asegúrate de tener la carpeta .git; de lo contrario, realiza los siguientes pasos:

- Inicia el repositorio, agrega los cambios y realiza un primer commit:

```bash
git init
git add .
git commit -m "escribe un mensaje"
```

Si realizaste todo correctamente, ahora podrás agregar el remote mencionado en el paso 3 y seguir con el paso 4.

5a: Debes ir a la página de tu aplicación en la web de [heroku](https://id.heroku.com/login) y dirigirte a la pestaña de la derecha que dice "More":

5b: Una vez que se despliegue el menú, selecciona la opción "Run console".

6: Una vez que se despliegue la consola, asegúrate de crear la base de datos si aún no está creada y migrar los cambios:

```bash
rails db:create
rails db:migrate
rails db:seed
```

Si seguiste los pasos hasta aquí, deberías poder ver la vista index de la aplicación.

## Construido Con 🛠️

- [Ruby](https://www.ruby-lang.org/es/) - El lenguaje utilizado
- [Ruby on Rails](https://rubyonrails.org) - El framework web utilizado
- [Ruby gems](https://rubygems.org) - Gestión de dependencias
- [Postgresql](https://www.postgresql.org) - Sistema de base de datos
- [Bootstrap](https://getbootstrap.com/) - Framework de CSS
- [Devise](https://github.com/heartcombo/devise) - Gema para autentificación y permisos.
- [AWS](https://aws.amazon.com/es/) - Amazon Web Services

## Soporte

Si tienes algún problema o sugerencia, por favor abre un problema [aquí](https://github.com/Delky91/KariPic/issues).

## Versionado 📌

Use [Git](https://git-scm.com) para el versionado.

## Autores ✒️

- **Luis Miño Bustos** Encuéntrame en [github](https://github.com/Delky91)
  
