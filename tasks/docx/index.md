---
layout: page
---

# Задания по Microsoft Word

<div id="accordion">
  {% for t in site.data.tasks.docx %}
  <div class="card">
    <div class="card-header" id="headingThree">
      <h5 class="mb-0">
        <button class="btn btn-link collapsed" data-toggle="collapse" data-target="#collapse{{forloop.index}}">
№{{forloop.index}} {{t.title}}
        </button>
      </h5>
    </div>
    <div id="collapse{{forloop.index}}" class="collapse" data-parent="#accordion">
      <div class="card-body">
<span>Файл:</span> <a href="{{t.file}}">скачать</a>

<div markdown="1">
{{t.description}}
</div>
</div>
  </div>
  {% endfor %} 
</div>