---
# Adapted from Mr. Green Jekyll Theme (https://github.com/MrGreensWorkshop/MrGreen-JekyllTheme)
# Copyright (c) 2023 Gerardo Vitagliano
# Licensed under MIT

layout: default
# Publications page
---
{%- include multi_lng/get-lng-by-url.liquid -%}
{%- assign lng = get_lng -%}

{%- assign publications_data = page.page_data | default: site.data.content.publications[lng].page_data -%}

{%- capture project_container_style -%} style="background-color:{{ project_data.main.back_color }};" {%- endcapture -%}

{%- if site.data.conf.others.publications.use_rows_as_link -%}
{%- assign hover_class = "table-hover" -%}
{%- endif -%}

{%- for category in publications_data.category %}
<div class="multipurpose-container publication-container" id="{{ category.type }}" style="border-left-color:{{ category.color }};">
  <h2>{{ category.title }}</h2>

I strive to make my research accessible, reproducible, and available for consultation. If a paper and/or code repository is not directly available from the list below, feel free to reach out.

  <table class="table {{ hover_class }}">
    <thead>
      <tr>
        <th>{{ site.data.lang[lng].publications.reference_text }}</th>
        <th>{{ site.data.lang[lng].publications.date_text }}</th>
        <th>{{ site.data.lang[lng].publications.doc_text }}</th>
        <th>{{ site.data.lang[lng].publications.code_text }}</th>
      </tr>
    </thead>
    <tbody>
      {%- for list in publications_data.list %}
        {%- if list.type != category.type %}{% continue %}{% endif -%}
        {%- assign link_onclick = nil -%}
        {%- capture link_paper -%} <a href="{{ list.paper_url }}" target="_blank" rel="noopener noreferrer"><b>{{ list.paper_source }}</b></a> {%- endcapture -%}
        {%- capture link_code -%} <a href="{{ list.code_url }}" target="_blank" rel="noopener noreferrer"><b>{{ list.code_source }}</b></a> {%- endcapture -%}
        <tr class="publication-item" {{ link_onclick }}>
          <td width="100%">
            <p>{{ list.authors }} : <b> {{ list.title }} </b> <i> {{ list.venue }} </i>, {{list.year}} </p>
          </td>
          <td>
            <p>{{ list.year }}</p>
          </td>
          <td>
            <p>{{ link_paper }}</p>
          </td>
           <td>
            <p>{{ link_code }}</p>
          </td>
        </tr>
      {%- endfor %}
    </tbody>
  </table>
</div>
{% endfor %}
