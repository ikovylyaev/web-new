---
layout: default
permalink: /en/
---
<div class="container-fluid">
       <nav class="navbar navbar-expand navbar-light">
            <div class="navbar-brand"><img src="{{site.url}}/img/logo.svg" style="height: 100%; max-height: 40px; max-width: 20vw;" alt="ikovylyaev logo"></div>
        
              <div class="collapse navbar-collapse" id="main-nav">
                <ul class="navbar-nav me-auto" style="position: absolute; right: 0px;;">
                  <li class="nav-item">
                    <a class="nav-link" href="{{site.url}}">ru</a>
                  </li>
                  <li class="nav-item">
                    <a class="nav-link active" aria-current="page" href="{{site.url}}/en">en</a>
                  </li>
                </ul>
              </div>
          </nav>
        <h1 class="display-2" style="text-align: right; margin-top: 20vh; font-weight: 200!important;">ivan<br>kovylyaev</h1>
        {% for post in site.posts limit: 1 %}
            {% if post.type == 'design' %}
            {% if post.link == 'null' %}
                <a href="#">
            {% else %}
                <a target="blank" href="{{post.url}}">
            {% endif %}
            <div class="header-image" style="background: url({{site.url}}/img/bg/{{post.img}}.webp); background-size: cover; background-position: center;">
            </div>
            <h2 class="display-4" style="margin-top: 20px;">{{ post.title }}</h2>
            <p>
                {% if post.concept == 'concept' %}
                 <span style="margin-right: 50px;">concept</span>
                {% endif %}
                <span>{{ post.categories }}</span>
            </p>
        </a>
        {%endif%}
        {% endfor %}
        <div class="row" style="margin-top: 10vh;">
            <div class="col-sm-12 col-md-5">
                <h2 class="display-4">about</h2>
            </div>
            <div class="col-sm-11 offset-sm-1 col-md-7 offset-md-0 mt-3">
                <p>i am ivan kovylyaev. freelance ui/ux and graphic designer from saint-petersburg, russia. currently working on greentech faculty of itmo university. if you want to work with me, please contact me by one of the links below.</p>
                <a href="https://disk.yandex.ru/i/N0AnN-6GTr-ttQ" style='margin-right: 50px;'>presentation</a>
            </div>
        </div>
        <div class="row" style="margin-top: 10vh;">
            {% for post in site.posts limit: 4 offset: 1 %}
            {% if post.type == 'design' %}
            {% if post.link == 'null' %}
                <div class="col-md-6 col-sm-12">
            {% else %}
                <a href="{{post.link}}" target="blank" class="col-md-6 col-sm-12">
            {% endif %}
                <img src="{{site.url}}/img/bg/{{post.img}}.webp" style="width: 100%;" alt="{{post.title}}">
                <h2 style="margin-top: 20px;">{{ post.title }}</h2>
                <p>
                {% if post.concept == 'concept' %}
                 <span style="margin-right: 50px;">concept</span>
                {% endif %}
                <span>{{ post.categories }}</span>
            </p>
            {% if post.link == 'null' %}
                </div>
            {% else %}
                </a>
            {% endif %}
            {%endif%}
            {% endfor %}
        </div>
        <div class="row" style="margin-top: 10vh;">
            <div class="col-sm-12 col-md-5">
                <h2 class="display-4">inventory</h2>
            </div>
            <div class="col-sm-11 offset-sm-1 col-md-7 offset-md-0 mt-3">
                <a href="https://drive.google.com/drive/folders/18AbQ0FsPcc2yzV1IkBHfUVSqIdPR6z-S?usp=sharing" target="blank">map of petersburg subway</a><br>
                <a href="https://drive.google.com/drive/folders/1F7pfxSSwSZ-sZ7Hl0UA8CyZafdK0g1N0?usp=sharing" target="blank">logo of petersburg subway</a><br>
            </div>
        </div>
        <div class="row" style="margin-top: 10vh;">
            {% for post in site.posts offset: 5 %}
            {% if post.type == 'design' %}
            {% if post.link == 'null' %}
                <div class="col-md-6 col-sm-12">
            {% else %}
                <a href="{{post.link}}" target="blank" class="col-md-6 col-sm-12">
            {% endif %}
                <img src="{{site.url}}/img/bg/{{post.img}}.webp" style="width: 100%;" alt="{{post.title}}">
                <h2 style="margin-top: 20px;">{{ post.title }}</h2>
                <p>
                {% if post.concept == 'concept' %}
                 <span style="margin-right: 50px;">concept</span>
                {% endif %}
                <span>{{ post.categories }}</span>
            </p>
            {% if post.link == 'null' %}
                </div>
            {% else %}
                </a>
            {% endif %}
            {%endif%}
            {% endfor %}
        </div>
        <div class="row" style="margin-top: 10vh;">
            <div class="col-sm-12 col-md-5">
                <h2 class="display-4">another projects</h2>
            </div>
            <div class="col-sm-11 offset-sm-1 col-md-7 offset-md-0 mt-3">
                <p><a href="http://video.ikovylyaev.com">photo and video</a></p>
                <p><a href="http://nature.ikovylyaev.com">ural</a></p>
                <p><a href="http://blog.ikovylyaev.com">blog (ru)</a></p>
            </div>
        </div>
        <div class="row" style="margin-top: 10vh;">
            <div class="col-sm-12 col-md-5">
                <h2 class="display-4">contacts</h2>
            </div>
            <div class="col-sm-11 offset-sm-1 col-md-7 offset-md-0 mt-3">
                <p><span style="opacity: 0.5; margin-right: 25px">mail</span><a href="mailto:hi@ikovylyaev.com">hi@ikovylyaev.com</a></p>
                <p><span style="opacity: 0.5; margin-right: 25px">behance</span><a href="https://behance.net/ikovylyaev">ikovylyaev</a></p>
                <p><span style="opacity: 0.5; margin-right: 25px">vk</span><a href="https://vk.com/ikovylyaev">ikovylyaev</a></p>
                <p><span style="opacity: 0.5; margin-right: 25px">instagram</span><a href="https://instagram.com/ikovylyaev">ikovylyaev</a></p>
                <p><span style="opacity: 0.5; margin-right: 25px">youtube</span><a href="https://www.youtube.com/channel/UCf9GOVc0qKKPB-Ee3LfH_uw">ivan kovylyaev</a></p>
            </div>
        </div>
        <div class="row" style="margin-top: 10vh;">
            <div class="col-sm-12 col-md-5">
                <h2 class="h1">legal information</h2>
            </div>
            <div class="col-sm-11 offset-sm-1 col-md-7 offset-md-0 mt-3">
                <p><a style="margin-right: 25px" href="{{ site.url }}/privacy/">privacy policy</a></p>
                <p><a style="margin-right: 25px" href="{{ site.url }}/terms/">terms of use</a></p>
                <p><a style="margin-right: 25px" href="{{ site.url }}/domain/">domain info</a></p>
            </div>
        </div>
    </div>
    
