---
layout: home
title: Home
---

Hello. This is my homepage.
---
layout: home
title: Home
---

{% assign latest = site.posts.first %}

{% if latest %}
# Latest

## [{{ latest.title }}]({{ latest.url }})
*{{ latest.date | date: "%B %-d, %Y" }}*

{{ latest.excerpt }}

[Read more →]({{ latest.url }})

---

[Past posts →](/posts/)
{% else %}
No posts yet.
{% endif %}
