# This is to Test to add a non expandeble Tab
### when it works fine if not not fine

[!card]({{ {{ content.categories | array.any @string.contains "android" }}.filePath }})

[!card]({{ {{ content.categories.title | array.any @string.contains "android" }}.filePath }})

#### Das ist der neuste Blogpost
[!card]({{ content.blog.posts[0].filePath }})

#### Und das ist ein festgelegter Blogpost
[!card](/blog/New-Update-121.md)
