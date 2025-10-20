---
layout: page
title: جستجو در سایت 
permalink: /search/
---

<div id="search-container">
    <input type="text" id="search-input" style="font-family: 'Vazirmatn'" placeholder="جستجو ...">
    <ul id="results-container"></ul>
</div>

<script src="{{ site.baseurl }}/assets/simple-jekyll-search.min.js" type="text/javascript"></script>

<script>
    SimpleJekyllSearch({
    searchInput: document.getElementById('search-input'),
    resultsContainer: document.getElementById('results-container'),
    searchResultTemplate: '<div style="text-align: right !important;"><a href="{url}"><h1 style="text-align:right !important;">{title}</h1></a></div>',
    json: '{{ site.baseurl }}/search.json'
    });
</script>