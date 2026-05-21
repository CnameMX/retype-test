#### 1

{{ for post in content.blog.posts ~}}
{{~ if post.categories | array.contains "android" ~}}
[!card vert]({{ post.filePath }})
{{~ end ~}}

{{ for post in content.blog.posts ~}}
{{~ if post.categories | array.contains "ios" ~}}
[!card vert]({{ post.filePath }})
{{~ end ~}}
