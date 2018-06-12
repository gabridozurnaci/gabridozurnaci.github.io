---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
data:
- city: Hamburg
  geo:
    lat: 53.5511
    lng: 9.9937
  restaurants:
  - name: Ramen Bar Zipang
    description: Sobald ihr den Laden betretet fühlt ihr euch als wärt ihr in Tokio.
    address: Eppendorfer Weg 62, 20259 Hamburg
    phone: 040 30703777
    hours:
    - day: Montag
      timings: Geschlossen
    - day: Dienstag - Sonntag
      timings: 18:00 - 22:00
    website: http://ramen-bar.de
    location:
      lat: 53.5726357
      lng: 9.960073999999999
    place_id: ChIJl8LFcVCPsUcRIo81qsooFVc
    yelp_id: ramen-bar-zipang-hamburg
    review_id: A1bdvT6TCIaNMmwmhqZxPA
  - name: MOMO Ramen
    description: Der einzige Ramenladen in der berühmten „Schanze“ - super lecker
      noch dazu.
    address: Margaretenstraße 58, 20357 Hamburg
    phone: 040 30703777
    hours:
    - day: Montag - Freitag
      timings: 18:00 - 22:00
    - day: Samstag & Sonntag
      timings: 13:00 - 22:00
    website: http://www.momo-ramen.de
    location:
      lat: 53.5662223
      lng: 9.9634776
    place_id: ChIJx152fUOPsUcRvzlmjNUp888
  - name: Kokomo Noodle Club
    description: Urbaner Look mit traditionellem Ambiente.
    address: Clemens-Schultz-Straße 41, 20359 Hamburg
    phone: 040 52155970
    hours:
    - day: Sonntag - Donnerstag
      timings: 12:00 - 22:00
    - day: Freitag & Samstag
      timings: 12:00 - 23:00
    website: http://www.momo-ramen.de
    location:
      lat: 53.5524882
      lng: 9.9623987
    place_id: ChIJF7eNfm6PsUcRXHAWR0B4S_g
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
