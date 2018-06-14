---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Köln?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Köln. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Köln
    shops:
        -
            name: 'Heng Long Asia Supermarkt'
            address: 'Aachener Str. 201-209, 50931 Köln'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0221 2828800'
        -
            name: 'Graces Asian Shop UG'
            address: 'Albertusstraße 7, 50667 Köln'
            hours: [{day: 'Montag - Samstag', timings: '12:00-16:00'}]
            phone: '0221 2574803'
        -
            name: 'Asia Markt Chhay Tri Long'
            address: 'Melatengürtel 22, 50933 Köln'
            hours: [{day: 'Montag - Samstag', timings: '10:00-19:00'}]
            phone: '0221 2406659'
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
