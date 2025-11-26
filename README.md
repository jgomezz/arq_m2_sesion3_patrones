# 📚 Sistema de Gestión de Biblioteca

**Ejercicio Práctico:** Repository Pattern + Data Mapper + H2 Database

---

## 📋 Objetivo

Desarrollar un sistema de gestión de biblioteca que implemente **Repository Pattern** con **Data Mapper** usando Spring Boot y H2.

---

## 🎯 Funcionalidades Requeridas

### Gestión de Libros
- ✅ Registrar nuevos libros
- ✅ Actualizar información de libros
- ✅ Eliminar libros
- ✅ Consultar por ID, ISBN, autor o género

### Gestión de Préstamos
- ✅ Prestar libro (marca como no disponible)
- ✅ Devolver libro (marca como disponible)
- ✅ Listar libros disponibles
- ✅ Listar libros prestados

### Búsquedas y Reportes
- ✅ Buscar por género, autor o año
- ✅ Contar disponibles y prestados

---

## 📊 Modelo de Datos

| Campo | Tipo | Restricciones |
|-------|------|---------------|
| id | Long | Auto-generado |
| titulo | String | Requerido, max 200 caracteres |
| autor | String | Requerido, max 100 caracteres |
| isbn | String | Requerido, único, formato `ISBN-XXX-X-XXXX-XXXX-X` |
| genero | String | Requerido, max 50 caracteres |
| anioPublicacion | Integer | Entre 1000 y 2025
