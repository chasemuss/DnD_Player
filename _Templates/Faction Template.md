<% "---" %>
tags:
- Faction/<% tp.file.title.replace(".md", "").replace(/ /g, "_") %>
- Location/<% tp.file.path(true).replace("/Factions", "").replace("/" + tp.file.title + ".md", "").replace(/ /g, "_") %>
alias:
- 
home_base:
- 
<% "---" %>

# Description


# Members


## Former Members

<%*
	const dir = "folder/folder/something/"
	const current_path = tp.file.path(true).replace(".md", "")
	console.log(current_path)
	if (!tp.file.exists(current_path)) {
		await this.app.vault.createFolder(current_path)
	}
	await tp.file.move(tp.file.path(true) + "/" + tp.file.title)
%>