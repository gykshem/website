---
layout: page
headerimage: 'header_html-bilder.jpg'
title: Bilder
comments: true
---

##Visa bilder med HTML
<p class="preamble">För att visa en bild på hemsidan kräver det att bilden är av rätt filtyp. Det finns tre primära filtyper för bilder som används på webben, och det är JPG, GIF & PNG.</p>

För att hämta in en bild i HTML använder du dig av ``<img>`` och därefter ``src`` för att bestämma vilken bild.
{% highlight html %}

<img src="bild.jpg"/>

{% endhighlight %}



###Namnge bilden
Med hjälp av ``alt`` kan vi ge bilden en beskrivning som inte är synligt av ögat, utan används av sökmotorer och blinda som inte kan se vad bilden föreställer.

{% highlight html %}

<img src="bild.jpg" alt="En fågel"/>

{% endhighlight %}



###Visa bild från en annan mapp

Om bilden inte ligger i samma mapp som html-filen måste du länka den till rätt mapp. 

{% highlight html %}

<img src="/undermapp/bild.jpg"/> <!-- Hämtar bilden från undermapp -->

<img src="../bild.jpg"/> <!-- Hämtar bilden från övermapp -->

<img src="http://wdk.se/bild.jpg"/> <!-- Hämtar bilden från adress -->

{% endhighlight %}



###Ändra storlek på bilden
För att ändra storlek med hjälp av HTML så kan man använda ``width`` och ``height``.

{% highlight html %}

<img src="bild.jpg" width="100px"/>

{% endhighlight %}


<div class="note box">
Du får inte använda å, ä, ö, mellanrum eller konstiga tecken i bildens namn. Du får däremot använda bindestreck och understreck i filnamnet, så använd det istället för mellanrum.
</div>


<img src="{{ site.url }}/assets/images/asset_bilder-format.png" style="margin-top: 40px;"/>


##Skillnaden mellan JPG, GIF och PNG  

###JPG (Joint Photographic Experts Group)
JPG utvecklades av Joint Photographic Experts Group (JPEG) som en standard för fotografer. Det praktiska med JPG var att man kunde redusera bildens storlek genom att minska antalet pixelområden. Man kunde alltså dra ner på antalet färger som man behövde hämta i bilden och på så sätt dra ner på filstorleken.  

Det här gjorde att JPG blev ett populärt filformat på den tiden då uppkopplingen var som långsammast.

JPG passar däremot inte för grafisk design eller typografi, även en högupplöst JPG tappar kvallité och resulterar i dåliga pixlar på grafiska element.

<div class="success box no-margin">+ JPG passar för foton</div>  

<div class="note box no-margin">- JPG passar inte för grafisk design eller typografi</div>

###GIF (Graphics Interchange Format)
Precis som JPG så är GIF ett rätt så gammalt format. I grunden är GIF en 8-bitars färgfil, vilket betyder att den endast kan innehålla 256 färger. Skillnaden mellan GIF och JPG är att GIF har möjligheten att vara transparant och stödjer dessutom animationer.

GIF är däremot ett gammalt och begränsat filformat, och du bör inte använda det för foton eller grafisk design.

<div class="success box no-margin">+ GIF passar för animationer</div>

<div class="note box no-margin">- GIF passar inte för foton eller grafisk design</div>



###PNG (Portable Network Graphics)
PNG skapades som ett alternativ till GIF. Det har stöd för fler färger (24-bit) och klarar transparans mycket bättre. Det är det mest använda formatet idag på internet och perfekt för grafisk design och typografi.

<div class="success box no-margin">+ PNG passar för grafisk design och typografi</div>

<div class="note box no-margin">- PNG passar inte för stora foton</div>


<hr/>

<img src="{{ site.url }}/assets/images/asset_html-bild-exempel.jpg"/> 

##Spara bild för webben
<strong>Det är viktigt</strong> att optimera bilderna för webben. Du kan inte använda det där semesterfotot på 8 MB direkt på hemsidan. Då laddar hemsidan långsammare och besökaren tröttnar. Om man surfar över mobilt bredband vill man dessutom inte att hemsidan ska dra för mycket av månadens betalsurf.  

I Photoshop finns alternativet att spara för webben. Skillnaden mellan att spara för webben och spara en bild är att du kan komprimera ner bilden för att minska storleken om du sparar för webben. Om du använder ett annat bildhanteringsprogram kan den här funktionen se annorlunda ut.  



### *1* Öppna bild

Öppna din bild i bildhanteringsprogrammet <span class="keyboard">Ctrl/Cmd</span> + <span class="keyboard">O</span> och förminska bildstorleken med de verktyg som finns tillgängliga, i Photoshop kan du ändra bildstorleken under <strong>Image</strong> > <strong>Image Size</strong>. 



### *2* Spara för webben

Tryck sedan <span class="keyboard">Shift</span> + <span class="keyboard">Alt</span> + <span class="keyboard">Ctrl/Cmd</span> + <span class="keyboard">S</span> för att spara för webben.



### *3* Bestäm filtyp och kvallité 

<img src="{{ site.url }}/assets/images/asset_save-for-web-1.jpg"/>  

<img src="{{ site.url }}/assets/images/asset_save-for-web-2.jpg"/>  



### *4* Spara

<img src="{{ site.url }}/assets/images/asset_save-for-web-3.jpg"/>  

<img src="{{ site.url }}/assets/images/asset_save-for-web-4.jpg" style="margin-left: -13px;"/>  


<div class="success box">
<h3>Toppen!</h3>
<p>Nu vet du hur man sparar bilder och hämtar in dom på hemsidan.</p> 
</div>


<a class="btn btn-next" href="{{ site.url }}/webbdesign/html-listor/">Gå till nästa steg!</a>
