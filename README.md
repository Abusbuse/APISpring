# R5.08 - Qualité de développement - Colle

> Auteurs: Flavien MARCK & Grégory WITTMANN \
> Date: 11 décembre 2023 \
> Version: 1.0

## 1. Introduction

Le projet consiste à déployer une API REST en utilisant le framework Spring Boot, reliée à une base de données.

## 2. Prérequis

- Java 17
- Docker & Docker-compose
- Maven
- Git

## 3. Installation

### 3.1. Récupération du projet

```bash
git clone https://github.com/Abusbuse/APISpring.git
```

### 3.2. Lancement de la base de données

```bash
docker-compose up -d
```

### 3.3. Lancement de l'application

```bash
mvn spring-boot:run
```

## 4. Utilisation

### 4.1. Création d'un utilisateur

```bash
curl -X POST -H "Content-Type: application/json" -d '{"name":"John", "lastname":"Doe"}' http://localhost:8080/user/add
```

### 4.2. Récupération de tous les utilisateurs

```bash
curl http://localhost:8080/user/all
```
