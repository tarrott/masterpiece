---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: halffalse
{{ replace (.Dir | after 10) "/" "" }}: ['']
---

