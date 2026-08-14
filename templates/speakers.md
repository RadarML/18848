<div class="grid cards speakers">
{% for person in speakers %}
<div class="card speaker">
    <img class="speaker-photo" src="{{ person.photo }}" alt="{{ person.name }}">
    <div class="speaker-body">
        <div class="speaker-name">
            <a href="{{ person.url }}">{{ person.name }}</a>
            {%- if person.affiliation %}
            <span class="speaker-affiliation">&bullet; {{ person.affiliation }}</span>
            {%- endif %}
        </div>
        {%- if person.title %}
        <div class="speaker-title">{{ person.title }}</div>
        {%- endif %}
        {%- if person.topic %}
        <div class="speaker-topic">{{ person.topic }}</div>
        {%- endif %}
    </div>
</div>
{% endfor %}
</div>
