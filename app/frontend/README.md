# Frontend

Este directorio contiene la aplicación frontend desarrollada con React Native. Aquí está la estructura de los archivos y carpetas:

- `android/`: Configuración y archivos específicos para la plataforma Android.
- `ios/`: Configuración y archivos específicos para la plataforma iOS.
- `src/`: Código fuente de la aplicación React Native.
  - `components/`: Componentes reutilizables de la interfaz de usuario.
  - `screens/`: Pantallas principales de la aplicación.
  - `navigation/`: Configuración y componentes de navegación.
  - `assets/`: Recursos estáticos como imágenes y fuentes.
  - `services/`: Servicios como llamadas a la API.
    - `api.js`: Configuración y funciones para interactuar con la API backend.
  - `redux/`: Configuración y archivos relacionados con Redux para la gestión del estado.
  - `App.js`: Componente principal de la aplicación.

## Scripts

- `start`: Inicia el servidor de desarrollo de React Native.
- `android`: Compila y ejecuta la aplicación en un dispositivo/emulador Android.
- `ios`: Compila y ejecuta la aplicación en un dispositivo/emulador iOS.
- `test`: Ejecuta las pruebas de la aplicación.

## Configuración

- `babel.config.js`: Configuración de Babel.
- `metro.config.js`: Configuración de Metro Bundler.
- `package.json`: Dependencias y scripts de npm.

## Instrucciones de Instalación

1. Instalar dependencias:
```bash
npm install
```

2. Iniciar la aplicación en modo de desarrollo:
```bash
npm start
```

3. Ejecutar en Android:
```bash
npm run android
````

4. Ejecutar en iOS:
```bash
npm run ios
```

## Estructura del proyecto

* android/: Directorio generado para la configuración específica de Android.
* ios/: Directorio generado para la configuración específica de iOS.
* src/: Contiene todo el código fuente de la aplicación.
  * components/: Aquí se encuentran los componentes reutilizables de la aplicación.
  * screens/: Las diferentes pantallas de la aplicación.
  * navigation/: Configuración y lógica de navegación entre las pantallas.
  * assets/: Archivos estáticos como imágenes, íconos, etc.
  * services/: Servicios para interactuar con APIs y otras funcionalidades.
  * redux/: Configuración y lógica de Redux para la gestión del estado global.
  * App.js: Punto de entrada de la aplicación React Native.

## Dependencias

Las principales dependencias utilizadas en este proyecto incluyen:

* react: Biblioteca principal para construir interfaces de usuario.
* react-native: Biblioteca para construir aplicaciones móviles nativas usando React.
* react-navigation: Biblioteca para gestionar la navegación en la aplicación.
* react-redux: Biblioteca para integrar Redux con React.
* redux: Biblioteca para la gestión del estado.
* axios: Cliente HTTP para realizar peticiones a la API backend.

Para ver todas las dependencias, consulta el archivo package.json.

