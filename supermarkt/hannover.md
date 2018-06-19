---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Hannover?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Hannover. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Hannover
    shops:
        -
            name: 'Asia Markt Kim-Thanh'
            address: 'Rundester. 6, 30161 Hannover'
            hours: [{day: 'Montag - Samstag', timings: '9:00-19:00'}]
            phone: '0511 3530837'
        -
            name: 'i.SHOP Feinkost aus Asien und aller Welt'
            address: 'Andreaestr. 8-9, 30159 Hannover'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0511 51949760'
        -
            name: 'Phungs Asia Shop'
            address: 'Varrelheide 190, 30657 Hannover'
            hours: [{day: 'Montag - Freitag', timings: '9:00-18:00'}, {day: Samstag, timings: '9:00-17:00'}]
            phone: '0511 3530562'
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
Gönnt authentisches Ramen, <a href="/restaurants">Klick hier</a>.