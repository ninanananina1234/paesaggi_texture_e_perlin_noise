# Paesaggi, textures e Perlin Noise
Ricerca sul Perlin Noise, per il corso di Matematica per il Design (2025), Nina Pambianco e Yulia Dudina,  
docente Andreas Gysin, ISIA U  
https://ninanananina1234.github.io/paesaggi_texture_e_perlin_noise/

## Spiegazione Matematica

### Il Processo

<table style="width:100%; border-collapse: collapse;">
<tr>
<th style="border: 1px solid black; padding: 10px; text-align: center;">Processo 1D</th>
<th style="border: 1px solid black; padding: 10px; text-align: center;">Processo 2D</th>
</tr>
<tr>
<td style="border: 1px solid black; padding: 10px;">
1. Suddivisione della linea in segmenti e assegnazione di un valore casuale per ogni nodo, successivamente l'individuazione di un punto casuale all'interno del segmento. Vengono poi individuati 2 vettori offset ovvero i vettori che partono dai nodi e arrivano al punto casuale.
</td>
<td style="border: 1px solid black; padding: 10px;">
Nell'approccio a più dimensioni questo passaggio corrisponde alla suddivisione del piano in una griglia e all'assegnazione di un <a href="#" style="color: blue; text-decoration: none;" onmouseover="document.getElementById('img1').style.display='block'" onmouseout="document.getElementById('img1').style.display='none'">vettore gradiente</a> casuale per ogni nodo, successivamente l'individuazione di un punto casuale all'interno della cella. Vengono poi individuati 2n (n= numero dimensioni) <a href="#" style="color: blue; text-decoration: none;" onmouseover="document.getElementById('img2').style.display='block'" onmouseout="document.getElementById('img2').style.display='none'">vettori offset</a> overro i vettori che partono dai nodi e arrivano al punto casuale.
</td>
</tr>
<tr>
<td style="border: 1px solid black; padding: 10px;">
2. Calcolo del <a href="#" style="color: blue; text-decoration: none;" onmouseover="document.getElementById('img3').style.display='block'" onmouseout="document.getElementById('img3').style.display='none'">prodotto scalare</a> tra il valore casuale e il vettore offset.
</td>
<td style="border: 1px solid black; padding: 10px;">
(Nell'approccio a più dimensioni questo passaggio corrisponde al prodotto scalare tra il vettore gradiente e il vettore offset).
</td>
</tr>
<tr>
<td style="border: 1px solid black; padding: 10px;">
3. Interpolazione dei valori ottenuti per ottenere un valore finale.
</td>
<td style="border: 1px solid black; padding: 10px;">
Nell'approccio a più dimensioni questo passaggio avviene <a href="#" style="color: blue; text-decoration: none;" onmouseover="document.getElementById('img4').style.display='block'" onmouseout="document.getElementById('img4').style.display='none'">nello stesso modo</a>.
</td>
</tr>
</table>

<div id="img1" style="display: none; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 1000;">
<img src="2.jpg" style="max-width: 300px;">
</div>

<div id="img2" style="display: none; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 1000;">
<img src="Perlin_Noise_2-15.png" style="max-width: 300px;">
</div>

<div id="img3" style="display: none; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 1000;">
<img src="Perlin_Noise_2-14.png" style="max-width: 300px;"><br>
<img src="PerlinNoiseDotProducts.png" style="max-width: 300px;">
</div>

<div id="img4" style="display: none; position: fixed; top: 50%; left: 50%; transform: translate(-50%, -50%); z-index: 1000;">
<img src="PerlinNoiseInterpolated.png" style="max-width: 300px;">
</div>

