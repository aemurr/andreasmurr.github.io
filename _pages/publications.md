---
layout: single
title: "Publications"
permalink: /publications/
author_profile: true
description: "Peer-reviewed articles and chapters by Andreas E. Murr (University of Warwick, CIDE). Election forecasting, electoral behaviour, political methodology."
---

Below are my peer-reviewed publications. For each, I link the DOI, an
open-access version of the manuscript where available, and (where applicable)
replication code. Working papers and preprints are on the [Working Papers]({{ '/working-papers/' | relative_url }}) page.

For citation metrics see my [Google Scholar](https://scholar.google.com/citations?user=YNLsHWMAAAAJ) and [ORCID](https://orcid.org/0000-0002-9536-0118) profiles.

{% assign by_year = site.data.publications | group_by: "year" | sort: "name" | reverse %}

{% for group in by_year %}
## {{ group.name }}

{% for pub in group.items %}
{% include publication.html pub=pub %}
{% endfor %}
{% endfor %}
