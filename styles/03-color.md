---
layout: page
type: detail
title: Color
group: styles
permalink: /styles/color.html
description: Color styles define how color is used in the design system.

---

<!-- For inspiration, check out [Material Design's color styles page](https://material.io/guidelines/style/color.html).
 -->
<h2>Brand UI Color</h2>
<div class="square-color-scheme">
    {% for clr in site.colorsFirstRow %}
        <div style="background-color: {{ clr.color }};">
            <h5 class="{% if clr.label == 'PRIMARY VARIANT' or clr.label == 'SECONDARY VARIANT' or clr.label == 'SECONDARY' %} color-white {% endif %}">{{ clr.label }}</h5>
            <p class="{% if clr.label == 'PRIMARY VARIANT' or clr.label == 'SECONDARY VARIANT' or clr.label == 'SECONDARY' %} color-white {% endif %}">{{ clr.color }}</p>
        </div>
    {% endfor %}
</div>

<h2>Success Button Color</h2>
<div class="square-color-scheme">
    {% for clr in site.colorsButtonInfo %}
        <div style="background-color: {{ clr.color }};">
            <h5 class="{% if clr.label == 'STROKE' or clr.label == 'SECONDARY' or clr.label == 'PRIMARY' %} color-white {% endif %}">{{ clr.label }}</h5>
            <p class="{% if clr.label == 'STROKE' or clr.label == 'SECONDARY' or clr.label == 'PRIMARY' %} color-white {% endif %}">{{ clr.color }}</p>
        </div>
    {% endfor %}
</div>

<h2>Info Button Color</h2>
<div class="square-color-scheme">
    {% for clr in site.colorsButtonSuccess %}
        <div style="background-color: {{ clr.color }};">
            <h5 class="{% if clr.label == 'STROKE' or clr.label == 'SECONDARY' %} color-white {% endif %}">{{ clr.label }}</h5>
            <p class="{% if clr.label == 'STROKE' or clr.label == 'SECONDARY' %} color-white {% endif %}">{{ clr.color }}</p>
        </div>
    {% endfor %}
</div>