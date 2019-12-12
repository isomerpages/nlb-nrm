---
title: Book Clubs
permalink: /initiatives/book-clubs/
---

![banner book clubs](\images\Next-Chapter_Meira-Chand.jpg)

### JOIN A BOOK CLUB

Keen to share your thoughts about books you have read? Why not join a book club? Check out the clubs we have at the public libraries conducted in English, Chinese, Malay and Tamil for various age groups.

For current club meeting dates and registration, please visit [HERE](http://www.nlb.gov.sg/golibrary){:target="_blank"}.

{%- assign book-club-data = site.data.book-clubs -%}
	{%- for book-club in book-club-data.book-clubs -%}
		{{- book-club.name -}}, {{- book-club.language -}}, {{- book-club.location -}}
	{%- endfor -%}
	{{- content -}}