---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Frankfurt?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Frankfurt. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Frankfurt
    shops:
        -
            name: 'Asia Land'
            address: 'Hostatostraße 20, 65929 Frankfurt am Main'
            hours: [{day: 'Montag - Freitag', timings: '9:00-18:30'}, {day: Samstag, timings: '9:00-16:00'}]
            phone: '069 33008930'
        -
            name: 'YuanFa Asia Markt'
            address: 'Fahrgasse 90, 60311 Frabkfurt am Main'
            hours: [{day: 'Montag - Samstag', timings: '10:00-19:30'}]
            phone: '069 21938988'
        -
            name: Taisan
            address: 'Fahrgasse 95, 60311 Frankfurt am Main'
            hours: [{day: 'Montag - Samstag', timings: '10:00-19:00'}]
            phone: '069 291766'
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