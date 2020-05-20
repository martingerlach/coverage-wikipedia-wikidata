# coverage-wikipedia-wikidata

Check the number of pages in wikipedia (e.g. enwiki) for which there is no wikidata-item.

For each project, we get all pages from the main namespace that are no redirects from the [mediawiki_page table](https://wikitech.wikimedia.org/wiki/Analytics/Data_Lake/Edits#Raw_Mediawiki_data).

We then join the [wikidata-item-page-link table](https://wikitech.wikimedia.org/wiki/Analytics/Data_Lake/Edits/Wikidata_item_page_link) to get the corresponding wikidata item (if it exists).

The main result is that for most wikipedias, coverage is >99%.
