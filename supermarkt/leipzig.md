---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Leipzig?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Leipzig. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Leipzig
    shops:
        -
            name: 'Asia Bistro and Supermarkt'
            address: 'Hainstraße 4, 04109 Leipzig'
            hours: [{day: 'Montag - Samstag', timings: '9:30-20:00'}]
            phone: '0341 9939653'
        -
            name: 'Korea Markt'
            address: 'Eisenbahnstraße 17, 04315 Leipzig'
            hours: [{day: 'Montag - Samstag', timings: '10:30-20:00'}]
            phone: '0341 4686498'
        -
            name: 'Mekong Asiasupermarkt'
            address: 'Ritterstraße 44-48, 04109 Leipzig'
            hours: [{day: 'Montag - Samstag', timings: '9:30-20:00'}]
            phone: '0341 9610438'
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