---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: true
description: ""
tags: ['']
images: ['']
blog_list_image: 
author: Saúl Zalimben
slug: {{ replace .Name "_" "-" }}
idiom: 
---

---
<!-- 
## New Cool Posts

{{ range first 10 ( where .Site.RegularPages "Type" "cool" ) }}
* [{{ .Title }}](blog/english/posts/{{.Filename}}) de este artículo.
{{ end }} 

 -->