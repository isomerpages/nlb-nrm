---
title: Book Clubs
permalink: /initiatives/book-clubs/
---

<style>
	.filteredtable tbody tr,
	.tablefilter{
		display:none;
	}
	
	#class1.tablefilter:checked ~ table tbody tr.class1,
	#class2.tablefilter:checked ~ table tbody tr.class2,
	#class3.tablefilter:checked ~ table tbody tr.class3,
	#class3.tablefilter:checked ~ table tbody tr.class4	{
		display:table-row;
	}
	.tablefilter + label{
		cursor: pointer;
		background-color: #666;
		color: #fff;
		padding: 3px;
	}
	.tablefilter:checked + label{
		background-color: #111;
	}
	#all.tablefilter:checked ~ table tbody tr{
		display:table-row;
	}
</style>
	
![banner book clubs](\images\Next-Chapter_Meira-Chand.jpg)

### Join a Book Clubs

Keen to share your thoughts about books you have read? Why not join a book club? Check out the clubs we have at the public libraries conducted in English, Chinese, Malay and Tamil for various age groups.

For current club meeting dates and registration, please visit [HERE](http://www.nlb.gov.sg/golibrary){:target="_blank"}.

<div class="container">
	<div class="row">
		<!-- Filter -->
		<input type="checkbox" class="tablefilter" name="all" id="all" checked />
		<label for="all">All</label>	
		<input type="checkbox" class="tablefilter" name="class1" id="class1" checked />
		<label for="class1">English</label>				
		<input type="checkbox" class="tablefilter" name="class2" id="class2" checked />
		<label for="class2">Chinese</label>		
		<input type="checkbox" class="tablefilter" name="class3" id="class3" checked />
		<label for="class3">Malay</label>
		<input type="checkbox" class="tablefilter" name="class4" id="class4" checked />
		<label for="class4">Tamil</label>
		
		{%- assign book-clubs-data = site.data.book-clubs -%}
		
		<!-- Table -->
		<table class="table table-bordered table-striped filteredtable">
			<thead>
				<tr class="class1">
					<td>Name</td>
					<td>Venue</td>
					<td>Language</td>
					<td>Description</td>
				</tr>
			</thead>
			<tbody>
				{%- for book-club in book-clubs-data.book-clubs -%}
				<tr class="class1">
					<td>{{- book-club.name -}}</td>
					<td>{{- book-club.venue -}}</td>
					<td>{{- book-club.language -}}</td>
					<td>{{- book-club.description -}}</td>
				</tr>
			</tbody>
		</table>
	</div>
</div>