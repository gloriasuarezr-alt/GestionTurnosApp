# GestionTurnosApp 📅

Aplicación móvil Android para gestión eficiente de turnos laborales. Permite crear, editar, eliminar y visualizar turnos de empleados de forma sencilla.

## 📋 Características

- ✅ Crear y eliminar turnos
- ✅ Asignar turnos a empleados
- ✅ Visualizar turnos por fecha
- ✅ Base de datos local con SQLite
- ✅ Interfaz intuitiva y responsive
- ✅ Persistencia de datos

## 🛠️ Tecnologías

- **Android Studio** (IDE)
- **Kotlin** (Lenguaje principal)
- **SQLite** (Base de datos local)
- **Material Design 3** (UI)
- **MVVM Architecture** (Patrón arquitectónico)

## 📱 Requisitos

- Android Studio 2023.1 o superior
- JDK 11 o superior
- Android SDK (API 24+)
- Gradle 8.0+

## 🚀 Instalación

1. **Clonar el repositorio**
```bash
git clone https://github.com/gloriasuarezr-alt/GestionTurnosApp.git
cd GestionTurnosApp
```

2. **Abrir en Android Studio**
   - Abre Android Studio
   - File → Open → Selecciona la carpeta del proyecto
   - Espera a que Gradle termine de sincronizar

3. **Compilar y ejecutar**
   - Conecta un dispositivo Android o usa el emulador
   - Presiona `Shift + F10` o Click en ▶️ Run

## 📁 Estructura del Proyecto

```
GestionTurnosApp/
├── app/
│   ├── src/
│   │   ├── main/
│   │   │   ├── java/com/gestionturnos/
│   │   │   │   ├── MainActivity.kt
│   │   │   │   ├── db/
│   │   │   │   │   ├── TurnoDatabase.kt
│   │   │   │   │   └── TurnoDao.kt
│   │   │   │   ├── models/
│   │   │   │   │   └── Turno.kt
│   │   │   │   └── ui/
│   │   │   │       ├── TurnosListFragment.kt
│   │   │   │       └── CrearTurnoFragment.kt
│   │   │   ├── res/
│   │   │   │   ├── layout/
│   │   │   │   │   ├── activity_main.xml
│   │   │   │   │   └── fragment_turnos.xml
│   │   │   │   └── values/
│   │   │   └── AndroidManifest.xml
│   │   └── build.gradle
│   └── proguard-rules.pro
├── gradle/
├── .gitignore
├── build.gradle
├── settings.gradle
└── README.md
```

## 🗄️ Modelo de Datos

### Tabla: Turnos
| Campo | Tipo | Descripción |
|-------|------|-------------|
| id | INTEGER (PK) | Identificador único |
| empleado | TEXT | Nombre del empleado |
| fecha | TEXT | Fecha del turno (yyyy-MM-dd) |
| horaInicio | TEXT | Hora de inicio (HH:mm) |
| horaFin | TEXT | Hora de fin (HH:mm) |
| tipo | TEXT | Tipo de turno (Mañana/Tarde/Noche) |
| createdAt | LONG | Timestamp de creación |

## 💡 Uso

1. **Crear un turno:**
   - Presiona el botón "+" en la pantalla principal
   - Completa los datos del turno
   - Presiona "Guardar"

2. **Ver turnos:**
   - Los turnos se muestran en una lista
   - Haz clic en uno para ver detalles

3. **Eliminar un turno:**
   - Desliza hacia la izquierda sobre un turno
   - Confirma la eliminación

## 📝 Ejemplo de Código

```kotlin
// Crear un turno
val turno = Turno(
    empleado = "Juan Pérez",
    fecha = "2026-05-20",
    horaInicio = "08:00",
    horaFin = "16:00",
    tipo = "Mañana"
)
viewModel.crearTurno(turno)
```

## 🐛 Debugging

- **Logs**: Usa Logcat en Android Studio (View → Tool Windows → Logcat)
- **Database Inspector**: Tools → App Inspection → Database Inspector
- **Emulator**: Abre el emulador desde AVD Manager

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:

1. Crea un fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

## 📄 Licencia

Este proyecto está bajo la licencia MIT - ver el archivo LICENSE para más detalles.

## 👤 Autor

**Gloria Suárez** 
- GitHub: [@gloriasuarezr-alt](https://github.com/gloriasuarezr-alt)

## 📞 Soporte

¿Problemas? Abre un issue en GitHub o contacta directamente.

---

**¡Disfruta gestionando tus turnos de forma eficiente!** 🎉
