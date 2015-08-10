---
layout: post
title: App de Dodecaedro
---

<style type="text/css">
	table { border-collapse: collapse; }
	table tr td { border: 2px solid black; }
	table td { padding: 10px; width: 200px; }
	table th { padding: 10px; text-align:center; }
</style>

## Consideraciones Iniciales

### Usuario

<table>
	<thead>
		<th>Dato</th>
		<th>Tipo</th>
	</thead>
	<tbody>
		<tr>
			<td>Usuario</td>
			<td>String</td>
		</tr>
		<tr>
			<td>e-mail</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Password</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Birthday</td>
			<td>Date</td>
		</tr>
		<tr>
			<td>Admin</td>
			<td>Boolean</td>
		</tr>
		<tr>
			<td>Editor</td>
			<td>Boolean</td>
		</tr>
	</tbody>	
</table>
<br>

### Artículo

<table>
	<thead>
		<th>Dato</th>
		<th>Tipo</th>
	</thead>
	<tbody>
		<tr>
			<td>Title</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Author</td>
			<td>Belongs to User</td>
		</tr>
		<tr>
			<td>Thumbnail</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Excerpt</td>
			<td>Text</td>
		</tr>
		<tr>
			<td>Category</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Subcategory</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Layout</td>
			<td>String</td>
		</tr>
		<tr>
			<td>Published</td>
			<td>Boolean</td>
		</tr>
	</tbody>
</table>
<br>

+ Hosteada en Heroku
+ Login en página de inicio 
+ Tres clases de usuario:
+ My database should only handle users and information for making the articles

## Consideraciones Secundarias

+ Sesiones que caducan al cerrar el navegador
+ Sin recuerdame y sin verificación de usuario
+ Creación de usuario por el administrador
+ Contraseña default
+ División entre editores y escritores
+ División por categorías
+ Publicación con la api de github
+ Comunicación con la api de facebook y twitter
+ Creación de tareas para agendar los posts
+ Newsletter mailer
+ Trabajar con https://developer.github.com/v3/repos/contents/
	+ Creador
	+ Editor
	+ Admin
