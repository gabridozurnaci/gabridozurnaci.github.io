---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
city: Nürnberg
data:
- city: Nürnberg
  geo:
    lat: 49.4521
    lng: 11.0767
  restaurants:
  - name: Ishihara
    description: Euer Essen wird live vor euch zubereitet und direkt auf den Teller
      serviert.
    address: Schottengasse 3, 90402 Nürnberg
    phone: 0911 226395
    hours:
    - day: Montag – Samstag
      timings: 12:00 - 14:30, 18:00 - 22:00
    - day: Sonntag
      timings: Geschlossen
    website: http://ishihara.de
    location:
      lat: 49.448286
      lng: 11.0704377
    place_id: ChIJyWUwv6lXn0cRcHd8sVipExs
    yelp_id: ishihara-nürnberg
    review_id: NllMP9d_Ca4NnDCrT_laew
  - name: KomeKome
    description: Erfahrt hier eine authentische japanische Atmosphäre mit vielfältiger
      Auswahl von Ramen-Toppings.
    address: Kirchenweg 22, 90419 Nürnberg
    phone: 0911 37844615
    hours:
    - day: Montag
      timings: Geschlossen
    - day: Dienstag - Mittwoch
      timings: 17:30 - 21:30
    - day: Donnerstag—Samstag
      timings: 11:30 - 14:30, 17:30 - 23:00
    - day: Sonntag
      timings: 11:30 - 14:30, 17:30 - 21:30
    website: http://komekome.de
    location:
      lat: 49.4620021
      lng: 11.0667002
    place_id: ChIJh85yskxWn0cRu-kkxXHHvWQ
  - name: KOKORO
    description: Traditionell-japanische Küche mit modernem Ambiente.
    address: Luitpoldstraße 3, 90402 Nürnberg
    phone: 0911 66486801
    hours:
    - day: Montag – Freitag
      timings: 11:30 - 14:30, 17:30 - 22:30
    - day: Samstag – Sonntag
      timings: 12:00 - 15:00, 17:00 - 22:30
    website: http://www.kokororestaurant.de/
    location:
      lat: 49.4479556
      lng: 11.080299
    place_id: ChIJ-wX6IqdXn0cRK_3JfE1kBKQ
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
