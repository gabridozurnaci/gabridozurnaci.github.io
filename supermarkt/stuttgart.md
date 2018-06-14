---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Stuttgart?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Stuttgart. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Stuttgart
    shops:
        -
            name: 'Trieu Asia Shop'
            address: 'Eberhardstraße 1, 70173 Stuttgart'
            hours: [{day: 'Montag - Samstag', timings: '9:30-20:00'}]
            phone: '0711 2486888'
        -
            name: 'Cash and Carry Asia Shop'
            address: 'Seyfferstraße 27, 70197 Stuttgart'
            hours: [{day: 'Montag - Samstag', timings: '8:30-20:00'}]
            phone: '0711 627279'
        -
            name: 'BETA Asia Supermarkt'
            address: 'Hedelfinger Str. 55, 70327 Stuttgart'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0711 22012734'
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
