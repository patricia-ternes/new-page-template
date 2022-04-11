---
layout: page-fullwidth
permalink: /teaching/
title: "Teaching"
---

## Undergraduate Modules
During 2018 and 2019 I teaching undergraduate modules in Engineering Courses at the [Federal Institute Catarinense](https://ifc.edu.br/). Listed below are the modules I worked on each semester.
 
### 2019.2

|  Code   | Module                   | Course                             | Credits |
| :-----: | ------------------------ | ---------------------------------- | :-----: |
| CPA1404 | Experimental Physics I   | Computational Engineering          |   40    |
| ECA1410 | Experimental Physics II  | Control and Automation Engineering |   40    |
| CPA1416 | Experimental Physics III | Computational Engineering          |   40    |
| CPA1403 | Basic Physic I           | Computational Engineering          |   80    |
| ECA1409 | Basic Physic II          | Control and Automation Engineering |   80    |
| CPA1415 | Basic Physic III         | Computational Engineering          |   80    |

{% include _small-top-button.html %}

### 2019.1

|  Code   | Module                   | Course                             | Credits |
| :-----: | ------------------------ | ---------------------------------- | :-----: |
| ECA1404 | Experimental Physics I   | Control and Automation Engineering |   40    |
| CPA1409 | Experimental Physics II  | Computational Engineering          |   40    |
| ECA1418 | Experimental Physics III | Control and Automation Engineering |   40    |
| ECA1403 | Basic Physic I           | Control and Automation Engineering |   80    |
| CPA1408 | Basic Physic II          | Computational Engineering          |   80    |
| ECA1417 | Basic Physic III         | Control and Automation Engineering |   80    |

{% include _small-top-button.html %}

### 2018.2

|  Code   | Module                  | Course                             | Credits |
| :-----: | ----------------------- | ---------------------------------- | :-----: |
| CPA1404 | Experimental Physics I  | Computational Engineering          |   40    |
| ECA1410 | Experimental Physics II | Control and Automation Engineering |   40    |
| CPA1403 | Basic Physic I          | Computational Engineering          |   80    |
| ECA1409 | Basic Physic II         | Control and Automation Engineering |   80    |
| CPA1415 | Basic Physic III        | Computational Engineering          |   80    |

{% include _small-top-button.html %}

### 2018.1

|  Code   | Module                   | Course                             | Credits |
| :-----: | ------------------------ | ---------------------------------- | :-----: |
| ECA1404 | Experimental Physics I   | Control and Automation Engineering |   40    |
| CPA1409 | Experimental Physics II  | Computational Engineering          |   40    |
| ECA1418 | Experimental Physics III | Control and Automation Engineering |   40    |
| ECA1403 | Basic Physic I           | Control and Automation Engineering |   80    |
| CPA1408 | Basic Physic II          | Computational Engineering          |   80    |
| ECA1417 | Basic Physic III         | Control and Automation Engineering |   80    |

{% include _small-top-button.html %}

## Trainings

<div class="teaching-training">
    {% for training_item in site.data.trainings %}
        <h3>{{ training_item.title }}</h3>
        <div class="content">
            <span class="fas fa-calendar-alt r15"> </span>{{ training_item.date }}<br>
            Workshop content:
            {% for training_content in training_item.content %}
                <ul>
                    <li> {{ training_content }} </li>
                </ul>
            {% endfor %}
            {% if training_item.notes %}
            Workshop notes:
                {% for training_notes in training_item.notes %}
                <a href="{{ site.url }}{{ site.baseurl }}{{ training_notes }}"><span class="fas fa-file-alt l15 r15"> </span></a>
                {% endfor %}<br>
            {% endif %}
            {% if training_item.url %}
            <span class="fab fa-github-alt r15"></span><a href="{{ training_item.url }}">GitHub Page</a>
            {% endif %}
        </div>
        {% include _small-top-button.html %}
        <hr>
    {% endfor %}
</div>

## Internships

<div class="teaching-training">
    {% for internship_item in site.data.internships %}
        <h3>{{ internship_item.title }}</h3>
        <div class="content">
            <span class="fas fa-calendar-alt r15"> </span>{{ internship_item.date }}<br>
            <span class="fas fa-map-marker-alt r15"> </span>{{ internship_item.place }}<br>
            Main activities:
            {% for training_content in internship_item.content %}
                <ul>
                    <li> {{ training_content }} </li>
                </ul>
            {% endfor %}
            {% if internship_item.url %}
                <span class="fas fa-globe r15"></span><a href="{{ internship_item.url }}">Webpage</a>
            {% endif %}
        </div>
        {% include _small-top-button.html %}
        <hr>
    {% endfor %}
</div>
<i class=""></i>