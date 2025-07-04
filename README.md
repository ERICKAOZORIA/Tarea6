# 🧰 Caja de Herramientas - Flutter App

Una aplicación Flutter multifuncional que incluye diversas herramientas útiles y APIs integradas.

## 📱 Características

### 🏠 Pantalla Principal
- Interfaz atractiva con imagen de caja de herramientas
- Navegación intuitiva a todas las funcionalidades
- Diseño moderno con gradientes y tarjetas

### 🔮 Predictor de Género
- **API**: [Genderize.io](https://api.genderize.io)
- Predice el género basado en el nombre
- Muestra probabilidad y número de muestras
- Interfaz visual con colores azul (masculino) y rosa (femenino)

### 🎂 Predictor de Edad
- **API**: [Agify.io](https://api.agify.io)
- Predice la edad basada en el nombre
- Categoriza en: Joven (<18), Adulto (18-59), Anciano (60+)
- Muestra iconos y colores representativos para cada categoría

### 🎓 Búsqueda de Universidades
- **API**: [Universities API](http://universities.hipolabs.com)
- Busca universidades por país (en inglés)
- Muestra nombre, dominio y enlace web
- Enlaces clicables para visitar sitios web

### 🌤️ Clima de República Dominicana
- **API**: [OpenWeatherMap](https://openweathermap.org)
- Muestra el clima actual de RD
- Información de temperatura, humedad y viento
- Iconos meteorológicos dinámicos

### 🐾 Información de Pokémon
- **API**: [PokéAPI](https://pokeapi.co)
- Busca Pokémon por nombre
- Muestra imagen, experiencia base, altura, peso y habilidades
- Reproduce el sonido del Pokémon

### 📰 Noticias de WordPress
- **API**: WordPress REST API (Kinsta Blog)
- Muestra las últimas 3 noticias
- Enlaces directos a artículos originales
- Logo de WordPress integrado

### 👨‍💻 Acerca de
- Información del desarrollador
- Datos de contacto para oportunidades laborales
- Habilidades técnicas
- Enlaces a redes sociales

## 🛠️ Tecnologías Utilizadas

- **Flutter**: Framework principal
- **Dart**: Lenguaje de programación
- **HTTP**: Llamadas a APIs REST
- **Cached Network Image**: Carga de imágenes optimizada
- **URL Launcher**: Apertura de enlaces externos
- **AudioPlayers**: Reproducción de sonidos de Pokémon
- **Font Awesome Flutter**: Iconos modernos

## 📦 Dependencias

```yaml
dependencies:
  flutter:
    sdk: flutter
  cupertino_icons: ^1.0.8
  http: ^1.1.0
  json_annotation: ^4.8.1
  url_launcher: ^6.2.2
  audioplayers: ^5.2.1
  cached_network_image: ^3.3.0
  font_awesome_flutter: ^10.6.0
```

## 🚀 Instalación y Ejecución

1. **Clona el repositorio**
   ```bash
   git clone [URL_DEL_REPOSITORIO]
   cd toolbox_app
   ```

2. **Instala las dependencias**
   ```bash
   flutter pub get
   ```

3. **Configura las APIs**
   - Para el clima: Obtén una API key gratuita de [OpenWeatherMap](https://openweathermap.org/api)
   - Edita `lib/services/api_service.dart` y reemplaza `TU_API_KEY_AQUI` con tu API key

4. **Ejecuta la aplicación**
   ```bash
   flutter run
   ```

## 📁 Estructura del Proyecto

```
lib/
├── main.dart                 # Punto de entrada de la aplicación
├── models/                   # Modelos de datos
│   ├── age_model.dart
│   ├── gender_model.dart
│   ├── news_model.dart
│   ├── pokemon_model.dart
│   ├── university_model.dart
│   └── weather_model.dart
├── screens/                  # Pantallas de la aplicación
│   ├── about_screen.dart
│   ├── age_prediction_screen.dart
│   ├── gender_prediction_screen.dart
│   ├── home_screen.dart
│   ├── news_screen.dart
│   ├── pokemon_screen.dart
│   ├── universities_screen.dart
│   └── weather_screen.dart
└── services/                 # Servicios para APIs
    └── api_service.dart
```

## 🎨 Personalización

### Cambiar información personal en "Acerca de"
Edita `lib/screens/about_screen.dart`:
- Reemplaza "Tu Nombre Aquí" con tu nombre
- Actualiza la información de contacto
- Modifica las habilidades técnicas

### Agregar tu foto como icono
1. Guarda tu foto en `assets/icons/app_icon.png`
2. Configura el icono en `android/app/src/main/res/` para Android
3. Configura el icono en `ios/Runner/Assets.xcassets/` para iOS

### Cambiar página de noticias
En `lib/services/api_service.dart`, modifica la constante `wordpressApiUrl` con la URL de tu página WordPress preferida.

## 🌐 APIs Utilizadas

| API | Propósito | Documentación |
|-----|-----------|---------------|
| Genderize.io | Predicción de género | [https://genderize.io](https://genderize.io) |
| Agify.io | Predicción de edad | [https://agify.io](https://agify.io) |
| Universities API | Búsqueda de universidades | [http://universities.hipolabs.com](http://universities.hipolabs.com) |
| OpenWeatherMap | Información del clima | [https://openweathermap.org/api](https://openweathermap.org/api) |
| PokéAPI | Datos de Pokémon | [https://pokeapi.co](https://pokeapi.co) |
| WordPress REST API | Noticias de blogs | [https://developer.wordpress.org/rest-api/](https://developer.wordpress.org/rest-api/) |

## 📱 Capturas de Pantalla

> **Nota**: Agrega capturas de pantalla de tu aplicación en funcionamiento

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Fork el repositorio
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la Licencia MIT - ver el archivo [LICENSE](LICENSE) para más detalles.

## 👨‍💻 Desarrollador

**[Tu Nombre]**
- 📧 Email: [tuemail@ejemplo.com]
- 💼 LinkedIn: [linkedin.com/in/tuperfil]
- 🐙 GitHub: [github.com/tuusuario]

---

⚡ **Desarrollado con Flutter 💙**
