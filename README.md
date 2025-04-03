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

4. **Puerto en Uso**
   ```powershell
   # Si el puerto 8081 está en uso, Expo ofrecerá usar otro puerto
   npx expo start
   # O especificar un puerto diferente
   npx expo start --port 8082
   ```
