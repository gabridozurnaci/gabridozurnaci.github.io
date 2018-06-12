---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
city: Düsseldorf
data:
- city: Düsseldorf
  geo:
    lat: 51.2277
    lng: 6.7735
  restaurants:
  - name: Takumi
    description: "„Authentisch, Original und Japanisch.“"
    address: Immermannstraße 28, 40210 Düsseldorf
    hours:
    - day: Montag - Freitag
      timings: 11:30 -22:30
    - day: Samstag
      timings: 11:30 - 23:00
    - day: Sonntag
      timings: 11:30 -23:30
    phone: 0211 1793308
    website: http://brickny.com/takumi/
    location:
      lat: 51.2236278
      lng: 6.7889458
    place_id: ChIJObAKrTrKuEcR2fHGz5Flamk
    yelp_id: takumi-düsseldorf
    review_id: Sm0J8slLcs1l-YxjCdreVg
  - name: Naniwa Noodles & Soups
    address: Oststraße 55, 40211 Düsseldorf
    description: Die Schlange vor dem Laden könnte durchaus mal länger sein, allerdings
      hat das seine Gründe.
    hours:
    - day: Mittwoch - Montag
      timings: 11:30-21:30
    - day: Dienstag
      timings: Geschlossen
    phone: 0211 161799
    website: http://naniwa.de
    location:
      lat: 51.224989
      lng: 6.7881388
    place_id: ChIJzcysPyXKuEcRryf9mRF22L8
  - name: Takezo
    description: Ursprünglich ist die Kette „Takezo“ aus Japan. Also was könnte authentischer
      sein als das?
    address: Immermannstraße 48, 40210 Düsseldorf
    hours:
    - day: Mittwoch - Samstag
      timings: 12-00
    - day: So
      timings: 12:00-22:00
    phone: 0211 39022053
    website: http://takezo.de
    location:
      lat: 51.2227239
      lng: 6.7907183
    place_id: ChIJ2VP_EzDKuEcR8_TRK-uHG_Y
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
