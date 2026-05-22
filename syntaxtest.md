---
label: Syntax Testing
icon: code
order: 100
---


[!card layout="vert" title="Newest Android Updates" kicker="Release note" text="Here you finde the newest Release notes for the Android Version" image="images/Nettask_Cyberpunk_FHD.jpg"](https://cnamemx.github.io/retype-test/tags/ios/)
[!card layout="vert" title="Newest IOS Updates" kicker="Release note" text="Here you finde the newest Release notes for The IOS Version" image="images/NetTask_Synthwave_FHD.jpg"](https://cnamemx.github.io/retype-test/tags/android/)


##### 2

{{ for cat in content.categories | array.map "title" ~}}
{{ if cat | string.contains "android" }}
It exist
{{ end }}
{{ end }}
#### 3

{{ content.categories["android"].pages | array.map "url" | array.last }}

for the whole tosting reasons