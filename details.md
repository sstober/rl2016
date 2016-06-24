---
layout: default
title: Schedule
---

# Detailed Schedule
-------------------

<p>* = optional reading</p>

<table class="table table-striped"> 
  <tbody>
    <tr>
      <th>Date</th>
      <th>Contents</th>	  
    </tr>
	
    {% for lecture in site.data.schedule.lectures %}
    <tr>
        <td>{{ lecture.date | date: "%d %b" }}</td>
        <td>        
		   {% for lect in lecture.content %}
		   <b><p class="{{ lecture.type }}">		  
	        {% if lect.slides %}
				<a href="{{ lect.slides }}">{{ lect.title }}</a>
            {% else %}
				{{ lect.title }}
			{% endif %}
		    </p></b>
		   {% endfor %}

       {% if lecture.note %}
       <p>Note: {{ lecture.note }}</p>
       {% endif %}

          {% if lecture.reading %}
            <p>Readings:  
             <ul>
                {% for reading in lecture.reading %}
                   <li>
                        {% if reading.optional %}
			   *
                        {% else %}
							<i class="fa-li fa"> </i>
						{% endif %}
                        {% if reading.author %}{{ reading.author }}, {% endif %}
                        {% if reading.url %}
						    <a href="{{ reading.url }}">{{ reading.title }}</a>
                        {% else %}
                            {{ reading.title }} 
                        {% endif %}
			{% if reading.note %} {{ reading.note }} {% endif %}
                   </li>
               {% endfor %}
          </ul></p>
        {% endif %}

        <p>Objectives: <ul>{% for objective in lecture.objectives %}
          <li>{{ objective }}</li>
        {% endfor %}</ul></p>

        <p>Activities: <ul>{% for acitvity in lecture.activities %}
          <li>{{ acitvity }}</li>
        {% endfor %}</ul></p>

        
        {% for assignment in lecture.assignment %}
        <p><b>Assignment:
			    {% if assignment.link %}<a href="{{ assignment.link }}">{{ assignment.label }}</a>
		      {% else %}{{ assignment.label }}
	        {% endif %}  
          </b>

           <p>Objectives: <ul>{% for objective in assignment.objectives %}
            <li>{{ objective }}</li>
          {% endfor %}</ul></p>

          <p>Activities: <ul>{% for acitvity in assignment.activities %}
            <li>{{ acitvity }}</li>
          {% endfor %}</ul></p>                 
        </p>
		    {% endfor %}
    
	  </td>
    </tr>
    {% endfor %}
  </tbody>
</table>
