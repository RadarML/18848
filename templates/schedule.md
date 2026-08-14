<table class="schedule">
{% for lecture in schedule %}
<tr{% if lecture.highlight %} class="highlight-{{ lecture.highlight }}"{% endif %}>
    <td>{{ lecture.date }}</td>
    <td>{%- set parts = [] -%}
        {%- if lecture.topic -%}
            {%- if lecture.bold | default(true) -%}
                {%- set _ = parts.append('<b>' ~ lecture.topic ~ '</b>') -%}
            {%- else -%}
                {%- set _ = parts.append(lecture.topic) -%}
            {%- endif -%}
        {%- endif -%}
        {%- if lecture.description -%}
            {%- set _ = parts.append(lecture.description) -%}
        {%- endif -%}
        {%- if lecture.assignment -%}
            {%- set _ = parts.append('<i>' ~ lecture.assignment ~ '</i>') -%}
        {%- endif -%}
        {{ parts | join('<br>') }}
    </td>
</tr>
{% endfor %}
</table>
