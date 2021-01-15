<template>
    <div>
    <nav class="accordion arrows"><header class="box-header"></header><input type="radio" name="accordion" id="cb1"><section class="box"><label for="cb1" class="box-title">Anställda</label><label for="acc-close" class="box-close"></label><div class="box-content">Vad gäller anställda, dvs både stationära tjänstemän och bemanningskonsulter, så utgör <b>anställningsavtalet</b> laglig grund för den behandling Lernia behöver göra inom ramen för anställningen. Därför behöver normalt inget samtycke inhämtas.</div></section><input type="radio" name="accordion" id="cb2"><section class="box"><label for="cb2" class="box-title">Deltagare</label><label for="acc-close" class="box-close"></label><div class="box-content">För deltagare i våra utbildningar har Lernia flera olika lagliga grunder för olika behandlingar beroende på utbildningstyp, uppdragsgivare och hur vårt uppdrag ser ut. För hela utbildningsverksamheten som helhet baserar vi majoriteten av personuppgiftsbehandlingen på fyra olika lagliga grunder. Utförande av uppgift av <b>allmänt intresse</b> (tex anordna utbildning), Utförande som ett led i <b>myndighetsutövning</b> (tex betygssättning), <b>Rättslig förpliktelse</b> (t ex att följa skollagen och rapportera till uppdragsgivaren) och <b>Intresseavvägning</b>.
            <br><br>
            För att få skicka ut nyhetsbrev eller andra marknadsföringsutskick till deltagare krävs dock uttryckligt <b>samtycke</b>. Detta inhämtas i samband med första inloggningen på Mitt Lernia och det kan också lämnas vid senare tillfälle och tas tillbaka via Mitt Lernia. För fotografering av deltagare krävs också samtycke vilket i dagsläget inhämtas på papper när behov uppstår. Tänk på att samtycke alltid måste vara frivilligt och närsomhelst kunna tas tillbaka.</div></section><input type="radio" name="accordion" id="cb3"><section class="box"><label for="cb3" class="box-title">Kandidater</label><label for="acc-close" class="box-close"></label><div class="box-content">När en person söker arbete på eller genom Lernia så ingår de ett <b>Matchningsavtal för Lerniakandidater</b>. Detta avtal mellan kandidaten och Lernia, utgör laglig grund för behandling av kandidaternas personuppgifter inom ramen för vårt uppdrag att matcha kandidaten till passande jobb och arbetsgivarnas behov. För behandling av testresultat behövs dock separat samtycke vilket vi inhämtar med hjälp av de testföretag som används. Likaså krävs samtycke för spontana drogtester.</div></section><input type="radio" name="accordion" id="cb4"><section class="box"><label for="cb4" class="box-title">Kundkontaktpersoner</label><label for="acc-close" class="box-close"></label><div class="box-content">
För att kunna upprätthålla kundrelationer behandlar Lernia sedvanliga uppgifter om kunders kontaktpersoner. Detta gör vi baserat på <b>intresseavvägning</b>, dvs att Lernias intresse att behandla begränsade personuppgifter kopplat till personens yrkesroll, anses väga tyngre än kundkontaktpersonens intresse av att uppgifterna inte behandlas.</div></section><input type="radio" name="accordion" id="acc-close"></nav>
    </div>
</template>

<style>
.accordion {
	margin: auto;
	width: 100%;
}
.accordion input {
	display: none;
}
.box {
	position: relative;
	background: white;
    height: 64px;
    transition: all .15s ease-in-out;
}
.box::before {
    content: '';
    position: absolute;
    display: block;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    pointer-events: none;
    box-shadow: 0 -1px 0 #e5e5e5,0 0 2px rgba(0,0,0,.12),0 2px 4px rgba(0,0,0,.24);
}
header.box {
	background: #00BCD4;
	z-index: 100;
	cursor: initial;
	box-shadow: 0 -1px 0 #e5e5e5,0 0 2px -2px rgba(0,0,0,.12),0 2px 4px -4px rgba(0,0,0,.24);
}
header .box-title {
	margin: 0;
	font-weight: normal;
	font-size: 16pt;
	color: white;
	cursor: initial;
}
.box-title {
	width: calc(100% - 40px);
	height: 64px;
	line-height: 64px;
	padding: 0 20px;
	display: inline-block;
	cursor: pointer;
	-webkit-touch-callout: none;-webkit-user-select: none;-khtml-user-select: none;-moz-user-select: none;-ms-user-select: none;user-select: none;
}
.box-content {
	width: calc(100% - 40px);
	padding: 30px 20px;
	font-size: 11pt;
	color: rgba(0,0,0,.54);
	display: none;
}
.box-close {
	position: absolute;
	height: 64px;
	width: 100%;
	top: 0;
	left: 0;
	cursor: pointer;
	display: none;
}
input:checked + .box {
	height: auto;
	margin: 16px 0;
    box-shadow: 0 0 6px rgba(0,0,0,.16),0 6px 12px rgba(0,0,0,.32);
}
input:checked + .box .box-title {
	border-bottom: 1px solid rgba(0,0,0,.18);
}
input:checked + .box .box-content,
input:checked + .box .box-close {
	display: inline-block;
}
.arrows section .box-title {
	padding-left: 44px;
	width: calc(100% - 64px);
}
.arrows section .box-title:before {
	position: absolute;
	display: block;
	content: '\203a';
	font-size: 18pt;
	left: 20px;
	top: -2px;
	transition: transform .15s ease-in-out;
	color: rgba(0,0,0,.54);
}
input:checked + section.box .box-title:before {
	transform: rotate(90deg);
}

.infobild {
    vertical-align: middle;
    padding-bottom: 2px;
    padding-right: 6px;
}

</style>
