---
label: Syntax Testing
icon: code
order: 100
---


#### 1

||| Android
{{ android_gefunden = false }}
{{~ for post in content.blog.posts ~}}
{{~ if!android_gefunden && (post.categories contains "android") ~}}
[!card vert]({{ post.filePath }})
{{ android_gefunden = true }}
{{~ end ~}}
{{~ end ~}}

{{ if!android_gefunden }}

[!info] Keine Beiträge
Derzeit sind im Blog-Archiv noch keine Einträge für die Plattform Android vorhanden.
{{ end }}

||| iOS
{{ ios_gefunden = false }}
{{~ for post in content.blog.posts ~}}
{{~ if!ios_gefunden && (post.categories contains "ios") ~}}
[!card vert]({{ post.filePath }})
{{ ios_gefunden = true }}
{{~ end ~}}
{{~ end ~}}

{{ if!ios_gefunden }}

[!info] Keine Beiträge
Derzeit sind im Blog-Archiv noch keine Einträge für die Plattform iOS vorhanden.
{{ end }}