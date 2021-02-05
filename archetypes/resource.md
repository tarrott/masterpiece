---
title: "{{ replace .Name "-" " " | title }}"
date: {{ .Date }}
draft: false
{{ replace (.Dir | after 10) "/" "" }}: ['']
---

