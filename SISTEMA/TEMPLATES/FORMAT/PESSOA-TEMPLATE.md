---
created:
  - '[[<% tp.date.now("YYYY-MM-DD") %>]]'
cssclasses:
  - hide-properties_editing
  - hide-properties_reading
---
| `Coleção` | `INPUT[suggester(optionQuery("")):collection]`   | `Relacionados` | `INPUT[inlineListSuggester(optionQuery(""), option(something, other),  useLinks(true), showcase):related]`  |

---
# [[<% tp.file.title %>]] 

|👤 **Pessoa**|
|---|
|**Tipo Relação:** `INPUT[inlineSelect(option('Colega'), option('Cliente'), option('Fornecedor'), option('Amigo'), option('Familiar'), option('Mentor'),showcase):TipoRelacao]`|
|**Organização:** `INPUT[text:Organizacao]`|
|**Cargo:** `INPUT[text:Cargo]`|
|**Área de Atuação:** `INPUT[text:AreaAtuacao]`|
|**Contato:** `INPUT[inlineList:Contatos]`|
|**Redes Sociais:** `INPUT[inlineList:RedesSociais]`|
|**Localização:** `INPUT[text:Localizacao]`|
|**Aniversário:** `INPUT[date:Aniversario]`|
|**Tags:** `INPUT[inlineList:Tags]`|

<%tp.file.cursor()%>

---

# Sobre

# Histórico de Interações

# Interesses em Comum

# Projetos Relacionados

# Notas

---

Last modified :   `="[[" + dateformat(date(today), "yyyy-MM-dd") + "]]"` - `$= dv.current().file.mtime`