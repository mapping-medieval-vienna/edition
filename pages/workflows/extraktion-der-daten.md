# Extraktion der Daten

TODO: aktualisieren und vervollständigen

zum Beispiel wird `<seg>` nicht mehr verwendet 

## Ortsangaben

## Datumsangaben

## Umwandlung des Formulars in TEI

Der Text soll trotz der zugefügten Information lesbar bleiben. Gleichzeitig soll die Nomenklatur nicht TEI durch die Hintertür neu erfinden. Für die Anzeige der Edition muss der Text in TEI umgewandelt werden. Das passiert auf Knopfdruck mit einem Skript. 

Für die Anzeige wird die zeilengetreue Version und die Formular-Version mit einem Skript zu einer TEI-konformen Version zusammengebracht. Das sieht dann (zurzeit) so aus:

zeilengetreu:
```
<seg><rs type="von">Als daz von Hansen <lb facs="#facs_371_r2l8" n="N007"/>Scharffenperger</rs> 
<measure type="preis" commodity="101 tl.">umb hundert und ain phunt d.</measure> 
<rs type="ereignis" ref="#kauf">mit kauf an Sy <lb facs="#facs_371_r2l9" n="N008"/>komen ist</rs></seg> 
```

(`@commodity` ist eine nicht vorgesehene Verwendung dieses Attributs, aber wir haben noch kein eigenes MMV-spezifisches Attribut definiert.)

Formular:
```
<ab type="formular">
Ⓥ<rs type="von">Agnes von Lincz</rs>
verkaufⒺ<rs type="ereignis">hat verkaufft</rs>
<lb/>
DB0001Ⓞ<rs type="objekt">ain haus</rs>
Neulucke, vor WidmertorⓁ<rs type="lage">gelegen vor Widmertor ze Wienn</rs>
DB0002Ⓝ<rs type="neben">zenegst Jacobin der Paugkerin haus</rs>
<lb/>
24 tl.Ⓟ<measure type="preis">umb vier und zwainczig phunt Wienner phenning</measure>
Ⓐ<rs type="an">dem erbern mann Veiten dem Valkchner und frawn Barbaren seiner hausfrawn</rs>
<lb/>
<rs>und ir baider erben
<lb/>furbaser ledichlich und freileich zehaben und allen irn frumen damit zeschaffen</rs>
<lb/>
<rs>ut littera sonat</rs>
1422-08-21 / Freitag vor Bartholomäus (Mo 24.8.)Ⓓ<date>Actum an Freitag vor Bartholomei Anno domini Mº ccccº xxiiº</date>
48 d.ⓟ<measure type="gebühr">Summa xlviii d.</measure>
</ab>
```

