---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
city: Leipzig
data:
- city: Leipzig
  geo:
    lat: 51.3397
    lng: 12.3731
  restaurants:
  - name: KIRIGAMI Ramen Leipzig
    description: Vegetarisches Ramen? Kein Problem!
    address: Chopinstraße 15, 04103 Leipzig
    phone: 0341 68416888
    hours:
    - day: Montag - Freitag
      timings: 11:00-14:30, 17:30-21:00
    - day: Samstag
      timings: 17:30 - 22:00
    - day: Sonntag
      timings: Geschlossen
    website: http://www.kirigamileipzig.de/
    location:
      lat: 51.3435061
      lng: 12.3902639
    place_id: ChIJD1G-HRb4pkcRQRygYy5nPFI
    yelp_id: kirigami-ramen-leipzig
    review_id: IIZMJrjTUbDhqPSDsKbduA
  - name: Umai Ramen Bar
    description: Esst hier traditionelle Ramen in modernen Räumlichkeiten.
    address: Klostergasse 7-9, 04109 Leipzig
    phone: 0341 2222575
    hours:
    - day: Montag - Freitag
      timings: 12:00-22:00
    - day: Samstag
      timings: Geschlossen
    - day: Sonntag
      timings: 14:00 - 22:00
    website: http://umaii.de
    location:
      lat: 51.3406731
      lng: 12.3728297
    place_id: ChIJJbWcMCH4pkcRbKnHK6_TJOI
---
<p class="post_subtitle">Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft.</p>
<br />
<div id="outer_container">
<div id="restaurants">
   {%- for city in page.data -%}
  <h3>{{ city.city }}</h3>
  <ol>
    {%- for restaurant in city.restaurants -%}
      <li>
        <div class="restaurant_entry">
        <h4>{{ restaurant.name }}</h4>
        <p class="restaurant_description">{{ restaurant.description }}</p>
        <hr />
        <p class="restaurant_address">Adresse: {{ restaurant.address }}</p>
        <p>Telefon: {{ restaurant.phone }}</p>
        <p class="restaurant_hours"><u>Öffnungszeiten</u></p>
        <table class="hours">
        {%- for hour in restaurant.hours -%}
          <tr><td><p>{{ hour.day}}</p></td><td><p>{{ hour.timings }}</p></td></tr>
        {%- endfor -%}
        </table>
        <p class="restaurant_web">Website: <a href="{{ restaurant.website }}">{{ restaurant.website }}</a></p>
        </div>
        {% if restaurant.review_id %}
        <span class="yelp-review" data-review-id="{{restaurant.review_id}}" data-hostname="www.yelp.de"></span>   
        {% endif %}   
     </li>
    {%- endfor -%}
  </ol>
  {%- endfor -%}
 </div>
</div>
