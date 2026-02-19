# Placeholders

Placeholders are dynamic variables that can be used within Cactus Mod to display real-time information. They are formatted as `{category.name}` and are automatically replaced with the corresponding value by the `PlaceholderHandler`.

## Available Placeholders

#### 🌵 Cactus Mod

| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{cactus.version}` | Die installierte Cactus Version. | - |
| `{cactus.dev}` | Gibt an, ob es sich um einen Dev-Build handelt. | - |

#### 👤 Player
| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{player.name}` | Dein Benutzername. | - |
| `{player.health}` | Aktuelle HP. | `0` |
| `{player.max_health}` | Maximale HP. | `0` |
| `{player.hunger}` | Hunger-Level. | `0` |
| `{player.saturation}` | Sättigungs-Level. | `0` |
| `{player.xp.level}` | Aktuelles XP Level. | `0` |
| `{player.xp.progress}` | XP Fortschritt (0.0 - 1.0). | `0` |
| `{player.x}` | X-Koordinate. | `0` |
| `{player.y}` | Y-Koordinate. | `0` |
| `{player.z}` | Z-Koordinate. | `0` |
| `{player.x.opposite}` | X-Koordinate in der anderen Dimension. | `0` |
| `{player.y.opposite}` | Y-Koordinate in der anderen Dimension. | `0` |
| `{player.z.opposite}` | Z-Koordinate in der anderen Dimension. | `0` |
| `{player.chunk.x}` | Aktuelle Chunk X Position. | `0` |
| `{player.chunk.z}` | Aktuelle Chunk Z Position. | `0` |
| `{player.chunk.x.offset}` | Block-Offset innerhalb des Chunks (X). | `0` |
| `{player.chunk.z.offset}` | Block-Offset innerhalb des Chunks (Z). | `0` |
| `{player.rotation.yaw}` | Horizontale Blickrichtung. | `0` |
| `{player.rotation.pitch}` | Vertikale Blickrichtung. | `0` |
| `{player.velocity.x}` | Bewegungs-Vektor X. | `0` |
| `{player.velocity.y}` | Bewegungs-Vektor Y. | `0` |
| `{player.velocity.z}` | Bewegungs-Vektor Z. | `0` |

#### 🌍 World

| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{world.biome}` | Aktuelles Biom (formatiert). | `Unknown` |
| `{world.difficulty}` | Schwierigkeitsgrad der Welt. | - |
| `{world.weather}` | Wetterzustand (Clear, Rain, Thunderstorm). | `Clear` |
| `{world.weather.rain}` | Ob es regnet (`true`/`false`). | `false` |
| `{world.weather.thunder}` | Ob es gewittert (`true`/`false`). | `false` |
| `{world.time}` | Spielzeit als Status (Day, Noon, Night, Midnight). | - |
| `{world.day.ticks}` | Vergangene Ticks des aktuellen Tages. | - |
| `{world.time.sec}` | Weltalter in Sekunden. | `0` |
| `{world.time.min}` | Weltalter in Minuten. | `0` |
| `{world.time.hour}` | Weltalter in Stunden. | `0` |
| `{world.time.day}` | Weltalter in Tagen. | `0` |
| `{world.time.week}` | Weltalter in Wochen. | `0` |
| `{world.time.formatted}` | Lesbare Zeitangabe (z.B. `1w 2d`). | `0s` |

#### 🌐  Server

| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{server.name}` | Anzeigename des Servers oder Weltname. | - |
| `{server.address}` | Server-IP oder Weltname. | `cactusmod.xyz` |
| `{server.ping}` | Deine Latenz zum Server. | `0` |
| `{server.tps}` | Server-Performance (Ticks per Second). | `20.0` |
| `{server.brand}` | Voller Server-Brand (z.B. "Paper (Velocity)"). | `Unknown` |
| `{server.brand.short}` | Kurzer Server-Brand (z.B. "Paper"). | `Unknown` |
| `{server.packets.in}` | Durchschnittlich empfangene Pakete. | `0` |
| `{server.packets.out}` | Durchschnittlich gesendete Pakete. | `0` |

#### 🖥️  Game Performance

| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{client.fps}` | Aktuelle Bilder pro Sekunde. | `100` |
| `{client.time}` | Aktuelle Systemzeit (HH:mm:ss). | - |
| `{client.version}` | Minecraft Version des Clients. | `Unknown` |
| `{client.protocol}` | Netzwerk-Protokoll Version. | `0` |
| `{client.brand}` | Versionstyp des Clients. | `Unknown` |
| `{client.is_singleplayer}` | Ob man im Singleplayer ist. | `false` |
| `{client.render.distance}` | Eingestellte Sichtweite. | `0` |
| `{client.gui.scale}` | GUI Skalierung. | `0` |
| `{client.vsync}` | VSync Status. | `false` |
| `{client.fullscreen}` | Vollbild-Modus aktiv. | `false` |
| `{client.window.width}` | Fensterbreite in Pixeln. | `0` |
| `{client.window.height}` | Fensterhöhe in Pixeln. | `0` |
| `{input.cps.left}` | Linksklick-Rate pro Sekunde. | `0` |
| `{input.cps.right}` | Rechtsklick-Rate pro Sekunde. | `0` |

#### ☕  Hardware & JVM

| Key | Beschreibung | Fallback |
| --- | --- | --- |
| `{system.os.name}` | Name des Betriebssystems. | `Unknown` |
| `{system.os.arch}` | OS Architektur (z.B. x64). | `Unknown` |
| `{system.os.version}` | OS Version. | `Unknown` |
| `{system.user.name}` | Benutzername im Betriebssystem. | `Unknown` |
| `{system.user.home}` | Pfad zum Home-Verzeichnis. | `Unknown` |
| `{system.cpu.cores}` | Verfügbare CPU-Kerne. | `0` |
| `{system.memory.total.mb}` | Gesamter reservierter RAM. | `0` |
| `{system.memory.free.mb}` | Freier RAM im JVM Heap. | `0` |
| `{system.memory.used.mb}` | Aktuell genutzter RAM. | `0` |
| `{system.memory.max.mb}` | Maximaler RAM für die JVM. | `0` |
| `{java.version}` | Installierte Java Version. | `Unknown` |
| `{jvm.name}` | Name der Java VM. | `Unknown` |
| `{jvm.vendor}` | Entwickler der Java VM. | `Unknown` |
| `{jvm.version}` | Version der Java VM. | `Unknown` |
| `{jvm.uptime.ms}` | Laufzeit der Java Instanz (ms). | `0` |
| `{jvm.threads.count}` | Anzahl aktiver Threads. | `0` |
| `{jvm.threads.daemon}` | Anzahl aktiver Daemon-Threads. | `0` |
| `{jvm.gc.count}` | Anzahl der Garbage Collections. | `0` |
| `{jvm.gc.time.ms}` | Zeitaufwand für GC (ms). | `0` |

## How it works

The `PlaceholderHandler` manages two types of values:

### 📥 Static Placeholders

These are hardcoded in the client (as seen in the list above). They are updated every frame or whenever the value is requested. If a value cannot be found (e.g., you are not in a world), a **fallback** value (like `0` or `Unknown`) is displayed.

### 🔄 Dynamic Placeholders

These can be registered by Addons or received from external sources. They use an `Identifier` and can be bound to a specific "Required State" to ensure they only show up when relevant.

> **Tip:** You can use these placeholders in most text-based modules, such as the Custom HUD or Macros!
