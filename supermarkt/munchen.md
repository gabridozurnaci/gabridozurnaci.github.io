---
layout: post
title: "Wo kannst du Instant Ramen kaufen in München?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in München. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: München
    shops:
        -
            name: i.Shop
            address: 'Prinzregentenstraße 120, 81677 München'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '089 62240036'
        -
            name: 'Asia Center'
            address: 'Friedenstraße 2, 81671 München'
            hours: [{day: 'Montag - Samstag', timings: '8:30-20:00'}]
            phone: '089 61372862'
        -
            name: 'Mekong Markt'
            address: 'Müllerstraße 34, 80469 München'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '089 26011738'
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