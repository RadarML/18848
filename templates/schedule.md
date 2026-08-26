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
        {%- if lecture.assignment -%}
            {%- set _ = parts.append('<i>' ~ lecture.assignment ~ '</i>') -%}
        {%- endif -%}
        {{ parts | join('<br>') }}
    </td>
</tr>
{% endfor %}
</table>
