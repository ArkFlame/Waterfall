# ArkFlame Waterfall

ArkFlame Waterfall is an actively maintained fork of the well-known Waterfall server teleportation suite, itself a fork of BungeeCord. Led by Juan Cruz Linsalata (LinsaFTW) and developed by the ArkFlame Development team—the creators of the widely adopted FlameCord with over 10,000 downloads and 200,000 views—this project extends the end-of-life (EOL) support for Waterfall. We provide this open-source software free to the Minecraft server community, using Waterfall as the foundation for our high-performance FlameCord software.

## Key Focus Areas
ArkFlame Waterfall emphasizes three core principles:
- **Stability**: Ensuring a robust and testable codebase to minimize proxy lag and enhance reliability.
- **Features**: Extending Waterfall with additional features beyond the original BungeeCord, tailored to community needs.
- **Scalability**: Supporting large numbers of concurrent players with optimized performance on modern hardware and networks.

## Why Fork Waterfall?
ArkFlame Waterfall is a principles-driven fork aimed at sustaining and enhancing the Waterfall ecosystem. While the upstream Waterfall project has reached EOL and recommends transitioning to Velocity, ArkFlame Development continues to maintain and update this fork to serve users who rely on Waterfall's proven architecture. Unlike other projects adopting Gradle, we remain committed to Maven for its reliability and performance in our development pipeline.

Our mission is to deliver a stable, feature-rich, and scalable proxy solution, incorporating community feedback and contributions to better serve the Minecraft server ecosystem.

## How To (Server Admins)
1. Download the latest `Waterfall.jar` from our homepage: [ArkFlame Waterfall](https://arkflame.dev/waterfall).
2. Ensure your server runs **Java 8 or above**.
3. Configure and run the proxy as you would with standard Waterfall or BungeeCord setups.

### Maven Repository
```xml
<repository>
    <id>papermc</id>
    <url>https://repo.papermc.io/repository/maven-public/</url>
</repository>
```

### Maven Dependency
```xml
<dependency>
    <groupId>io.github.waterfallmc</groupId>
    <artifactId>waterfall-api</artifactId>
    <version>1.21-R0.3-SNAPSHOT</version>
    <scope>provided</scope>
</dependency>
```

### Gradle Repository
```groovy
repositories {
    maven {
        url 'https://repo.papermc.io/repository/maven-public/'
    }
}
```

### Gradle Dependency
```groovy
dependencies {
    compileOnly 'io.github.waterfallmc:waterfall-api:1.21-R0.3-SNAPSHOT'
}
```

## How To (Compiling From Source)
To compile ArkFlame Waterfall, you need:
- **JDK 8**
- **git**
- **bash**
- **Maven**
- An active internet connection

Steps:
1. Clone the repository: `git clone https://github.com/arkflame/waterfall.git`.
2. Navigate to the repository and run `./waterfall b` in a bash terminal.
3. Find the compiled jar in `Waterfall-Proxy/bootstrap/target/`.

## Join Us
We welcome contributions! Feel free to open a pull request (PR) on our [GitHub repository](https://github.com/arkflame/waterfall).  
Connect with our community:
- **Discord**: [ArkFlame Development Discord](https://discord.gg/gF36AT3)
