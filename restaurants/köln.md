---
layout: post
title: "Ramen Restaurants überall in Köln"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Köln betrifft."
icon: "assets/images/food.png"
categories: misc
city: Köln
data:
- city: Köln
  geo:
    lat: 50.9375
    lng: 6.9603
  restaurants:
  - name: Tobioka
    description: Toller Service, umfangreiche Karte.
    address: Karolingerring 40, 50678 Köln
    phone: 0221 3489888
    hours:
    - day: Montag - Freitag
      timings: 12:00-14:30, 18:30-22:30
    - day: Samstag - Sonntag
      timings: 18:30-22:30
    website: http://www.tobioka.de/
    location:
      lat: 50.9222889
      lng: 6.9569319
    place_id: ChIJ2-YXBE8kv0cRujutw19YX88
    yelp_id: tobioka-köln
    review_id: NNi47ANc23wjN_1aFsTgfw
  - name: Shokudo Nudelhaus & Sushi
    description: So frisch und bekömmlich gibt es die im Umkreis sonst nirgendwo.
    address: Lützowstraße 41, 50674 Köln
    phone: 0221 2760188
    hours:
    - day: Montag - Samstag
      timings: 12:00-16:00, 17:00-23:00
    - day: Samstag - Sonntag
      timings: 15:00-23:00
    location:
      lat: 50.934015
      lng: 6.932429
    place_id: ChIJo1la8AIlv0cRNybnkiKfT8I
  - name: Restaurant NIKKO
    description: Gerichte aus frischen Zutaten, zubereitet nach den Techniken der
      traditionellen japanischen Küche
    address: Dürener Str. 89, 50931 Köln
    phone: 0221 4000094
    hours:
    - day: Montag - Freitag
      timings: 12:00 - 14:30,  18:30 - 22:30
    - day: Samstag - Sonntag & Freitag
      timings: 18.00 - 22:00
    website: http://nikko-koeln.de
    location:
      lat: 50.9325366
      lng: 6.921146299999999
    place_id: ChIJy34Y3uEkv0cR-BBGYwHGNBQ
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
