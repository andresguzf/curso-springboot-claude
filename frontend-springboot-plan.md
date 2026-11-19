
# Planificación Frontend React + Spring Boot

Genera una planificación tipo **wizard**, para ir paso a paso en la creación de nuestro frontend, que se integrará con nuestro backend desarrollado en **Spring Boot**.

En el proyecto de Spring Boot tienes el archivo `CLAUDE.md`, que contiene todo el contexto del backend, incluidos los endpoints y toda la información necesaria para realizar la integración.

Para esta aplicación frontend, utiliza **React en su última versión**, y crea también un diseño **UI/UX moderno y profesional utilizando Tailwind CSS** como framework de estilos.

## 1. Mensajes flash

Ten en cuenta los **mensajes flash** cuando se crean, modifican o eliminan registros, ya sean clientes o usuarios.

Estos mensajes deben:

- Mostrarse en la parte superior de la aplicación o del dashboard.
- Permanecer visibles durante aproximadamente **5 segundos**.
- Desaparecer automáticamente después de ese tiempo.
- Poder cerrarse manualmente mediante una **X**.

## 2. Administración de clientes, usuarios y roles

El administrador no solamente debe administrar clientes, sino también gestionar usuarios y roles, incluyendo las siguientes operaciones:

- Visualizar usuarios.
- Crear usuarios.
- Listar usuarios.
- Cambiar los roles de los usuarios.
- Crear nuevos roles.

### Reglas de seguridad

Ten en cuenta que el backend ya implementa reglas de seguridad para los administradores:

- Un administrador no puede eliminarse a sí mismo.
- Un administrador tampoco puede eliminar al único administrador existente en el sistema.
- Hay que tener especial cuidado al modificar o quitar el rol de administrador a un usuario cuando no existan otros administradores disponibles.

## 3. Ventanas modales de confirmación

Cuando se realice una eliminación, en lugar de utilizar la típica alerta de JavaScript (`alert()` o `confirm()`), debe mostrarse una **ventana modal de confirmación**.

Esta ventana debe tener una interfaz gráfica moderna con estilos de Tailwind CSS, preguntar al usuario si realmente desea eliminar el registro y ofrecer las opciones de **Confirmar** o **Cancelar**.

## 4. Paginación, búsquedas y filtros

También debes considerar:

- **Paginación** en las listas y tablas.
- **Búsquedas** por nombre, apellido y correo electrónico.
- **Filtros** por fecha y otros parámetros que consideres convenientes según los datos disponibles.
- Los filtros deben ubicarse en un **sidebar lateral izquierdo**.
- El sidebar debe ser **colapsable**, de manera que pueda ocultarse para aprovechar mejor el espacio disponible y permitir visualizar la tabla completa.

## 5. Planificación tipo wizard

La planificación debe estar organizada paso a paso, siguiendo un flujo tipo **wizard**, para implementar progresivamente cada funcionalidad del frontend y su integración con el backend de **Spring Boot**.
