{% assign topic=include.topic %}

<article class="b-topic" id="{{ topic.id }}">
	<h3 class="b-topic__title">{% if topic.speaker %}<a href="/2019/speakers#{{ topic.id }}">{{topic.speaker}}</a> - {% endif %} {{ topic.title }}</h3>
	{% if topic.slideshare == true %}
    {% include 2019/pages/topic-slides-slideshare.md topic=topic %}
	{% endif %}
	{% include 2019/pages/topic-output.md topic=topic %}

</article>