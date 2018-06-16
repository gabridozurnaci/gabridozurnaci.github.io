---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Nürnberg?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Nürnberg. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Nürnberg
    shops:
        -
            name: 'Kajanas Asia Shop'
            address: 'Breitscheidstraße 19, 90459 Nürnberg'
            hours: [{day: 'Montag - Samstag', timings: '10:00-20:00'}]
            phone: '0911 49124'
        -
            name: 'Asia Shop Wing Fat'
            address: 'Sulzbacher Str. 97, 90489 Nürnberg'
            hours: [{day: 'Montag - Samstag', timings: '9:00-19:00'}]
            phone: '0911 5818925'
        -
            name: 'Asia Kauf-Center'
            address: 'Kirchenweg 19, 90419 Nürnberg'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0911 331920'
---
Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht. Scrollt doch einfach mal runter. 
<br />
<div id="outer_container">
<div id="restaurants">
   {%- for city in page.data -%}
  <h3>{{ city.city }}</h3>
  <ol>
    {%- for shop in city.shops -%}
      <li>
        <div class="restaurant_entry">
        <h4>{{ shop.name }}</h4>
        <p class="restaurant_address">Adresse: {{ shop.address }}</p>
        <p class="restaurant_hours"><u>Öffnungszeiten</u></p>
        <table class="hours">
        {%- for hour in shop.hours -%}
          <tr><td><p>{{ hour.day}}</p></td><td><p>{{ hour.timings }}</p></td></tr>
        {%- endfor -%}
        </table>        
        <p>Telefon: {{ shop.phone }}</p>
      </div>
      </li>
    {%- endfor -%}
  </ol>
  {%- endfor -%}
 </div>
</div>
