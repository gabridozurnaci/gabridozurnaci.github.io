---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Dortmund?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Dortmund. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Dortmund
    shops:
        -
            name: 'Tain Kim Heng'
            address: 'Hohe Str. 62, 44139 Dortmund'
            hours: [{day: 'Montag - Samstag', timings: '9:30-19:00'}]
            phone: '0231 95290488'
        -
            name: 'TTS Asien Supermarkt'
            address: 'Rheinische Str. 52, 44137 Dortmund'
            hours: [{day: 'Montag - Samstag', timings: '9:30-20:00'}]
            phone: '0231 819288'
        -
            name: 'Suresch Asiafrischmarkt'
            address: '6 Brüderweg, 44135 Dortmund'
            hours: [{day: 'Montag - Samstag', timings: '9:00-20:00'}]
            phone: '0231 551760'
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
Gönnt authentisches Ramen, <a href="/restaurants/dortmund">Klick hier</a>.