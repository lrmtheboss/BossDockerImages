# BossDockerImages

Docker images for various uses.

## Images

### [Installers](/installers)

Installers images for use with pterodactyl panel when installing a server.

* [alpine](/installers/alpine)
  * `ghcr.io/lrmtheboss/bossdockerimages:installers_alpine`
* [debian](/installers/debian)
  * `ghcr.io/lrmtheboss/bossdockerimages:installers_debian`
* [ubuntu](/installers/ubuntu)
  * `ghcr.io/lrmtheboss/bossdockerimages:installers_ubuntu`

### [Java](/java)

Java images for pterodactyl panel.

Recommend order in pterodactyl egg configuration:

```txt
Java 25|ghcr.io/lrmtheboss/bossdockerimages:java_25
Java 21|ghcr.io/lrmtheboss/bossdockerimages:java_21
Java 17|ghcr.io/lrmtheboss/bossdockerimages:java_17
Java 11|ghcr.io/lrmtheboss/bossdockerimages:java_11
Java 8|ghcr.io/lrmtheboss/bossdockerimages:java_8
```

### [MariaDB](/mariadb)

MariaDB images for pterodactyl panel.

* [10.6](/mariadb/10.6)
  * `ghcr.io/lrmtheboss/bossdockerimages:mariadb_10.6`
* [11.4](/mariadb/11.4)
  * `ghcr.io/lrmtheboss/bossdockerimages:mariadb_11.4`
* [11.8](/mariadb/11.8)
  * `ghcr.io/lrmtheboss/bossdockerimages:mariadb_11.8`

### [MongoDB](/mongodb)

MongoDB images for pterodactyl panel.

* [7](/mongodb/7)
  * `ghcr.io/lrmtheboss/bossdockerimages:mongodb_7`
* [8](/mongodb/8)
  * `ghcr.io/lrmtheboss/bossdockerimages:mongodb_8`

### [NodeJS](/nodejs)

NodeJS images for pterodactyl panel.

* [22](/nodejs/22)
  * `ghcr.io/lrmtheboss/bossdockerimages:nodejs_22`
* [24](/nodejs/24)
  * `ghcr.io/lrmtheboss/bossdockerimages:nodejs_24`

### [OSes](/oses)

OSes images for pterodactyl panel.

* [alpine](/oses/alpine)
  * `ghcr.io/lrmtheboss/bossdockerimages:oses_alpine`
* [debian](/oses/debian)
  * `ghcr.io/lrmtheboss/bossdockerimages:oses_debian`
* [ubuntu](/oses/ubuntu)
  * `ghcr.io/lrmtheboss/bossdockerimages:oses_ubuntu`

### [Postgres](/postgres)

Postgres images for pterodactyl panel.

* [15](/postgres/15)
  * `ghcr.io/lrmtheboss/bossdockerimages:postgres_15`
* [16](/postgres/16)
  * `ghcr.io/lrmtheboss/bossdockerimages:postgres_16`
* [17](/postgres/17)
  * `ghcr.io/lrmtheboss/bossdockerimages:postgres_17`
* [18](/postgres/18)
  * `ghcr.io/lrmtheboss/bossdockerimages:postgres_18`

### [Redis](/redis)

Redis images for pterodactyl panel.

* [8](/redis/8)
  * `ghcr.io/lrmtheboss/bossdockerimages:redis_8`
