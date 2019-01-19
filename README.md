# Plasma
Plasma provides an asynchronous, non-blocking (data access) Database Abstraction Layer.

Plasma does not aim to be a full Database Abstraction Layer. Simulating missing features is not a goal and should never be.

This is just a repository to concentrate general information, issues, feedback or suggestions.

The core component is living at [plasma/core](https://github.com/PlasmaPHP/core). While the drivers for the specific Database Management Systems are living in their own repositories - because they have their own specific dependencies.

Some specific packages or return types are enforced, because there's no general interface for those things. A popular example are Promises. There are ReactPHP, Amphp and Guzzle Promises.
They don't share a common interface, so it's impossible to type declare against it. As such it has been decided to settle on one implementation, as long as there is no general interface which all "major implementation packages" implement.

# Components
- [Core component](https://github.com/PlasmaPHP/core)
- [Binary Buffer component](https://github.com/PlasmaPHP/binary-buffer)
- [Schemas component](https://github.com/PlasmaPHP/schemas)
- ...more components to come


# Drivers
This is a list of all known drivers for Plasma.

- [plasma/driver-mysql](https://github.com/PlasmaPHP/driver-mysql) - A driver for MySQL/MariaDB
