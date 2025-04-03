# Proyecto React Native con Expo

## Configuración del Entorno

### Requisitos Previos
- Node.js (última versión LTS)
- Git
- Expo CLI (`npm install -g expo-cli`)
- Cuenta en GitHub

### Estructura del Proyecto
```
Ultima/
├── assets/           # Recursos multimedia
├── App.js           # Componente principal
├── app.json         # Configuración de Expo
├── babel.config.js  # Configuración de Babel
├── package.json     # Dependencias y scripts
└── README.md        # Documentación
```

## Comandos PowerShell

### Inicialización del Proyecto
```powershell
# Limpiar directorio si es necesario
rm -r -force *

# Crear nuevo proyecto Expo
npx create-expo-app .
```

### Desarrollo
```powershell
# Iniciar servidor de desarrollo (COMANDO CORRECTO)
npx expo start

# Para plataformas específicas
npx expo start --android
npx expo start --ios
npx expo start --web
```

### Control de Versiones
```powershell
# Inicializar repositorio Git
git init

# Agregar archivos
git add .

# Commit inicial
git commit -m "Inicio del proyecto"

# Crear repositorio en GitHub y agregar remoto
git remote add origin [URL_DEL_REPOSITORIO]

# Subir cambios
git push -u origin main
```

## Flujo de Trabajo

1. **Desarrollo Local**
   - Realizar cambios en el código
   - Probar con `npx expo start` (COMANDO CORRECTO)
   - Verificar que todo funcione correctamente

2. **Control de Versiones**
   - Agregar cambios: `git add .`
   - Crear commit: `git commit -m "Descripción de los cambios"`
   - Subir a GitHub: `git push origin main`

3. **Nuevo Proyecto Git**
   - Crear nuevo repositorio en GitHub
   - Actualizar URL remota: `git remote set-url origin [NUEVA_URL]`
   - Subir código: `git push -u origin main`

## Notas Importantes

- Cada vez que se pruebe una funcionalidad y funcione correctamente, se debe:
  1. Hacer commit de los cambios
  2. Subir a GitHub
  3. Documentar los cambios en el README si es necesario

- Mantener el `package.json` actualizado con las dependencias necesarias

- Usar `npx expo start --clear` si hay problemas con la caché

## Solución de Problemas Comunes

1. **Error de Caché**
   ```powershell
   npx expo start --clear
   ```

2. **Reinstalar Dependencias**
   ```powershell
   rm -r -force node_modules
   npm install
   ```

3. **Limpiar Proyecto**
   ```powershell
   rm -r -force *
   npx create-expo-app .
   ```

# Welcome to your Expo app 👋

This is an [Expo](https://expo.dev) project created with [`create-expo-app`](https://www.npmjs.com/package/create-expo-app).

## Get started

1. Install dependencies

   ```bash
   npm install
   ```

2. Start the app

   ```bash
    npx expo start
   ```

In the output, you'll find options to open the app in a

- [development build](https://docs.expo.dev/develop/development-builds/introduction/)
- [Android emulator](https://docs.expo.dev/workflow/android-studio-emulator/)
- [iOS simulator](https://docs.expo.dev/workflow/ios-simulator/)
- [Expo Go](https://expo.dev/go), a limited sandbox for trying out app development with Expo

You can start developing by editing the files inside the **app** directory. This project uses [file-based routing](https://docs.expo.dev/router/introduction).

## Get a fresh project

When you're ready, run:

```bash
npm run reset-project
```

This command will move the starter code to the **app-example** directory and create a blank **app** directory where you can start developing.

## Learn more

To learn more about developing your project with Expo, look at the following resources:

- [Expo documentation](https://docs.expo.dev/): Learn fundamentals, or go into advanced topics with our [guides](https://docs.expo.dev/guides).
- [Learn Expo tutorial](https://docs.expo.dev/tutorial/introduction/): Follow a step-by-step tutorial where you'll create a project that runs on Android, iOS, and the web.

## Join the community

Join our community of developers creating universal apps.

- [Expo on GitHub](https://github.com/expo/expo): View our open source platform and contribute.
- [Discord community](https://chat.expo.dev): Chat with Expo users and ask questions.
