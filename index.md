   {% assign doclist = site.pages | sort: 'url'  %}
    <ul>
       {% for doc in doclist %}
            {% if doc.name contains '.pdf' or doc.name contains '.ppt'%}
                <li><a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.url }}</a></li>
            {% endif %}
        {% endfor %}
    </ul>
