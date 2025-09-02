<!-- Титульная страница -->
<div class="title-page-container">
	<div class="page-title"><% tp.file.title %></div>

<!-- Таблица с метаданными -->
<table class="metadata-table">
	  <tr>
		<td><strong>Авторы</strong></td>
		<td><% tp.frontmatter.Authors ? tp.frontmatter.Authors.join(", ") : "не указано" %></td>
	  </tr>
	  <tr>
		<td><strong>Теги</strong></td>
		<td><% tp.frontmatter.tags ? tp.frontmatter.tags.join(", ") : "не указаны" %></td>
	  </tr>
	  <tr>
		<td><strong>Закончена</strong></td>
		<td><% tp.frontmatter.isDone ? "Да" : "В работе" %></td>
	  </tr>
	  <tr>
		<td><strong>Дата создания</strong></td>
		<td><% tp.frontmatter.createdAt || "не указана" %></td>
	  </tr>
</table>
</div>


<!-- Основной контент статьи -->
<% tp.frontmatter.content ? tp.frontmatter.content : "" %>