---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Bremen?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Bremen. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Bremen
    shops:
        -
            name: 'Hua Li Asia Supermarkt'
            address: 'Bahnhofstr. 10, 28195 Bremen'
            hours: [{day: 'Montag - Samstag', timings: '10:00-19:30'}]
            phone: '0412 24278668'
        -
            name: 'Asia Shopping Bremen - Dong Fang'
            address: 'Eher Heerstraße 68A, 28359 Bremen'
            hours: [{day: 'Montag - Freitag', timings: '10:00-18:30'}, {day: Samstag, timings: '10:00-16:00'}]
        -
            name: 'Asia Shop'
            address: 'Martinistraße  66, 28195 Bremen'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0421 1690917'
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
Gönnt dich authentisches Ramen, <a href="/restaurants">Klick hier</a>.