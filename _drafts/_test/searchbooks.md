---
layout: page-11
title: kitap ara
published: false
---

<style>
	#search-container {
	    max-width: 100%;
	}

	input[type=text] {
		font-size: normal;
	    outline: none;
	    padding: 1rem;
		background: rgb(236, 237, 238);
	    width: 100%;
		-webkit-appearance: none;
		font-family: inherit;
		font-size: 100%;
		border: none;
	}
	#results-container {
		margin: .5rem 0;
	}
</style>

<!-- Html Elements for Search -->
<div id="search-container">
<input type="text" id="search-input" placeholder="Search for a book...">
<ol id="results-container"></ol>
</div>

<!-- Script pointing to search-script.js -->
<script src="/search.js" type="text/javascript"></script>

<!-- Configuration -->
<script type="text/javascript">
SimpleJekyllSearch({
  searchInput: document.getElementById('search-input'),
  resultsContainer: document.getElementById('results-container'),
  json: '/searchbooks.json',
  searchResultTemplate: '<div style="text-transform: lowercase;"><li><a href="{url}" title="{title}">{title}</a></li></div>',
  noResultsText: 'No results found',
  limit: 30000,
  fuzzy: false,
  exclude: ['Welcome']
})
</script>
<br />
<br />
<div style="clear: both;"></div>
