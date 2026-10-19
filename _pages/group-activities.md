---
layout: archive
title: "Pictures from our group activities"
permalink: /group-activities/
author_profile: true
photos:
  - image: "MD03864.webp"
    preview: "MD03864.webp"
    caption: "IT:U Open Day · April 2026"
    width: 1200
    height: 1068
  - image: "acl2025-natural.webp"
    preview: "acl2025-natural.webp"
    caption: "ACL 2025 · July 2025"
    width: 1200
    height: 1045
  - image: "retreat1.webp"
    preview: "retreat1.webp"
    caption: "Research retreat in Speinshart with UTN’s NLLG lab · February 2026"
    width: 1200
    height: 851
  - image: "la-ruffa-2025-natural.webp"
    preview: "la-ruffa-2025-natural.webp"
    caption: "Group dinner at La Ruffa · August 2025"
    width: 1200
    height: 900
  - image: "retreat2.webp"
    preview: "retreat2.webp"
    caption: "Research retreat in Speinshart with UTN’s NLLG lab · February 2026"
    width: 803
    height: 1200
  - image: "20260220_103653.webp"
    preview: "20260220_103653.webp"
    caption: "A walk during the research retreat · February 2026"
    width: 676
    height: 1200
  - image: "Fei's visit.webp"
    preview: "Fei's visit.webp"
    caption: "Dinner during Prof Fei Xia’s visit · September 2026"
    width: 900
    height: 1200
  - image: "June 23 dinner at Mr. Wen copy.webp"
    preview: "June 23 dinner at Mr. Wen copy.webp"
    caption: "Dinner at Mr. Wen during Pinyao's visit · June 2025"
    width: 900
    height: 1200
---

{% include base_path %}

[← Back to team and mentoring]({{ base_path }}/mentoring/)

Conferences, visits, retreats, and meals together. Select a photo to view it full size.

<div class="group-activities-gallery">
  {% for photo in page.photos %}
  <figure class="group-activities-gallery__photo">
    <a class="image-popup" href="{{ base_path }}/images/group-activities-web/{{ photo.image | uri_escape }}" title="{{ photo.caption | escape }}">
      <img src="{{ base_path }}/images/group-activities-web/thumbnails/{{ photo.preview | uri_escape }}"
           width="{{ photo.width }}" height="{{ photo.height }}"
           loading="{% if forloop.first %}eager{% else %}lazy{% endif %}" decoding="async">
    </a>
    <figcaption>{{ photo.caption }}</figcaption>
  </figure>
  {% endfor %}
</div>
