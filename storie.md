---
layout: page
title: Storie
permalink: /storie/
---

In questa pagina raccontiamo le principali storie di successo che questo progetto è riuscito a realizzare. Tante piccole cose che, messe insieme, speriamo offrano un contributo utile.

{: .table .table-striped #storie}
Storia          |Link                    |Come è finita             |Grazie a     |Data di Chiusura
:---------------|:-----------------------|:-------------------------|:------------|:-------------------
{% for member in site.data.storie %} {{member.Fabbisogno}} | [Link]({{member.Link}}) | {{member.Conclusione}} | {{member.Grazie}} | {{member.Data_Chiusura}}
{% endfor %}

