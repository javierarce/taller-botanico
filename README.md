# Taller botánico

### Tracery

- [Tracery](http://www.tracery.io)
- [Tutorial interactivo](http://www.crystalcodepalace.com/traceryTut.html)
- [Repositorio en GitHub](https://github.com/galaxykate/tracery)

### Cheap Bots, Done Quick!

- [Cheap Bots, Done Quick!](https://cheapbotsdonequick.com)

### Tracery


#### Gramática sencilla

```json
{
  "animal": ["unicorn", "raven", "sparrow"]
}

```

#### Anidamiento

```json
{
  "animal": ["unicorn", "raven", "sparrow"],
  "color": ["orange", "blue", "white"],   
  "sentence": ["The #color# #animal# is happy"]
}
```

#### Modificadores


#### .capitalize 

```json
{
  "objects": ["watch", "bike", "book"],
  "origin": "#objects.capitalize#"
} 
```

#### .capitalizeAll 

```json
{
  "objects": ["watch", "bike", "book"],
  "origin": "#objects.capitalizeAll#"
}

```
#### .s 

```json
{
  "objects": ["watch", "bike", "book"],
  "origin": "#objects.s#"
}
```

#### .a 

```json
{
  "objects": ["book", "amplifier", "harp"],
  "origin": "#objects.a#"
}
```
#### .ed

```json
{
  "verbs": ["bounce", "walk", "buy"],
  "origin": "#objects.ed#"
}
```

#### .replace(x,y)

```json
{
  "objects": ["his watch", "his bike"],
  "origin": "#objects.replace(his, her)#"
}
```


#### Memoria

```json
{
  "objects": ["watch", "bike", "book"],
  "story": ["I want #object.a#, ok? #object.a#!"],
  "origin": ["#[object:#objects#]story#"]
}
```

#### Más difícil todavía

```json
{ 
  "name": ["Fox", "Jedoo"], 
  "story": ["#hero# was #occupation.a#. One day #pronoun# #action#."], 
  "setPronoun": ["[pronoun:she]", "[pronoun:he]"],
   "setOccupation": [ "[occupation:baker][action:baked, decorated cupcakes, iced a cake]", "[occupation:warrior][action:fought a monster, saved a village]"], 
  "origin": ["#[#setOccupation#][#setPronoun#][hero:#name#]story#"] 
}
```


### SVG

```json
{
  "story": "Texto {svg <svg>YOUR SVG CODE</svg>}"
}
```

```json
{ 
  "story": "Texto {svg <svg xmlns='http://www.w3.org/
           2000/svg' xmlns:xlink='http://www.w3.org/
           1999/xlink' width='1024' height='512'></
           svg>}" 
}
```

#### Imágenes

```js
<image width="540" height="380" xlink:href="URL" />
```

```json
{
  "image": ["url","url2", "url3"],
  "origin": "{svg <svg xmlns='http://www.w3.org/2000/svg' xmlns:xlink='http://www.w3.org/1999/xlink' 
   width='540' height='380'><image width='540' height='380' xlink:href='#image#' /></svg>}"
}
```
#### Texto 

```json
<text x="256" y="300" font-size="30" stroke="black" stroke-width="1" 
fill="white" text-anchor="middle" style="font-family: Impact">Mi texto</text>
```

#### Texto 

```json
<text x="256" y="300" font-size="30" stroke="black" stroke-width="1" fill="white"
text-anchor="middle" style="font-family: Roboto">Mi texto</text>
<style type=\"text/css\">@import url(https://fonts.googleapis.com/css?family=Roboto);</style>
</svg>
```

#### HTML 

```json
<foreignObject x='0' y='0' width='540' height='380'>
  <p xmlns='http://www.w3.org/1999/xhtml' style='width: 100%; color: white; background: black; padding: 20px; margin: 0; font-size:24px;'>
    Hola <strong>mundo</strong>
  </p>
</foreignObject>
```

#### JavaScript 

```json
<foreignObject x='0' y='0' width='540' height='380'> 
  <div xmlns='http://www.w3.org/1999/xhtml'id='date'></div> 
  <script>   
    document.getElementById('date')[0].innerHTML = new Date(); 
  </script> 
</foreignObject>
```




### Etiqueta

– Don’t @mention people who haven’t opted in.  
– Don’t follow Twitter users who haven’t opted in.  
– Don’t use a pre-existing hashtag.  
– Don’t go over your rate limits.  

Fuente: [Basic Twitter bot etiquette, Darius Kazemi](http://tinysubversions.com/2013/03/basic-twitter-bot-etiquette).

---

### Recursos

#### Texto
- [Corpora](http://github.com/dariusk/corpora)
- [Artículo aleatorio de la Wikipedia](http://en.wikipedia.org/wiki/Special:Random)
- [Awesome Public Datasets](http://github.com/awesomedata/awesome-public-datasets)
- [Aesome JSON Datasets](http://github.com/jdorfman/Awesome-JSON-Datasets)
- [Cheap Markovs, Traced Quick!](http://github.com/serin-delaunay/cheapmarkovstracedquick)
- [Snowclones](http://snowclones.org)

#### Imágenes
- [New Yorker Random Cartoon](http://new-yorker-cartoon-url.glitch.me/image)
- [Unsplash Random Image](http://unsplash-proxy.glitch.me/random/1024x512?query=book)
- [The Cat API](http://thecatapi.com/api/images/get?format=src&type=jpg)
- [Lorem Flickr](http://loremflickr.com)
- [Picsum.photos](http://picsum.photos)

---

### Personas

#### Kate Compton / Galaxy Kate
- [www](http://www.galaxykate.com) [tw](https://twitter.com/GalaxyKate) [gh](https://github.com/galaxykate/tracery)

#### George Buckenham / v21
- [www](http://v21.io) [tw](https://twitter.com/v21) [gh](https://github.com/v21)

#### Darius Kazemi / tinysubversions
- [www](https://tinysubversions.com) [tw](https://twitter.com/tinysubversions) [gh](http://github.com/dariusk)


---

![Promo del taller](booots.gif)
