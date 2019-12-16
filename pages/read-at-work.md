---
title: "Read@Work"
permalink: /read-at-work/
---

![banner read@work](\images\RWFeature-e1560911840942.jpg)

Launched in late 2016, Read@Work supports organisations in seeding a reading culture at the workplace. More than 60 organisations are on board Read@Work to strengthen their staff’s learning and reading habits. Join us to enjoy a complimentary suite of services designed to encourage working adults to read and learn:

* Monthly Read@Work EDMs to get staff in the mood for reading.
* Free Lunch and Learn programmes, including bite-sized talks by professional trainers and librarians’ sharing on intriguing topics like graphic novels or poetry.
* Sharing by librarians about eResources such as Digital Business Library, Press Display, Lynda.com and Overdrive.
* Supplementary reading recommendations for Leaders as Reading Advocates, where we encourage our partners’ leaders and avid readers to share their favourite reads with colleagues.
* Services of a dedicated librarian to tailor programmes that fit your organisations' needs.
* Include our support at events e.g. learning festivals and membership drives.

Join Read@Work today.

Latest EDM: [Read@Work_Curiosity](/edms/Read@Work_Curiosity.pdf){:target="_blank"}

Past EDMs:

* [Read@Work_Adaptability](/edms/Read@Work_Adaptability.pdf){:target="_blank"}
* [Read@Work_Creativity](/edms/Read@Work_Creativity-linkable-PDF.pdf){:target="_blank"}
* [Read@Work_Adversity](/edms/Read@Work_Adversity.pdf){:target="_blank"}

Enquire through <read@nlb.gov.sg> with "Read@Work" in the subject.

<p/>

{%- assign nrm-partners = site.data.nrm-partners -%}
<div class="content">
	<div class="acc-kontainer">
		{%- for partner-type in nrm-partners.partner-structure -%}
			{%- if partner-type.title = "Read@Work Partners" -%}
				<div>
					<input type="radio" name="acc" id="acc{{forloop.index}}">
					<label for="acc{{forloop.index}}"><i></i> {{- partner-type.title -}} </label>
					<div class="acc-body">
						<div class="row is-multiline">
							{%- for partner in partner-type.partners -%}
							<div class="col is-4 padding--right--xl padding--bottom">
								<div class="margin--top--none">
									{{- partner.name -}}
								</div>
							</div>
							{%- endfor -%}
						</div>
					</div>
				</div>
			{%- endif -%}
		{%- endfor -%}
	</div>
</div> 