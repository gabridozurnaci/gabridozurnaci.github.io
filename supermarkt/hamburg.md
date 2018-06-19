---
layout: post
title: "Wo kannst du Instant Ramen kaufen in Hamburg?"
description: "Du weißt nicht wo du deine zukünftigen Lieblingsramen findest? Wir haben euch asiatische Supermärkte mit den besten Bewertungen zusammengesucht in Hamburg. Scrollt doch einfach mal runter."
icon: "assets/images/001-bag.png"
categories: misc
data:
-
    city: Hamburg
    shops:
        -
            name: 'Vinh-Loi Asien Supermarkt'
            address: 'Klosterwall 2A, 20095 Hamburg'
            hours: [{day: 'Montag - Samstag', timings: '9:00-19:00'}]
            phone: '040 3258890'
        -
            name: 'Asia-Markt Lebensmittel und Geschenkartikel'
            address: 'Rosenstraße 2, 20095 Hamburg'
            hours: [{day: 'Montag - Samstag', timings: '10:00-19:00'}]
            phone: '040 324431'
        -
            name: 'Yuan Ye Markt'
            address: 'Bugenhagenstraße 5, 20096 Hamburg'
            hours: [{day: 'Montag - Samstag', timings: '9:30-20:00'}]
            phone: '040 30392120'
            Website: 'https://www.yuanye.de/'
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