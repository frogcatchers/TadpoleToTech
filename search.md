---
layout: page
title: Search
permalink: /search/
---

<div id="search-container">
  <input type="text" id="search-input" placeholder="Search posts and learning paths...">
  <ul id="results-container"></ul>
</div>

<script src="{{ site.baseurl }}/assets/js/simple-jekyll-search.min.js"></script>

<script>
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '{{ site.baseurl }}/search.json',
  searchResultTemplate: '<li><a href="{url}">{title}</a> <span class="search-category">({category})</span><br><small>{tags}</small></li>',
  noResultsText: 'No results found',
  limit: 10,
  fuzzy: false,
  exclude: ['Welcome']
})
</script>

<style>
#search-input {
  width: 100%;
  padding: 10px;
  font-size: 16px;
  border: 1px solid #ccc;
  border-radius: 4px;
  margin-bottom: 15px;
}

#results-container {
  list-style: none;
  padding: 0;
}

#results-container li {
  padding: 10px;
  border-bottom: 1px solid #eee;
}

.search-category {
  color: #666;
  font-style: italic;
}
</style>
