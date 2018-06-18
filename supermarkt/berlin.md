---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Berlin?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Berlin. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Berlin
    shops:
        -
            name: 'Asia Markt Lee GmbH'
            address: 'Dircksenstraße 101-103, 10179 Berlin'
            hours: [{day: 'Montag - Samstag', timings: '9:00-20:00'}]
            phone: '030 84712697'
        -
            name: Asia-Markt
            address: 'Kopenhagener Str. 2, 10437'
            hours: [{day: 'Montag - Freitag', timings: '9:00-20:00'}, {day: Samstag, timings: '10:00-20:00'}]
            phone: '030 40504959'
        -
            name: 'Asia Mekong'
            address: 'Henriette-Herz-Platz 1, 10178 Berlin'
            hours: [{day: 'Montag - Samstag', timings: '10:00-20:00'}]
            phone: '030 2478282'
        -
            name: 'Go Asia'
            address: 'Turmstr. 29, 10551 Berlin'
            hours: [{day: 'Montag - Samstag', timings: '9:00-21:00'}]
            phone: '030 39882841'
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
Gönnt dich authentisches Ramen, <a href="/restaurants/berlin">Klick hier</a>.
