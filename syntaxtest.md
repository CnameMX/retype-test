---
label: Syntax Testing
icon: code
order: 100
---


#### 1

{{ android_gefunden = false }}
{{~ for post in content.blog.posts ~}}
{{~ if post.categories | array.contains "android" ~}}
[!card vert]({{ post.filePath }})
{{ android_gefunden = true }}
{{~ end ~}}
{{~ end ~}}




{{ ios_gefunden = false }}
{{~ for post in content.blog.posts ~}}
{{~ if post.categories | array.contains "ios" ~}}
[!card vert]({{ post.filePath }})
{{ ios_gefunden = true }}
{{~ end ~}}
{{~ end ~}}

