<table class="schedule">
{% for lecture in schedule %}
<tr{% if lecture.highlight %} class="highlight-{{ lecture.highlight }}"{% endif %}>
    <td>{{ lecture.date }}</td>
    <td>{%- set parts = [] -%}
        {%- if lecture.topic -%}
            {%- if lecture.bold | default(true) -%}
                {%- set topic = '<b>' ~ lecture.topic ~ '</b>' -%}
            {%- else -%}
                {%- set topic = lecture.topic -%}
            {%- endif -%}
            {%- if lecture.slides -%}
                {%- set topic = topic ~ '&emsp;<a href="' ~ lecture.slides ~ '">[slides]</a>' -%}
            {%- endif -%}
            {%- set _ = parts.append(topic) -%}
        {%- endif -%}
        {%- if lecture.description -%}
            {%- set _ = parts.append(lecture.description) -%}
        {%- endif -%}
        {%- if lecture.resources -%}
            {%- for category, links in lecture.resources.items() -%}
                {%- set links_html = [] -%}
                {%- for name, url in links.items() -%}
                    {%- set _ = links_html.append('<a href="' ~ url ~ '">[' ~ name ~ ']</a>') -%}
                {%- endfor -%}
                {%- set _ = parts.append(category ~ ':&ensp;' ~ (links_html | join('&ensp;'))) -%}
            {%- endfor -%}
        {%- endif -%}
        {%- if lecture.assignment -%}
            {%- set _ = parts.append('<i>' ~ lecture.assignment ~ '</i>') -%}
        {%- endif -%}
        {{ parts | join('<br>') }}
    </td>
</tr>
{% endfor %}
</table>
