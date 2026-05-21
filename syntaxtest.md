---
label: Syntax Testing
icon: code
order: 100
---


{{ string.upcase "hello world" }}
{{ array.size page.tags }}
{{ date.now.year }}

{{ for post in content.blog.posts | array.limit 3 ~}}
- [{{ post.title }}]({{ post.path }})
{{ end }}

{{ for cat in content.categories.title | array.contains "android"}}
- [{{ cat.title }}]({{ cat.path }})
{{ end }}

{{ for cat in content.categories ~}}
- [{{ cat.title }}](/categories/{{ cat.title }}) ({{ cat.pages | array.size }} pages)
{{ end }}

#### next

{{ for cat in content.categories | array.contains "android" }}
- [{{ cat.title }}](/categories/{{ cat.title }}) ({{ cat.pages | array.size }} pages)
{{ end }}

[!card]({{ (/categories/android/ | array.first).filePath }})