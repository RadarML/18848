<table class="schedule">
{% for lecture in schedule %}
<tr>
    <td>{{ lecture.week }}</td>
    <td><b>{{ lecture.title }}</b>
        {%- if lecture.desc %}
        <br>{{ lecture.desc }}
        {%- endif %}
    </td>
</tr>
{% endfor %}
</table>
