---
title: Book Clubs
permalink: /initiatives/book-clubs/
---

![banner book clubs](\images\Next-Chapter_Meira-Chand.jpg)

### JOIN A BOOK CLUB

Keen to share your thoughts about books you have read? Why not join a book club? Check out the clubs we have at the public libraries conducted in English, Chinese, Malay and Tamil for various age groups.

For current club meeting dates and registration, please visit [HERE](http://www.nlb.gov.sg/golibrary){:target="_blank"}.

<div class="content">
{%- assign nrm-book-clubs = site.data.book-clubs -%}
	{%- for book-club in nrm-book-clubs.book-clubs -%}
		{{- book-club.name -}}<br/>
	{%- endfor -%}
	{{- content -}}
</div>