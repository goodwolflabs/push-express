# Push Express 🚀🔔

**Push Express** es una herramienta que simplifica la integración de componentes de los productos de Push Protocol en proyectos web. Aunque el desarrollo comenzó con la implementación de servicios de notificaciones push, actualmente soporta una amplia gama de funcionalidades de Push Protocol. Permite agregar componentes y servicios utilizando TypeScript o JavaScript, con soporte para Yarn y NPM.

## Características

- Agrega componentes de todos los productos de Push Protocol con un solo comando.
- Compatible con TypeScript y JavaScript.
- Instala automáticamente las dependencias usando Yarn, NPM o manualmente.
- Integración sencilla con [Push Protocol](https://push.org/) para gestionar notificaciones Web3, chats, y más.

## Instalación (Opcional)

Para instalar **Push Express**, sigue estos pasos:

### Instalar con npm

```bash
npm install -g push-express
```

### Instalar con Yarn

```bash
yarn global add push-express
```

## Uso

Una vez instalado, puedes usar **Push Express** en tu proyecto para agregar componentes de los productos de Push Protocol.

### 1. Agregar un componente

Ejecuta el siguiente comando para agregar un componente:

```bash
npx push-express add [componente]
```

o

```bash
push-express add [componente]
```

> **Nota:** Reemplaza `[componente]` con el producto específico de Push Protocol que deseas integrar (por ejemplo, `notification`, `chat`, etc.).

### 2. Selecciona el tipo de archivo

Después de ejecutar el comando anterior, selecciona el tipo de archivo para tu proyecto:

- **TypeScript** (predeterminado)
- **JavaScript**

### 3. Instala las dependencias

Después de agregar el componente, **Push Express** te pedirá que elijas cómo instalar las dependencias:

- **Yarn**: Instala automáticamente las dependencias usando Yarn.
- **NPM**: Instala automáticamente las dependencias usando NPM.
- **Manual**: Mostrará el comando para instalarlas manualmente.

```bash
npm install @pushprotocol/restapi@latest ethers@^5.7
```

### 4. Inicia tu proyecto

Una vez agregado el componente e instaladas las dependencias, puedes iniciar tu proyecto:

```bash
npm run dev
```

o

```bash
yarn dev
```

## Ejemplo

Aquí tienes un ejemplo de cómo podría lucir la estructura de tu proyecto después de agregar un componente:

```bash
src/
├── components/
│   └── push-notification/
│       ├── index.ts
│       └── push-notification.tsx
└── service/
    └── push-notification/
        ├── index.ts
        └── push-notification.service.ts
```

## Contribuciones

¡Las contribuciones son bienvenidas! Si deseas contribuir a **Push Express**, sigue estos pasos:

1. Haz un fork del proyecto [https://github.com/wolfcito/push-express](https://github.com/wolfcito/push-express).
2. Crea una rama para tu funcionalidad (`git checkout -b feature/nueva-funcionalidad`).
3. Haz commit de tus cambios (`git commit -m 'Agregar nueva funcionalidad'`).
4. Haz push a la rama (`git push origin feature/nueva-funcionalidad`).
5. Abre un pull request.

> ⚠️ **Advertencia**:  
> El código en este repositorio se proporciona sin garantías. Es importante señalar que el código no ha sido auditado para detectar posibles vulnerabilidades de seguridad. Usar este código podría generar pérdida de fondos, datos comprometidos o riesgos para los activos. Procede con precaución y utiliza este código bajo tu propio riesgo. Consulta el archivo LICENSE para más detalles sobre los términos y condiciones.

## Licencia

Este proyecto está bajo la licencia MIT. Para más información, consulta el archivo [LICENSE](LICENSE).
