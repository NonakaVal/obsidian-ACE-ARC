---
created:
  - '[[2025-08-16]]'
cssclasses:
  - hide-properties_editing
  - hide-properties_reading
---
| `Coleção` | `INPUT[suggester(optionQuery("")):collection]`   | `Relacionados` | `INPUT[inlineListSuggester(optionQuery(""), option(something, other),  useLinks(true), showcase):related]`  |

---
# [[TEMPLATE-BASE]] 

|🎥 **Vídeo**|
|---|
|**Canal/Criador:** `INPUT[text:Criador]`|
|**URL:** `INPUT[text:URL]`|
|**Status:** `INPUT[inlineSelect(option("Para assistir", "Assistindo", "Assistido", "Revisitar"), showcase):Status]`|

<% tp.file.cursor() %>

---

# Descrição

# Principais Pontos

# Aprendizados

# Ações Derivadas

---

Last modified :   `="[[" + dateformat(date(today), "yyyy-MM-dd") + "]]"` - `$= dv.current().file.mtime`