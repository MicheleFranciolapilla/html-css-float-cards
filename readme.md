# ESERCIZIO CON UTILIZZO DI FLOAT E CLEAR 

 ## Strumenti utilizzati：


- **Font google (Fredoka One):**

  Il font *`Fredoka One`* (lo stesso del mockup) viene utilizzato per tutti i testi della pagina web, ad eccezione del paragrafo presente nella sezione di testa **(scelta personale finalizzata a prendere sempre maggior confidenza con *html* e *css*)**, per il quale si utilizza il font di default, richiamato dal codice `.default_font{font-weight: 500; font-family: initial;}` all'interno del file *style.css*.
  
- **Variabili css:**

  Si è fatto uso di variabili all'interno del foglio di stile.
  Sono state usate variabili per settare i colori e tutti quegli attributi **(tra cui il `width` delle sezioni)** la cui rapida modifica puo′　tornare utile nel caso si voglia modificare qualcosa del layout della pagina.
```:root{
    --title_color: #E53170;
    --section_width: 70vw;
    --card_bkgrcolor: #0F0E17;
    --card_textcolor: #FFFFFE;
    --card_textcolor_hov: yellowgreen;
    --card_mailcolor: #6ECBDD;
    --card_mailcolor_hov: yellow;
    --card_bordercolor: rgba(146, 93, 225, 0.6);
    --card_margin: 2.5%;
}
```

- **Float e Clear annidati:**

Le singole cards si presentano come contenitori **(di classe clearfix)** dentro cui hanno posto una immagine ed una sezione dati (testuale + contatto mail), separate tra loro ed entrambe flottate **(di classe floater)**.
Le cards sono a loro volta flottate dentro la sezione, **(anch'essa di classe clearfix)**, secondo il seguente codice：

```
.floater{
    float: left;
}

.clearfix::after{
    content: "";
    display: table;
    clear: both;
}
```

- **Attributo MailTo:**

Mediante il codice `<a href="mailto:mail@dominio">mail@dominio</a> ` si ha accesso alla propria casella di posta elettronica con il campo destinatario gia' compilato.



- **Aggiunte extra:**

Oltre al gia' citato cambio di font, si sono aggiunti alcuni effetti visivi sulla card, con il selettore avanzato *:hover*.



---



