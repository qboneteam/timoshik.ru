---
layout: post
title: "Перечисление значений переменной в цикле (Jekyll)"
date: 2020-04-27
---


В заголовке определяем значения переменных:
```
---
somevars: [1980 , 1979 , 1978]
---
```

Затем перечисляем их:
<pre>
___{% if page.somevars -%}
___    {% for somevar in page.somevars %}
___        {{ somevar }}</br>
___    {% endfor %}
___{% endif %}
</pre>
