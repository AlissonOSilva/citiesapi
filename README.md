# API de cidades

# Requisitos
Git 

Docker

Java 8

Comunidade IntelliJ

# DataBase

PostgreSQL

Ativar extensão para calculo da distancia entre cidades.

CREATE EXTENSION cube;
CREATE EXTENSION earthdistance;

# Query Earth Distance


Point

select ((select lat_lon from cidade where id = 4929) <@> (select lat_lon from cidade where id=5254)) as distance;

Cube

select earth_distance(
ll_to_earth(-21.95840072631836,-47.98820114135742),
ll_to_earth(-22.01740074157715,-47.88600158691406)
) as distance;

# Spring Boot
https://start.spring.io/

Java 8

Gradle Project

Jar

Spring Web

Spring Data JPA

PostgreSQL Driver

# Spring Data
jpa.query-methods

# Properties
appendix-application-properties

jdbc-database-connectio

# Types
JsonTypes

UserType
