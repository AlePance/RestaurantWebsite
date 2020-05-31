---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
---
**Insert lead paragraph here.**

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* {{ .Title }}
{{ end }}