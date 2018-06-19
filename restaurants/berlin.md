---
layout: post
title: "Ramen Restaurants überall in Berlin"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Berlin betrifft."
icon: "assets/images/food.png"
categories: misc
city: Berlin
data:
- city: Berlin
  geo:
    lat: 52.52
    lng: 13.405
  restaurants:
  - name: Cocolo Ramen X-berg
    description: Hier findet ihr viel Auswahl und Variationen, wenn es um Ramen geht
      - ein sehr
    address: Paul-Lincke-Ufer 39-40, 10999 Berlin
    hours:
    - day: Montag - Samstag
      timings: 12:00 - 23:00
    phone: 030 98339073
    location:
      lat: 52.4966706
      lng: 13.4225608
    place_id: ChIJU2yw4MpPqEcR56FvelCSm5A
    yelp_id: cocolo-ramen-xberg-berlin
    review_id: _f3C6vcwRMadepqaKpz7GQ
  - name: Cocolo Ramen
    description: Die kleine Schwester von „Cocolo Ramen X-berg“.
    address: Gipsstraße 3, 10119 Berlin
    hours:
    - day: Montag - Samstag
      timings: 18:00 - 0:00
    - day: Sonntag
      timings: Geschlossen
    website: http://kuchi.de/
    location:
      lat: 52.5271819
      lng: 13.3993066
    place_id: ChIJ133InOZRqEcRyWmWgjkY6KE
  - name: Marubi Ramen Japanische & Shanghai Spezialitäten
    description: "„Marubi kocht absolut ohne Glutamat“, heisst es auf der offiziellen
      Website. Also wer darauf verzichten möchte, sollte dort unbedingt vorbeischauen."
    address: Schönhauser Alle 177, 10119 Berlin
    hours:
    - day: Montag - Samstag
      timings: 12:00 - 22:00
    - day: Sonntag
      timings: 17:00 - 22:00
    phone: 030 47378858
    website: http://marubi.eu/
    location:
      lat: 52.5314367
      lng: 13.4117509
    place_id: ChIJ0VYsVf1RqEcRyAPeG3I4iZk
  - name: Takumi NINE Sapporo
    description: Takumi sollte dem einem oder anderen Ramenliebhaber inzwischen bekannt
      sein. Dieser hier ist nur ein weiterer erfolgreicher Laden der Kette aus Düsseldorf.
    address: Chauseestr. 124, 10115 Berlin
    hours:
    - day: Montag - Freitag
      timings: 12:00 - 15:00, 18:00 - 23:00
    - day: Samstag & Sonntag
      timings: 13:00 - 22:00
    website: http://takumininberlin.de/
    location:
      lat: 52.5290334
      lng: 13.3846772
    place_id: ChIJv07Qh-tRqEcRdNC50ECvRWU
---
<p class="post_subtitle">{{ page.description }} </p>
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
Keine Zeit ins Restaurant zu gehen?  <a href="/supermarkt/berlin">Klick hier</a> für die Supermärkte überall Berlin!