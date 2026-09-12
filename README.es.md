# Configuración de AuthMe

Una configuración limpia y personalizable de AuthMe para servidores PaperMC.

## Características

* AuthMe 6.0.0
* Hashing de contraseñas mediante Argon2
* Diálogos de inicio de sesión y registro de Paper
* Tareas de autenticación asíncronas
* Autenticación mediante sesiones
* Restricciones de inicio de sesión y registro
* Protección del inventario antes de autenticarse
* Protección AntiBot
* Protección de jugadores mediante Limbo
* SQLite como backend predeterminado
* Mensajes en español
* Soporte para cuentas premium
* Copias de seguridad automáticas

## Requisitos

* PaperMC
* AuthMe 6.0.0
* Minecraft 1.21.6+
* PacketEvents
* Argon2

### Argon2

Esta configuración utiliza **Argon2** para el hashing de contraseñas.

En Linux, la biblioteca de Argon2 del sistema debe estar instalada antes de iniciar el servidor.

```bash
sudo <tu-gestor-de-paquetes> install argon2
```

> ⚠️ **Advertencia:** Si la biblioteca de Argon2 no está disponible, AuthMe puede no ser capaz de inicializar el algoritmo de hashing configurado y el servidor podría no iniciar correctamente.

## Instalación

1. Instala PaperMC.
2. Instala AuthMe y las dependencias necesarias.
3. Instala Argon2 en Linux si es necesario.
4. Detén el servidor.
5. Reemplaza el `config.yml` de AuthMe por el incluido en este repositorio.
6. Inicia el servidor.

## Base de datos

SQLite está hablitado de forma predeterminada:

```yaml
DataSource:
    backend: SQLITE
```

MySQL/MariaDB puede habilitarse mediante la configuración de base de datos de AuthMe cuando se necesite una base de datos externa.

> ℹ️ **Esta configuración no incluye credenciales.** Las credenciales de base de datos y correo electrónico se dejan vacías intencionalmente y deben configurarse si utilizas esos servicios.

## Compatibilidad

| Componente | Versión |
| ---------- | ------- |
| AuthMe     | 6.0.0   |
| Servidor   | PaperMC |
| Minecraft  | 1.21.6+ |

Otras versiones pueden requerir modificaciones en la configuración.

## Licencia

Este proyecto está bajo la licencia MIT.

Consulta [LICENSE](LICENSE) para ver el texto completo de la licencia.

---

🇺🇸 **[Read in English →](README.en.md)**
