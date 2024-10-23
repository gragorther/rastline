<script lang="ts">
	import Kartica from '$lib/kartica.svelte';
	import type { Opis } from '$lib/types';
	const opisi: Opis[] = [
		{
			name: 'Jabolko',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/3/35/Golden_delicious_apple.jpg/640px-Golden_delicious_apple.jpg',
			description:
				'Jabolko [jábou̯ko] je sadež, ki raste na drevesu jablani. Spada med kulturne rastline, ki jih je vzgojil človek s pomočjo križanja. Korenine jabolka izvirajo iz Azije. V Evropo je verjetno prispelo s trgovci. Obstaja več kot 7500 kultivarjev jabolk. Jabolko zraste iz pet-listnega cveta.'
		},
		{
			name: 'Hruška',
			image: 'https://upload.wikimedia.org/wikipedia/commons/c/cf/Pears.jpg',
			description:
				'Hruška (znanstveno ime Pyrus communis) je do 16 m visoko drevo s pokončnimi vejami. Deblo doseže do 60 cm premera, lubje ima sivkasto-rjave barve, skorja je razpokana, številne vejice - mladike imajo na koncu trnate zaključke. Listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi. Hruška spada v skupino pečkatih sadežev.'
		},
		{
			name: 'Kivi',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/d/de/Kiwifruit_cross_section.jpg/600px-Kiwifruit_cross_section.jpg',
			description:
				'Kivi (znanstveno ime Actinidia deliciosa) je do 10 m visoko drevo s pokončnimi vejami. Deblo doseže do 40 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		},
		{
			name: 'Banana',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/4/4c/Bananas.jpg/640px-Bananas.jpg',
			description:
				'Banana (znanstveno ime Musa acuminata) je do 10 m visoko drevo s pokončnimi vejami. Deblo doseže do 40 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		},
		{
			name: '3',
			image: 'https://i.pinimg.com/564x/a7/ff/a5/a7ffa5b022d9adde308bf924585075fa.jpg',
			description:
				'Število 3 je zelo zanimivo število, ki se pogosto pojavlja v matematiki, fiziki in filozofiji. V mnogih kulturah je tudi simbolno pomembno, saj predstavlja tridelnost, kot so tri dimenzije prostora, tri časa (preteklost, sedanjost, prihodnost) in tri aspekte človeka (telesnost, duhovnost, duševnost).'
		},
		{
			name: 'Mandarina',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/1/10/Citrus_reticulata_April_2013_Nordbaden.JPG/540px-Citrus_reticulata_April_2013_Nordbaden.JPG',
			description:
				'Mandarina (znanstveno ime Citrus reticulata) je do 10 m visoko drevo s pokončnimi vejami. Deblo doseže do 40 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		},
		{
			name: 'Limona',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/e/e4/P1030323.JPG/640px-P1030323.JPG',
			description:
				'Limona (znanstveno ime Citrus limon) je do 10 m visoko drevo s pokončnimi vejami. Deblo doseže do 40 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		},
		{
			name: 'Gorčica',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/c/c1/Senf-Variationen_edit.jpg/639px-Senf-Variationen_edit.jpg',
			description:
				'Gorčica (znanstveno ime Capsicum annuum) je do 1 m visoka rastlina s pokončnimi vejami. Deblo doseže do 10 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		},
		{
			name: 'Krompir',
			image:
				'https://upload.wikimedia.org/wikipedia/commons/thumb/c/c8/Potato_and_cross_section.jpg/640px-Potato_and_cross_section.jpg',
			description:
				'Krompir (znanstveno ime Solanum tuberosum) je do 1 m visoka rastlina s pokončnimi vejami. Deblo doseže do 10 cm premera, lubje ima sivkasto-rjave barve, skorja je gladka, listi so zgoraj gladki, temnozeleni, spodaj pa bledi, fino dlakavi.'
		}
	];
</script>

<h1 class="text-5xl">Rastline</h1>
<p>
	Rastlíne (znanstveno ime Plantae) so eno izmed kraljestev živih bitij, v katerega uvrščamo
	približno 300.000 danes znanih vrst. Skupina vključuje splošno razširjene in poznane življenjske
	oblike, kot so drevesa, cvetnice, trave, praprotnice in mahovi, izključuje pa rdeče in rjave alge,
	živali, glive, arheje ter bakterije. Za rastline je značilno, da razen izjem pridobivajo energijo
	za rast in delovanje organizma iz sončne svetlobe s pomočjo procesa fotosinteze, ki poteka v
	kloroplastih, poleg tega imajo njihove celice celične stene, grajene iz celuloze. Z rastlinami se
	znanstveno ukvarja botanika, ki je panoga biologije. V preteklosti so med rastline uvrščali tudi
	alge, glive in druge nesorodne avtotrofne organizme, to tradicijo botanika do neke mere ohranja še
	danes. Skupnosti vseh rastlin na določenem območju v določenem času pravimo flora.
</p>
<div class="grid grid-cols-3 font-black text-2xl p-5 rounded-2xl">
	{#each opisi as opis}
		<Kartica {opis}></Kartica>
	{/each}
</div>
