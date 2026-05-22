---
label: Syntax Testing
icon: code
order: 100
---


||| Android

{{
android_post = null
for post in content.blog.posts
if!android_post
if post.categories
if post.categories contains "android"
android_post = post
end
end
end
end
}}

{{ if android_post }}
[!card vert]({{ android_post.filePath }})
{{ else }}

[!info] Keine Beiträge
Derzeit sind im Blog-Archiv noch keine Einträge für die Plattform Android vorhanden.
{{ end }}

||| iOS

{{
ios_post = null
for post in content.blog.posts
if!ios_post
if post.categories
if post.categories contains "ios"
ios_post = post
end
end
end
end
}}

{{ if ios_post }}
[!card vert]({{ ios_post.filePath }})
{{ else }}

[!info] Keine Beiträge
Derzeit sind im Blog-Archiv noch keine Einträge für die Plattform iOS vorhanden.
{{ end }}