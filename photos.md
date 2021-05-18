---
title: Photos
layout: page
---

<div class="row">
    {% for photoAlbum in site.data.photo-albums %}
    <div class="col-12 col-md-4">
        <div class="card mx-auto m-2">
            <img src="{{ photoAlbum.cover | prepend: "/assets/img/photos-gallery/" | relative_url}}" class="card-img-top" alt="{{ photoAlbum.title }}">
            <div class="card-body">
                <h5 class="card-title">{{ photoAlbum.title }}</h5>
                <a href="{{ photoAlbum.link }}" class="btn btn-primary" target="_blank">Go to Gallery</a>
            </div>
        </div>
    </div>
    {% endfor %}
</div>