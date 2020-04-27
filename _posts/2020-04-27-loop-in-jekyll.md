---
layout: post
title: "Перечисление значений переменной в цикле (Jekyll)"
date: 2020-04-27
---

```
---
somevars: [1980 , 1979 , 1978]

{%- if page.somevars -%}
    {% for somevar in page.somevars %}
        {{ somevar }}</br>
    {% endfor %}
{%- endif -%}
```
