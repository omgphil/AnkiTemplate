## Front Template
```html
<div class=frontbg>
	{{Word}}
<br />
{{#Expression}}
<div class=hira>
{{furigana:Expression}}
</div>
{{/Expression}}

</div>
```

## Back Template
```html
<div class=frontbg>
	{{Word}}
</div>
<div class=backbg>
{{#Reading}}
	<div class="japanese">
		{{furigana:Reading}}
	</div>
{{/Reading}}
<div class="meaning">
 	{{hint:furigana:Meaning}}
</div>
<a class="hyper" href="https://jisho.org/search/{{text:Expression}}">Jisho</a>
|
<a class="hyper" href="https://jpdb.io/search?q={{text:Expression}}&lang=english#a">Jpdb.io</a>
</div>
```

## CSS Template
```css
@font-face {
  font-family: "Yu Mincho";
  src: url("_yumin.ttf") ;
}

@font-face {
  font-family: "Yu Mincho DemiBold";
  src: url("_yumindb.ttf") ;
}

.frontbg {
 background-color: #18adab;
 border-radius: 7px;
 color: #fff;
 position: relative;
 left: 0;
}

.card {
 font-family:Yu Mincho;
 font-size: 50px;
 text-align: center;
 color: black;
}

.android .card {
 font-family:Yu Mincho;
 font-size: 30px;
 text-align: center;
 color: black;
}

.frontbg {
 background-color: #18adab;
 border-radius: 7px;
 color: #fff;
 position: relative;
 left: 0;
}

.engdefbg {
 font-family: Raleway;
 font-style: italic;
 padding: 15px;
 margin-left: -5px;
 margin-top: -15px;
 color: #18adab;
 font-size: 15px;
}

.android .engdefbg {
 font-family: Raleway;
 font-style: italic;
 padding: 15px;
 margin-left: -15px;
 margin-top: -20px;
 color: #18adab;
 font-size: 10px;
}

.android .others {
 position: relative;
 top: 10px;
 border: 1px dotted #72c8e1;
 color: #18adab;
 font-size: 17px;
 width: auto;
 padding-top: 8px;
 padding-left: 15px;
 padding-bottom: 8px;
 padding-right: 15px;
 margin-bottom: 20px;
}


.backbg {
 position: relative;
 top: -3px;
 background-color: #fff;
 padding: 15px;
 padding-bottom: 15px;
 padding-left: 30px;
 padding-right: 30px;
 border-radius: 0px 0px 10px 10px; 
 color: #016ea6;
 font-size: 28px;
 text-align: left;
}

.android .backbg {
 position: relative;
 top: -5px;
 background-color: #fff;
 padding: 15px;
 padding-bottom: 15px;
 padding-left: 15px;
 padding-right: 15px;
 border-radius: 0px 0px 10px 10px; 
 color: #016ea6;
 font-size: 20px;
 text-align: left;
}

.hira {
 font-size: 25px;
 line-height: 5px;
 padding-bottom: 40px;
}

.android .hira {
 font-size: 18px;
 line-height: 5px;
 padding-bottom: 25px;
}

hr {
 height: 2px;
 font-size: 30px;
 border: 0;
 background: #72c8e1;
}

u {
 text-decoration: none;
 border-bottom: 1px dotted;
}


.japanese {
  font-size: 35px;
}

.meaning {
 position: relative;
}

.meaning::before {
    content: "";
    position: absolute;
    top: 50%;
    left: -15px;
    border-width: 10px;
    border-style: solid;
    border-color: transparent transparent transparent #72c8e1;
    transform: translateY(-50%);
}

b {
  font-family: "Yu Mincho DemiBold";
  color:#000;
}


```
