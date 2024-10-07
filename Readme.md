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

### Java

Java images for pterodactyl panel.

Recommend order in pterodactyl egg configuration:
```txt
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

### [MongoDB](/mongodb)

MongoDB images for pterodactyl panel.

* [7](/mongodb/7)
    * `ghcr.io/lrmtheboss/bossdockerimages:mongodb_7`
* [8](/mongodb/8)
    * `ghcr.io/lrmtheboss/bossdockerimages:mongodb_8`

### [NodeJS](/nodejs)

NodeJS images for pterodactyl panel.

* [18](/nodejs/18)
    * `ghcr.io/lrmtheboss/bossdockerimages:nodejs_18`
* [20](/nodejs/20)
    * `ghcr.io/lrmtheboss/bossdockerimages:nodejs_20`
* [22](/nodejs/22)
    * `ghcr.io/lrmtheboss/bossdockerimages:nodejs_22`

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

* [13](/postgres/13)
    * `ghcr.io/lrmtheboss/bossdockerimages:postgres_13`
* [14](/postgres/14)
    * `ghcr.io/lrmtheboss/bossdockerimages:postgres_14`
* [15](/postgres/15)
    * `ghcr.io/lrmtheboss/bossdockerimages:postgres_15`
* [16](/postgres/16)
    * `ghcr.io/lrmtheboss/bossdockerimages:postgres_16`
* [17](/postgres/17)
    * `ghcr.io/lrmtheboss/bossdockerimages:postgres_17`

### [Redis](/redis)

Redis images for pterodactyl panel.

* [7](/redis/6)
    * `ghcr.io/lrmtheboss/bossdockerimages:redis_7`