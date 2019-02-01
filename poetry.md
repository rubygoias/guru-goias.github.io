---
layout: page
permalink: /encontros/
title: Encontros
---

<p>
    Para saber do próximo encontro acompanhe o <a href="https://telegram.me/guru_go" target="_blank"> grupo do Telegram</a>.
<br/>
    Veja aqui um histórico dos nossos encontros.
</p>

<br/>
<hr/>
<br/>
<table class="table">
<tbody class="post-list">
{% for poem in site.poetry reversed %}
    <tr>        
        <td>
            <a class="" href="{{ poem.url | prepend: site.baseurl }}">{{ poem.title }}</a>
        </td> 
        <td><p class="post-meta">{{ poem.date | date: ' %-d/%m/%Y' }}</p></td>
    </tr>
{% endfor %}

</tbody>
</table>

<style>
.table {
    width: 100%;
    margin-bottom: 1rem;
    background-color: transparent;
}

table {
    border-collapse: collapse;
}