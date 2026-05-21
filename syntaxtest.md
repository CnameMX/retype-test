---
label: Syntax Testing
icon: code
order: 100
---


#### 1

{{ for post in content.blog.posts ~}}
{{~ if post.categories | array.contains "android" ~}}
    [!card vert]({{ post.filePath }})
{{~ end ~}}

#### 2


{{ for post in content.blog.posts.categories ~}}
{{~ post.title | array.contains "ios" ~}}
    [!card vert]({{ post.filePath }})
{{~ end ~}}

#### 3

{{ for post in content.blog.posts.categories ~}}
- {{ post.title }}