# AuthMe Configuration

A clean, customizable AuthMe configuration for PaperMC servers.

## Features

* AuthMe 6.0.0
* Argon2 password hashing
* Paper login and registration dialogs
* Async authentication tasks
* Session authentication
* Login and registration restrictions
* Inventory protection before authentication
* AntiBot protection
* Limbo player protection
* SQLite by default
* Spanish messages
* Premium account support
* Automatic database backups

## Requirements

* PaperMC
* AuthMe 6.0.0
* Minecraft 1.21.6+
* PacketEvents
* Argon2

### Argon2

This configuration uses **Argon2** for password hashing.

On Linux, the Argon2 system library must be installed before starting the server.

#### Arch Linux / CachyOS

```bash
sudo pacman -S argon2
```

> ⚠️ **Warning:** If the Argon2 library is unavailable, AuthMe may fail to initialize the configured password hashing algorithm and the server may fail to start correctly.

## Installation

1. Install PaperMC.
2. Install AuthMe and the required dependencies.
3. Install Argon2 on Linux if necessary.
4. Stop the server.
5. Replace AuthMe's `config.yml` with the configuration from this repository.
6. Start the server.

## Database

SQLite is enabled by default:

```yaml
DataSource:
    backend: SQLITE
```

MySQL/MariaDB can be enabled through AuthMe's database configuration when an external database is required.

> ℹ️ **No credentials are included with this configuration.** Database and email credentials are intentionally left empty and must be configured if you use those services.

## Compatibility

| Component | Version |
| --------- | ------- |
| AuthMe    | 6.0.0   |
| Server    | PaperMC |
| Minecraft | 1.21.6+ |

Other versions may require configuration changes.

## License

This project is licensed under the MIT License.

See [LICENSE](LICENSE) for the full license text.

---

🇪🇸 **[Leer en español →](README.es.md)**
