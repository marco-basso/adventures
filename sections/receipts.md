---
layout: page
---

# Ricette

{% for receipt in site.receipts %}
- [{{ receipt.title }}]({{ receipt.url | relative_url }})
    {% if receipt.tried != true %}<small>**da provare**</small>{% endif %}
{% endfor %}
