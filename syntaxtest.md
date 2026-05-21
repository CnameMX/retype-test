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
new