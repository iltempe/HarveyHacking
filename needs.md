---
layout: page
title: Needs
permalink: /needs/
---
<div class="panel-group">
	{% for member in site.data.needs %}
	<div class="panel-body">
	<a href="https://api.harveyneeds.org/needs/{{ member.Id | datapage_url: '.' }}" class="list-group-item">
		<h4 class="list-group-item-heading">{{member.location_name | markdownify}}</h4>
		<p class="list-group-item-text">{{member.location_address | markdownify}}</p>
    <p class="list-group-item-text">{{member.needs}}</p>
	</a>
<div class="panel-footer">
<ul class="share-buttons">
  <li>Share:</li>
  <li><a href="http://terremotocentroitalia.info/issues/{{ member.number | datapage_url: '.' }}" title="Copy link"><img alt="Copy link" src="/img/icone/link.png"></a></li>
  <li><a href="https://www.facebook.com/sharer/sharer.php?u=http://terremotocentroitalia.info/issues/{{ member.number | datapage_url: '.' }}&title={{member.title|truncate:70|uri_escape}} | {{ site.title }}" title="Share on Facebook" target="_blank"><img alt="Share on Facebook" src="/img/icone/Facebook.png"></a></li>
  <li><a href="https://twitter.com/intent/tweet?url=http://terremotocentroitalia.info/issues/{{ member.number | datapage_url: '.' }}&text={{member.title|truncate:50|uri_escape}}&via=terremotocentro&hashtags=terremotocentroitalia" target="_blank" title="Tweet"><img alt="Tweet" src="/img/icone/Twitter.png"></a></li>
 <li><a href="https://plus.google.com/share?url=http://terremotocentroitalia.info/issues/{{ member.number | datapage_url: '.' }}" target="_blank" title="Share on Google+"><img alt="Share on Google+" src="/img/icone/Google+.png"></a></li>
 <li><a data-proofer-ignore href="mailto:?subject={{member.title|truncate:70|uri_escape}} | {{site.title}}&body={{member.title|truncate:70|uri_escape}}%20Clicca qui:%20http://terremotocentroitalia.info/issues/{{ member.number | datapage_url: '.' }}" title="Send email"><img alt="Send email" src="/img/icone/Email.png"></a></li>
</ul>
</div>
</div>
{% endfor %}
</div>
