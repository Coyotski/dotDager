# dotDager - Portfolio Personal

Un sitio web portfolio personal desarrollado en Django, que muestra información personal, intereses y enlaces de contacto con un diseño moderno y responsivo.

## 🚀 Características

- **Diseño responsivo**: Se adapta perfectamente a dispositivos móviles y desktop
- **Animaciones**: Efectos visuales atractivos con animate.css
- **Secciones interactivas**: 
  - Perfil personal con foto
  - Sección "Sobre Mí"
  - Intereses con tarjetas interactivas
  - Enlaces de redes sociales
- **Interfaz moderna**: Gradientes, efectos hover y diseño limpio

## 🛠️ Tecnologías utilizadas

- **Backend**: Django 5.2.5
- **Frontend**: HTML5, CSS3, JavaScript
- **Iconos**: Font Awesome
- **Animaciones**: Animate.css
- **Base de datos**: SQLite (desarrollo)

## 📦 Instalación

1. **Clona el repositorio**
   ```bash
   git clone https://github.com/Coyotski/dotDager.git
   cd dotDager
   ```

2. **Crea un entorno virtual**
   ```bash
   python -m venv .venv
   ```

3. **Activa el entorno virtual**
   - Windows:
     ```bash
     .venv\Scripts\activate
     ```
   - macOS/Linux:
     ```bash
     source .venv/bin/activate
     ```

4. **Instala las dependencias**
   ```bash
   pip install django
   ```

5. **Ejecuta las migraciones**
   ```bash
   python manage.py migrate
   ```

6. **Inicia el servidor de desarrollo**
   ```bash
   python manage.py runserver
   ```

7. **Abre tu navegador** y visita `http://127.0.0.1:8000`

## 📁 Estructura del proyecto

```
dotDager/
├── manage.py
├── dotdager/
│   ├── __init__.py
│   ├── settings.py
│   ├── urls.py
│   ├── wsgi.py
│   └── portfolio/
│       ├── __init__.py
│       ├── admin.py
│       ├── apps.py
│       ├── models.py
│       ├── tests.py
│       ├── urls.py
│       ├── views.py
│       ├── migrations/
│       ├── static/
│       │   └── portfolio/
│       │       ├── styles.css
│       │       ├── profile.jpg
│       │       └── pepino.png
│       └── templates/
│           └── portfolio/
│               └── index.html
└── static/
```

## 🎨 Personalización

### Cambiar información personal
Edita el archivo `dotdager/portfolio/templates/portfolio/index.html` para actualizar:
- Nombre y descripción personal
- Intereses y hobbies
- Enlaces de redes sociales

### Modificar estilos
Los estilos se encuentran en `dotdager/portfolio/static/portfolio/styles.css`:
- Colores del tema
- Animaciones y transiciones
- Diseño responsivo

### Agregar nuevas secciones
1. Modifica `views.py` para agregar nueva lógica
2. Actualiza `index.html` con el nuevo contenido
3. Añade estilos correspondientes en `styles.css`

## 🌐 Despliegue

### GitHub Pages (100% Gratuito - Sitio Estático)

**¡Versión estática ya incluida en la carpeta `docs/`!**

1. **Ve a tu repositorio en GitHub**: https://github.com/Coyotski/dotDager
2. **Settings → Pages**
3. **Source**: Deploy from a branch
4. **Branch**: `main` 
5. **Folder**: `/docs`
6. **Save**
7. **¡Tu sitio estará disponible en**: `https://coyotski.github.io/dotDager/`

### Railway (Django Completo - También Gratuito)

1. **Ve a https://railway.app**
2. **Crea cuenta gratuita**
3. **Clic en "Start a New Project"**
4. **Selecciona "Deploy from GitHub repo"**
5. **Conecta y selecciona este repositorio**
6. **Configura variables de entorno:**
   - `SECRET_KEY`: `django-production-key-123456789`
   - `DEBUG`: `False`
7. **¡Listo! Railway desplegará automáticamente**

### Render (Django Completo)

1. **Ve a https://render.com**
2. **Crea cuenta gratuita**
3. **New → Web Service**
4. **Conecta tu repositorio GitHub**
5. **Configura:**
   - **Build Command**: `pip install -r requirements.txt`
   - **Start Command**: `python startup.py runserver 0.0.0.0:$PORT`
6. **Variables de entorno:**
   - `SECRET_KEY`: `django-production-key-123456789`
   - `DEBUG`: `False`

### Heroku (Requiere verificación de cuenta)

1. **Instala Heroku CLI** desde https://devcenter.heroku.com/articles/heroku-cli

2. **Autentícate en Heroku**
   ```bash
   heroku login
   ```

3. **Crea una aplicación**
   ```bash
   heroku create tu-nombre-app
   ```

4. **Configura variables de entorno**
   ```bash
   heroku config:set SECRET_KEY="tu-clave-secreta"
   heroku config:set DEBUG=False
   ```

5. **Despliega**
   ```bash
   git push heroku main
   ```

## 📱 Características responsivas

El sitio se adapta automáticamente a diferentes tamaños de pantalla:
- **Desktop**: Diseño completo con todas las características
- **Tablet (≤900px)**: Ajustes de padding y tamaños
- **Móvil (≤600px)**: Layout optimizado para pantallas pequeñas

## 🤝 Contribuir

1. Fork el proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.

## 👨‍💻 Autor

**Mariano Villa (DotDager)**

- YouTube: [@DotDager](https://www.youtube.com/@DotDager)
- Instagram: [@dager.32](https://www.instagram.com/dager.32/)

## 🙏 Agradecimientos

- Font Awesome por los iconos
- Animate.css por las animaciones
- La comunidad de Django por la documentación
- Mariano Villa quien solicitó este sitio como un reto

---
⭐ ¡No olvides darle una estrella al proyecto si te fue útil!
