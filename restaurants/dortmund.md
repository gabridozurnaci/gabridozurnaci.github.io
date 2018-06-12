---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
city: Dortmund
data:
- city: Dortmund
  geo:
    lat: 51.5136
    lng: 7.4653
  restaurants:
  - name: Restaurant Kyoto - Dortmund
    description: 'Sorgt euch nicht, wenn ihr keine Zeit habt: Hier werden die Ramen
      sogar vor eure Tür geliefert.'
    address: Rosental 9, 44135 Dortmund
    phone: 0231 5898400
    hours:
    - day: Montag - Donnerstag
      timings: 12:00 - 15:00, 17:00 - 22:30
    - day: Freitag
      timings: 12:00 - 15:00, 17:00 - 23:00
    - day: Samstag
      timings: 12:00 - 23:00
    - day: Sonntag
      timings: 12:00 - 21:30
    website: http://www.kyoto-dortmund.de/
    location:
      lat: 51.5136004
      lng: 7.4689236
    place_id: ChIJHRQ2Ol8XuUcR4aLOwsjF1LM
    yelp_id: kyoto-dortmund
    review_id: gSkm8DNnh0z7qX1OXPhy7Q
  - name: KimBaBBox
    description: 'Empfehlenswert: Nudelsuppe III mit Tofu, Algen, Möhren, Schnittlauch
      und Sesam, und Rinderhack.'
    address: Hohe Str. 57, 44139 Dortmund
    phone: 0231 47418418
    hours:
    - day: Montag - Freitag
      timings: 12:00 - 15:00, 16:30 - 21:00
    - day: Sonntag
      timings: 16:30 - 21:00
    location:
      lat: 51.5049195
      lng: 7.4590538
    place_id: ChIJB0iXsd4ZuUcRWpex_WRQZ2w
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
