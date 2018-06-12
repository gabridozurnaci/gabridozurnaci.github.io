---
layout: post
title: "Ramen Restaurants überall in Deutschland"
description: "Instant Ramen haben inzwischen euer Herz erobert, doch ab und an müsst ihr auch mal das Original probieren. Daher sind hier unsere Top-Empfehlungen, was Restaurants in Deutschland betrifft."
icon: "assets/images/food.png"
categories: misc
city: Frankfurt
data:
- city: Frankfurt
  geo:
    lat: 50.1109
    lng: 8.6821
  restaurants:
  - name: Muku
    description: Japan in Frankfurt
    address: Dreieichstr. 7, 60594 Frankfurt am Main
    hours:
    - day: Dienstag - Freitag
      timings: 18:00-23:0
    - day: Samstag
      timings: 12:00-14:00, 18:00-23:00
    - day: Sonntag
      timings: 17:00 -21:00
    phone: 069 48445153
    website: http://www.muku-ramen.com
    location:
      lat: 50.106039
      lng: 8.692535
    place_id: ChIJVX6vAqAOvUcRe-zxKipNsAw
    yelp_id: ramen-muku-frankfurt-am-main
    review_id: 1PXwEOXQb9Y8U0JieyY1_Q
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
