<!DOCTYPE html>
<html lang="cs">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Poznávačka – Ekologická olympiáda</title>
<style>
:root{
  --paper:#e7eae1;
  --card:#fbfbf7;
  --ink:#1b2a21;
  --ink-soft:#54685b;
  --line:#c3ccbd;
  --brass:#8a6a2f;
  --moss:#446b4e;
  --berry:#7c3b4c;
  --radius:3px;
}
*{box-sizing:border-box}
html,body{margin:0;padding:0}
body{
  background:var(--paper);
  color:var(--ink);
  font-family:ui-sans-serif,system-ui,"Segoe UI",Roboto,Helvetica,Arial,sans-serif;
  font-size:16px;
  line-height:1.5;
  -webkit-text-size-adjust:100%;
}
.wrap{max-width:900px;margin:0 auto;padding:18px 16px 64px}

/* ---------- hlavička ---------- */
header{border-bottom:2px solid var(--ink);padding-bottom:12px;margin-bottom:14px}
h1{
  font-family:Iowan Old Style,"Palatino Linotype",Palatino,Georgia,serif;
  font-size:1.6rem;font-weight:600;letter-spacing:-.01em;margin:0 0 2px;
}
.sub{color:var(--ink-soft);font-size:.86rem;margin:0}

/* ---------- ovládání ---------- */
.controls{display:flex;flex-wrap:wrap;gap:8px;align-items:center;margin-bottom:10px}
select,button{font:inherit;color:var(--ink)}
select{
  background:var(--card);border:1px solid var(--line);border-radius:var(--radius);
  padding:6px 8px;font-size:.88rem;
}
.btn{
  background:var(--card);border:1px solid var(--line);border-radius:var(--radius);
  padding:6px 12px;font-size:.88rem;cursor:pointer;
}
.btn:hover{border-color:var(--ink-soft)}
.btn:active{transform:translateY(1px)}
.btn.primary{background:var(--moss);border-color:var(--moss);color:#fff}
.btn.ghost{background:transparent}
:focus-visible{outline:2px solid var(--brass);outline-offset:2px}

.chips{display:flex;flex-wrap:wrap;gap:6px;margin-bottom:14px}
.chip{
  background:transparent;border:1px solid var(--line);border-radius:999px;
  padding:4px 11px;font-size:.8rem;cursor:pointer;color:var(--ink-soft);
}
.chip[aria-pressed="true"]{background:var(--ink);border-color:var(--ink);color:var(--paper)}

/* ---------- kartička ---------- */
.stage{perspective:1600px;margin-bottom:12px}
.card{
  position:relative;width:100%;aspect-ratio:3/4;max-height:70vh;
  transform-style:preserve-3d;transition:transform .5s cubic-bezier(.3,.8,.3,1);
  cursor:pointer;border:none;padding:0;background:none;display:block;
}
@media (min-width:640px){.card{aspect-ratio:4/3}}
.card.flipped{transform:rotateY(180deg)}
.face{
  position:absolute;inset:0;backface-visibility:hidden;-webkit-backface-visibility:hidden;
  background:var(--card);border:1px solid var(--line);border-radius:var(--radius);
  box-shadow:0 1px 0 var(--line);overflow:hidden;
  display:flex;flex-direction:column;align-items:center;justify-content:center;
}
.back{transform:rotateY(180deg);padding:24px;text-align:center;gap:10px}
.face img{width:100%;height:100%;object-fit:contain;background:#eceee8}
.num{
  position:absolute;top:8px;left:10px;font-size:.72rem;color:var(--ink-soft);
  background:rgba(251,251,247,.88);padding:1px 6px;border-radius:2px;
}
.hint{
  position:absolute;bottom:8px;left:0;right:0;text-align:center;
  font-size:.74rem;color:var(--ink-soft);
}
.loading,.failed{color:var(--ink-soft);font-size:.9rem;padding:24px;text-align:center}
.failed a{color:var(--moss)}

.cz{font-family:Iowan Old Style,"Palatino Linotype",Palatino,Georgia,serif;font-size:1.7rem;line-height:1.2;margin:0}
.lat{font-family:Iowan Old Style,"Palatino Linotype",Palatino,Georgia,serif;font-style:italic;color:var(--ink-soft);margin:0}
.grp{font-size:.78rem;color:var(--brass)}
.note{font-size:.8rem;color:var(--berry);max-width:34ch}

/* ---------- lišta pod kartou ---------- */
.nav{display:flex;align-items:center;justify-content:space-between;gap:10px}
.count{font-size:.84rem;color:var(--ink-soft);font-variant-numeric:tabular-nums}
.bar{height:2px;background:var(--line);margin:10px 0 4px}
.bar span{display:block;height:100%;background:var(--moss);transition:width .25s}

/* ---------- přehled ---------- */
.grid{display:grid;grid-template-columns:repeat(auto-fill,minmax(150px,1fr));gap:12px}
.tile{background:var(--card);border:1px solid var(--line);border-radius:var(--radius);overflow:hidden}
.tile .ph{aspect-ratio:1;background:#eceee8;display:flex;align-items:center;justify-content:center}
.tile img{width:100%;height:100%;object-fit:cover}
.tile .cap{padding:7px 9px}
.tile .cap b{font-family:Iowan Old Style,Georgia,serif;font-weight:600;font-size:.92rem;display:block}
.tile .cap i{color:var(--ink-soft);font-size:.78rem}

.tip{font-size:.8rem;color:var(--ink-soft);border-left:2px solid var(--brass);padding-left:10px;margin:16px 0}
.hidden{display:none}
@media (prefers-reduced-motion:reduce){.card{transition:none}}
</style>
</head>
<body>
<div class="wrap">

<header>
  <h1>Poznávačka</h1>
  <p class="sub">Ekologická olympiáda — národní kolo 2025 a 2022</p>
</header>

<div class="controls">
  <select id="setSel" aria-label="Sada">
    <option value="2025">2025 — národní kolo (120)</option>
    <option value="2022">2022 (121)</option>
    <option value="all">Obě sady dohromady</option>
  </select>
  <button class="btn" id="shuffleBtn">Zamíchat</button>
  <button class="btn" id="orderBtn">Podle čísla</button>
  <button class="btn ghost" id="viewBtn">Přehled všech</button>
</div>

<div class="chips" id="chips"></div>

<section id="cardView">
  <div class="stage">
    <button class="card" id="card" aria-label="Otočit kartičku">
      <div class="face front" id="front"></div>
      <div class="face back" id="back"></div>
    </button>
  </div>
  <div class="bar"><span id="progress"></span></div>
  <div class="nav">
    <button class="btn" id="prevBtn">← Zpět</button>
    <span class="count" id="count"></span>
    <button class="btn primary" id="nextBtn">Další →</button>
  </div>
  <p class="tip">Klikni na kartičku (nebo mezerník) pro otočení, šipkami se posouváš dál. Obrázky se stahují z Wikipedie a Wikimedia Commons, takže je potřeba připojení k internetu — a u podobných druhů si výsledek radši ověř.</p>
</section>

<section id="listView" class="hidden">
  <div class="grid" id="grid"></div>
</section>

</div>

<script>
/* ---------------- data ----------------
   c = český název, l = latinský, g = skupina, q = vlastní dotaz na Commons, n = poznámka */
const DATA = {
"2025":[
{c:"babočka admirál",l:"Vanessa atalanta",g:"Zoologie"},
{c:"mandelinka bramborová",l:"Leptinotarsa decemlineata",g:"Zoologie"},
{c:"srpice",l:"Mecoptera",g:"Zoologie",n:"stačí řád"},
{c:"vroubenka smrdutá",l:"Coreus marginatus",g:"Zoologie"},
{c:"vosík",l:"Polistes",g:"Zoologie",n:"stačí rod"},
{c:"vážka ploská",l:"Libellula depressa",g:"Zoologie"},
{c:"svižník polní",l:"Cicindela campestris",g:"Zoologie"},
{c:"dlouhososka",l:"Bombylella",g:"Zoologie",n:"stačí rod"},
{c:"martináč bukový",l:"Aglia tau",g:"Zoologie"},
{c:"saranče modrokřídlá",l:"Oedipoda caerulescens",g:"Zoologie"},
{c:"jepice",l:"Ephemera sp.",g:"Zoologie",q:"Ephemera danica",n:"stačí rod"},
{c:"babočka osiková",l:"Nymphalis antiopa",g:"Zoologie"},
{c:"střevlík kožitý",l:"Carabus coriaceus",g:"Zoologie"},
{c:"kněžice pásovaná",l:"Graphosoma italicum",g:"Zoologie"},
{c:"kovařík horský",l:"Ctenicera cuprea",g:"Zoologie"},
{c:"dlouhošíjka",l:"Phaeostigma",g:"Zoologie",q:"Phaeostigma notata",n:"stačí rod"},
{c:"kozlíček dazule",l:"Acanthocinus aedilis",g:"Zoologie",n:"tesařík 0,5 bodu"},
{c:"drvodělka",l:"Xylocopa",g:"Zoologie",q:"Xylocopa violacea",n:"stačí rod"},
{c:"cvrček polní",l:"Gryllus campestris",g:"Zoologie"},
{c:"slávička mnohotvárná",l:"Dreissena polymorpha",g:"Zoologie"},
{c:"paroh daňka evropského",l:"Dama dama",g:"Zoologie",q:"Dama dama antler",n:"poznává se paroh"},
{c:"lebka nutrie říční",l:"Myocastor coypus",g:"Zoologie",q:"Myocastor coypus skull",n:"poznává se lebka"},
{c:"lebka bobra evropského",l:"Castor fiber",g:"Zoologie",q:"Castor fiber skull",n:"poznává se lebka"},
{c:"lebka prasete divokého",l:"Sus scrofa",g:"Zoologie",q:"Sus scrofa skull",n:"poznává se lebka"},
{c:"lebka lasice kolčavy (lasičky)",l:"Mustela nivalis",g:"Zoologie",q:"Mustela nivalis skull",n:"poznává se lebka"},
{c:"lebka netopýra",l:"Chiroptera",g:"Zoologie",q:"bat skull Myotis",n:"poznává se lebka"},
{c:"lebka straky obecné",l:"Pica pica",g:"Zoologie",q:"Pica pica skull",n:"poznává se lebka"},
{c:"lebka křivky obecné",l:"Loxia curvirostra",g:"Zoologie",q:"Loxia curvirostra skull",n:"poznává se lebka"},
{c:"vejce kosa černého",l:"Turdus merula",g:"Zoologie",q:"Turdus merula egg",n:"poznává se vejce"},
{c:"vejce poštolky obecné",l:"Falco tinnunculus",g:"Zoologie",q:"Falco tinnunculus egg",n:"poznává se vejce"},
{c:"slepýš křehký",l:"Anguis fragilis",g:"Zoologie"},
{c:"bolen dravý",l:"Leuciscus aspius",g:"Zoologie"},
{c:"okoun říční",l:"Perca fluviatilis",g:"Zoologie"},
{c:"sumeček americký",l:"Ameiurus nebulosus",g:"Zoologie"},
{c:"vranka obecná",l:"Cottus gobio",g:"Zoologie"},
{c:"lasice hranostaj",l:"Mustela erminea",g:"Zoologie"},
{c:"myš domácí",l:"Mus musculus",g:"Zoologie"},
{c:"hryzec vodní",l:"Arvicola amphibius",g:"Zoologie"},
{c:"šakal obecný",l:"Canis aureus",g:"Zoologie"},
{c:"jelen sika",l:"Cervus nippon",g:"Zoologie"},
{c:"straka obecná",l:"Pica pica",g:"Zoologie",n:"poznává se i zvuk"},
{c:"puštík obecný",l:"Strix aluco",g:"Zoologie",n:"poznává se i zvuk"},
{c:"hýl obecný",l:"Pyrrhula pyrrhula",g:"Zoologie",n:"poznává se i zvuk"},
{c:"orel mořský",l:"Haliaeetus albicilla",g:"Zoologie",n:"poznává se i zvuk"},
{c:"datel černý",l:"Dryocopus martius",g:"Zoologie",n:"poznává se i zvuk"},
{c:"slavík obecný",l:"Luscinia megarhynchos",g:"Zoologie",n:"poznává se i zvuk"},
{c:"pěnkava obecná",l:"Fringilla coelebs",g:"Zoologie",n:"poznává se i zvuk"},
{c:"blatnice skvrnitá",l:"Pelobates fuscus",g:"Zoologie",n:"poznává se i zvuk"},
{c:"ropucha obecná",l:"Bufo bufo",g:"Zoologie",n:"poznává se i zvuk"},
{c:"rosnička zelená",l:"Hyla arborea",g:"Zoologie",n:"poznává se i zvuk"},
{c:"břečťan popínavý",l:"Hedera helix",g:"Botanika – les"},
{c:"šťavel kyselý",l:"Oxalis acetosella",g:"Botanika – les"},
{c:"jalovec obecný",l:"Juniperus communis",g:"Botanika – les"},
{c:"bříza bělokorá",l:"Betula pendula",g:"Botanika – les"},
{c:"modřín evropský (opadavý)",l:"Larix decidua",g:"Botanika – les"},
{c:"buk lesní",l:"Fagus sylvatica",g:"Botanika – les"},
{c:"vřes obecný",l:"Calluna vulgaris",g:"Botanika – les"},
{c:"trnka obecná",l:"Prunus spinosa",g:"Botanika – les"},
{c:"habr obecný",l:"Carpinus betulus",g:"Botanika – les"},
{c:"třešeň ptačí",l:"Prunus avium",g:"Botanika – les"},
{c:"kukuřice setá",l:"Zea mays",g:"Botanika – pole a rumiště"},
{c:"ježatka kuří noha",l:"Echinochloa crus-galli",g:"Botanika – pole a rumiště"},
{c:"laskavec ohnutý",l:"Amaranthus retroflexus",g:"Botanika – pole a rumiště"},
{c:"pýr plazivý",l:"Elytrigia repens",g:"Botanika – pole a rumiště"},
{c:"pryšec kolovratec",l:"Euphorbia helioscopia",g:"Botanika – pole a rumiště"},
{c:"merlík bílý",l:"Chenopodium album",g:"Botanika – pole a rumiště"},
{c:"pelyněk černobýl",l:"Artemisia vulgaris",g:"Botanika – pole a rumiště"},
{c:"vratič obecný (kopretina vratič)",l:"Tanacetum vulgare",g:"Botanika – pole a rumiště"},
{c:"třtina křovištní",l:"Calamagrostis epigejos",g:"Botanika – pole a rumiště"},
{c:"lnice květel",l:"Linaria vulgaris",g:"Botanika – pole a rumiště"},
{c:"dobromysl obecná",l:"Origanum vulgare",g:"Botanika – pole a rumiště"},
{c:"jetel rolní (zaječí)",l:"Trifolium arvense",g:"Botanika – louka"},
{c:"medyněk vlnatý",l:"Holcus lanatus",g:"Botanika – louka"},
{c:"psineček obecný",l:"Agrostis capillaris",g:"Botanika – louka"},
{c:"kozí brada luční",l:"Tragopogon pratensis",g:"Botanika – louka"},
{c:"pryšec tuhý",l:"Euphorbia stricta",g:"Botanika – louka",n:"v seznamu přepsáno jako „světlík tuhý“"},
{c:"bojínek luční",l:"Phleum pratense",g:"Botanika – louka"},
{c:"mrkev obecná",l:"Daucus carota",g:"Botanika – louka"},
{c:"topol osika",l:"Populus tremula",g:"Botanika – louka"},
{c:"chrpa luční",l:"Centaurea jacea",g:"Botanika – louka"},
{c:"hloh",l:"Crataegus sp.",g:"Botanika – louka",q:"Crataegus monogyna",n:"stačí rod"},
{c:"srha laločnatá (říznačka)",l:"Dactylis glomerata",g:"Botanika – louka"},
{c:"křídlatka česká",l:"Reynoutria ×bohemica",g:"Botanika – rybník"},
{c:"dvouzubec černavý",l:"Bidens frondosa",g:"Botanika – rybník"},
{c:"parožnatka – skleněnka",l:"Nitella flexilis",g:"Botanika – rybník"},
{c:"orobinec širokolistý",l:"Typha latifolia",g:"Botanika – rybník"},
{c:"vachta trojlistá",l:"Menyanthes trifoliata",g:"Botanika – rybník"},
{c:"šťovík přímořský",l:"Rumex maritimus",g:"Botanika – rybník"},
{c:"žabník jitrocelový",l:"Alisma plantago-aquatica",g:"Botanika – rybník"},
{c:"rdest kadeřavý",l:"Potamogeton crispus",g:"Botanika – rybník"},
{c:"rákos obecný",l:"Phragmites australis",g:"Botanika – rybník"},
{c:"bahnička vejčitá",l:"Eleocharis ovata",g:"Botanika – rybník"},
{c:"žebratka bahenní",l:"Hottonia palustris",g:"Botanika – rybník"},
{c:"ostřice šáchorovitá (česká)",l:"Carex bohemica",g:"Botanika – rybník"},
{c:"máta rolní",l:"Mentha arvensis",g:"Botanika – rybník"},
{c:"olše lepkavá",l:"Alnus glutinosa",g:"Botanika – rybník"},
{c:"růžkatec bradavčitý",l:"Ceratophyllum submersum",g:"Botanika – rybník"},
{c:"vrba křehká",l:"Salix euxina",g:"Botanika – rybník"},
{c:"závitka mnohokořenná",l:"Spirodela polyrhiza",g:"Botanika – rybník"},
{c:"netýkavka žláznatá",l:"Impatiens glandulifera",g:"Botanika – rybník"},
{c:"vápenec",l:"",g:"Geologie",q:"Limestone"},
{c:"obsidián",l:"",g:"Geologie",q:"Obsidian"},
{c:"slepenec",l:"",g:"Geologie",q:"Conglomerate rock"},
{c:"serpentinit (hadec)",l:"",g:"Geologie",q:"Serpentinite"},
{c:"pemza",l:"",g:"Geologie",q:"Pumice"},
{c:"pískovec",l:"",g:"Geologie",q:"Sandstone"},
{c:"magnetit",l:"",g:"Geologie",q:"Magnetite"},
{c:"baryt (těživec)",l:"",g:"Geologie",q:"Baryte"},
{c:"ametyst",l:"",g:"Geologie",q:"Amethyst"},
{c:"kalcit",l:"",g:"Geologie",q:"Calcite"},
{c:"muskovit (světlá slída)",l:"",g:"Geologie",q:"Muscovite"},
{c:"sádrovec",l:"",g:"Geologie",q:"Gypsum"},
{c:"grafit",l:"",g:"Geologie",q:"Graphite"},
{c:"pyrit",l:"",g:"Geologie",q:"Pyrite"},
{c:"galenit",l:"",g:"Geologie",q:"Galena"},
{c:"magnezit",l:"",g:"Geologie",q:"Magnesite"},
{c:"granát",l:"",g:"Geologie",q:"Garnet mineral"},
{c:"turmalín",l:"",g:"Geologie",q:"Tourmaline"},
{c:"chryzotil (azbest)",l:"",g:"Geologie",q:"Chrysotile"},
{c:"azurit",l:"",g:"Geologie",q:"Azurite"}
],
"2022":[
{c:"pestrokrovečník včelový",l:"Trichodes apiarius",g:"Brouci",n:"pestrokrovečníkovití (Cleridae)"},
{c:"smrtník věštivý",l:"Blaps mortisaga",g:"Brouci",n:"potemníkovití (Tenebrionidae)"},
{c:"střevlíček kovový",l:"Pterostichus burmeisteri",g:"Brouci",n:"střevlíkovití (Carabidae)"},
{c:"mrchožrout znamenaný",l:"Oiceoptoma thoracica",g:"Brouci",n:"mrchožroutovití (Silphidae)"},
{c:"kovařík červený",l:"Stenagostus rufus",g:"Brouci",n:"kovaříkovití (Elateridae)"},
{c:"klikoroh devětsilový",l:"Liparus glabrirostris",g:"Brouci",n:"nosatcovití (Curculionidae)"},
{c:"tesařík bukový",l:"Cerambyx scopolii",g:"Brouci",n:"tesaříkovití (Cerambycidae)"},
{c:"krasec lipový",l:"Lamprodila rutilans",g:"Brouci",n:"krascovití (Buprestidae)"},
{c:"chrobák velký",l:"Geotrupes stercorarius",g:"Brouci",n:"chrobákovití (Geotrupidae)"},
{c:"chroust obecný",l:"Melolontha melolontha",g:"Brouci",n:"vrubounovití (Scarabaeidae)"},
{c:"zlatohlávek zlatý",l:"Cetonia aurata",g:"Brouci",n:"zlatohlávkovití (Cetoniidae)"},
{c:"mandelinka topolová",l:"Chrysomela populi",g:"Brouci",n:"mandelinkovití (Chrysomelidae)"},
{c:"kornatec velký",l:"Peltis grossa",g:"Brouci",n:"kornatcovití (Trogossitidae)"},
{c:"drabčík císařský",l:"Staphylinus caesareus",g:"Brouci",n:"drabčíkovití (Staphylinidae)"},
{c:"kozlíček hnědý",l:"Dorcadion fulvum",g:"Brouci",n:"tesaříkovití (Cerambycidae)"},
{c:"světluška větší",l:"Lampyris noctiluca",g:"Brouci",n:"světluškovití (Lampyridae)"},
{c:"červotoč císařský",l:"Hedobia imperialis",g:"Brouci",n:"červotočovití (Anobiidae)"},
{c:"puchýřník Schaefferův",l:"Cerocoma schaefferi",g:"Brouci",n:"majkovití (Meloidae)"},
{c:"mršník topolový",l:"Hololepta plana",g:"Brouci",n:"mršníkovití (Histeridae)"},
{c:"vějířník nápadný",l:"Metoecus paradoxus",g:"Brouci",n:"vějířníkovití (Rhipiphoridae)"},
{c:"kuňka obecná",l:"Bombina bombina",g:"Živočichové"},
{c:"ještěrka obecná",l:"Lacerta agilis",g:"Živočichové"},
{c:"drop velký",l:"Otis tarda",g:"Živočichové"},
{c:"dytík úhorní",l:"Burhinus oedicnemus",g:"Živočichové"},
{c:"ostralka štíhlá",l:"Anas acuta",g:"Živočichové"},
{c:"puštík obecný",l:"Strix aluco",g:"Živočichové"},
{c:"želva bahenní",l:"Emys orbicularis",g:"Živočichové"},
{c:"ropucha obecná",l:"Bufo bufo",g:"Živočichové"},
{c:"užovka hladká",l:"Coronella austriaca",g:"Živočichové"},
{c:"skokan ostronosý",l:"Rana arvalis",g:"Živočichové"},
{c:"vrápenec velký",l:"Rhinolophus ferrumequinum",g:"Živočichové"},
{c:"šakal obecný",l:"Canis aureus",g:"Živočichové"},
{c:"plch zahradní",l:"Eliomys quercinus",g:"Živočichové"},
{c:"zubr evropský",l:"Bison bonasus",g:"Živočichové"},
{c:"rejsek obecný",l:"Sorex araneus",g:"Živočichové"},
{c:"ježek západní",l:"Erinaceus europaeus",g:"Živočichové"},
{c:"kuna lesní",l:"Martes martes",g:"Živočichové"},
{c:"hnízdo – moudiváček lužní",l:"Remiz pendulinus",g:"Pobytové stopy",q:"Remiz pendulinus nest",n:"poznává se hnízdo"},
{c:"hnízdo – straka obecná",l:"Pica pica",g:"Pobytové stopy",q:"Pica pica nest",n:"poznává se hnízdo"},
{c:"hnízdo – labuť velká",l:"Cygnus olor",g:"Pobytové stopy",q:"Cygnus olor nest",n:"poznává se hnízdo"},
{c:"hrad – bobr evropský",l:"Castor fiber",g:"Pobytové stopy",q:"beaver lodge Castor fiber",n:"poznává se hrad"},
{c:"stopa – sova",l:"Strigiformes",g:"Pobytové stopy",q:"owl footprint track snow",n:"poznává se stopa"},
{c:"stopa – vydra říční",l:"Lutra lutra",g:"Pobytové stopy",q:"Lutra lutra track footprint",n:"poznává se stopa"},
{c:"stopa – mýval severní",l:"Procyon lotor",g:"Pobytové stopy",q:"Procyon lotor track footprint",n:"poznává se stopa"},
{c:"lebka lišky obecné",l:"Vulpes vulpes",g:"Lebky",q:"Vulpes vulpes skull",n:"šelmy (Carnivora)"},
{c:"lebka kuny skalní",l:"Martes foina",g:"Lebky",q:"Martes foina skull",n:"šelmy (Carnivora)"},
{c:"lebka ježka východního",l:"Erinaceus roumanicus",g:"Lebky",q:"Erinaceus skull",n:"hmyzožravci (Erinaceomorpha)"},
{c:"lebka nutrie říční",l:"Myocastor coypus",g:"Lebky",q:"Myocastor coypus skull",n:"hlodavci (Rodentia)"},
{c:"lebka labutě velké",l:"Cygnus olor",g:"Lebky",q:"Cygnus olor skull",n:"vrubozobí (Anseriformes)"},
{c:"lebka prasete divokého",l:"Sus scrofa",g:"Lebky",q:"Sus scrofa skull",n:"sudokopytníci (Cetartiodactyla)"},
{c:"lípa malolistá (srdčitá)",l:"Tilia cordata",g:"Botanika – les"},
{c:"jeřáb ptačí",l:"Sorbus aucuparia",g:"Botanika – les"},
{c:"habr obecný",l:"Carpinus betulus",g:"Botanika – les"},
{c:"buk lesní",l:"Fagus sylvatica",g:"Botanika – les"},
{c:"jasan ztepilý",l:"Fraxinus excelsior",g:"Botanika – les"},
{c:"rokytník skvělý",l:"Hylocomium splendens",g:"Botanika – les"},
{c:"hvězdovka brvitá",l:"Geastrum fimbriatum",g:"Botanika – les"},
{c:"ryzec pravý",l:"Lactarius deliciosus",g:"Botanika – les"},
{c:"muchomůrka červená",l:"Amanita muscaria",g:"Botanika – les"},
{c:"hnojník inkoustový",l:"Coprinopsis atramentaria",g:"Botanika – les"},
{c:"břečťan popínavý",l:"Hedera helix",g:"Botanika – les"},
{c:"metlička křivolaká",l:"Avenella flexuosa",g:"Botanika – les"},
{c:"křídlatka česká",l:"Reynoutria ×bohemica",g:"Botanika – pole a rumiště"},
{c:"lopuch plstnatý",l:"Arctium tomentosum",g:"Botanika – pole a rumiště"},
{c:"vratič obecný (kopretina vratič)",l:"Tanacetum vulgare",g:"Botanika – pole a rumiště"},
{c:"laskavec ohnutý",l:"Amaranthus retroflexus",g:"Botanika – pole a rumiště"},
{c:"ježatka kuří noha",l:"Echinochloa crus-galli",g:"Botanika – pole a rumiště"},
{c:"zlatobýl kanadský",l:"Solidago canadensis",g:"Botanika – pole a rumiště"},
{c:"rdesno (truskavec) ptačí",l:"Polygonum aviculare",g:"Botanika – pole a rumiště"},
{c:"třtina křovištní",l:"Calamagrostis epigejos",g:"Botanika – pole a rumiště"},
{c:"hluchavka bílá",l:"Lamium album",g:"Botanika – pole a rumiště"},
{c:"pelyněk černobýl",l:"Artemisia vulgaris",g:"Botanika – pole a rumiště"},
{c:"pěťour maloúborný",l:"Galinsoga parviflora",g:"Botanika – pole a rumiště"},
{c:"pryšec kolovratec",l:"Euphorbia helioscopia",g:"Botanika – pole a rumiště"},
{c:"slepenec",l:"",g:"Geologie",q:"Conglomerate rock"},
{c:"brekcie (vulkanická)",l:"",g:"Geologie",q:"Volcanic breccia"},
{c:"granodiorit (granit, žula)",l:"",g:"Geologie",q:"Granodiorite"},
{c:"rohovec",l:"",g:"Geologie",q:"Chert",n:"pazourek 0,5 bodu"},
{c:"obsidián (vulkanické sklo)",l:"",g:"Geologie",q:"Obsidian"},
{c:"magnezit",l:"",g:"Geologie",q:"Magnesite"},
{c:"granát (almandin)",l:"",g:"Geologie",q:"Almandine",n:"ve svoru"},
{c:"biotit",l:"",g:"Geologie",q:"Biotite"},
{c:"sádrovec",l:"",g:"Geologie",q:"Gypsum"},
{c:"muskovit",l:"",g:"Geologie",q:"Muscovite",n:"světlá slída 0,5 bodu"},
{c:"ortoklas",l:"",g:"Geologie",q:"Orthoclase",n:"(draselný) živec 1 bod"},
{c:"kalcit",l:"",g:"Geologie",q:"Calcite"},
{c:"chryzotil",l:"",g:"Geologie",q:"Chrysotile",n:"azbest 1 bod"},
{c:"belemnit",l:"",g:"Geologie",q:"Belemnite fossil",n:"bonusová položka mimo soutěž"}
]
};
/* číslování podle originálního seznamu */
DATA["2025"].forEach((d,i)=>{d.i=i+1;d.set="2025"});
DATA["2022"].forEach((d,i)=>{d.i=i+1;d.set="2022";if(d.i>74)d.i=d.i+33}); // geologie 2022 začíná na 108

/* ---------------- stahování obrázků ---------------- */
const cache = new Map();
const BAD = /\.(svg|ogg|ogv|webm|pdf|tif|tiff|wav|mid)$/i;

async function j(url){
  const r = await fetch(url);
  if(!r.ok) throw new Error(r.status);
  return r.json();
}
async function wikiPageImage(lang,title){
  const d = await j(`https://${lang}.wikipedia.org/w/api.php?action=query&prop=pageimages&piprop=thumbnail&pithumbsize=900&redirects=1&format=json&origin=*&titles=${encodeURIComponent(title)}`);
  const p = d.query && d.query.pages;
  for(const k in p){ if(p[k].thumbnail && !BAD.test(p[k].thumbnail.source)) return p[k].thumbnail.source; }
  return null;
}
async function commons(query){
  const d = await j(`https://commons.wikimedia.org/w/api.php?action=query&generator=search&gsrnamespace=6&gsrlimit=8&prop=imageinfo&iiprop=url&iiurlwidth=900&format=json&origin=*&gsrsearch=${encodeURIComponent(query)}`);
  const p = d.query && d.query.pages;
  if(!p) return null;
  const arr = Object.values(p).sort((a,b)=>a.index-b.index);
  for(const it of arr){
    const info = it.imageinfo && it.imageinfo[0];
    if(info && !BAD.test(info.url)) return info.thumburl || info.url;
  }
  return null;
}
async function imageFor(card){
  const key = card.set+"-"+card.i;
  if(cache.has(key)) return cache.get(key);
  const latin = (card.l||"").replace(/ sp\.$/,"").replace("×","");
  let src = null;
  try{
    if(card.q){                                   // vlastní dotaz (lebky, stopy, horniny)
      src = await commons(card.q);
      if(!src && !card.l) src = await wikiPageImage("en", card.q);
    }
    if(!src && latin) src = await wikiPageImage("cs", latin);
    if(!src && latin) src = await wikiPageImage("en", latin);
    if(!src)          src = await wikiPageImage("cs", card.c);
    if(!src && latin) src = await commons(latin);
  }catch(e){}
  cache.set(key, src);
  return src;
}

/* ---------------- stav ---------------- */
let deck = [], idx = 0, flipped = false, shuffled = false, activeGroups = new Set(), listMode = false;

const $ = id => document.getElementById(id);

function pool(){
  const s = $("setSel").value;
  return s==="all" ? [...DATA["2025"], ...DATA["2022"]] : [...DATA[s]];
}
function groupsOf(arr){ return [...new Set(arr.map(d=>d.g))]; }

function renderChips(){
  const gs = groupsOf(pool());
  activeGroups = new Set(gs);
  $("chips").innerHTML = "";
  gs.forEach(g=>{
    const b = document.createElement("button");
    b.className="chip"; b.textContent=g; b.setAttribute("aria-pressed","true");
    b.onclick = ()=>{
      if(activeGroups.has(g) && activeGroups.size>1) activeGroups.delete(g); else activeGroups.add(g);
      b.setAttribute("aria-pressed", activeGroups.has(g));
      build();
    };
    $("chips").appendChild(b);
  });
}
function build(){
  deck = pool().filter(d=>activeGroups.has(d.g));
  if(shuffled) for(let i=deck.length-1;i>0;i--){const k=Math.floor(Math.random()*(i+1));[deck[i],deck[k]]=[deck[k],deck[i]]}
  idx = 0; flipped = false;
  listMode ? renderList() : show();
}

/* ---------------- kartička ---------------- */
async function show(){
  const card = deck[idx];
  $("card").classList.toggle("flipped", flipped);
  $("count").textContent = deck.length ? `${idx+1} / ${deck.length}` : "—";
  $("progress").style.width = deck.length ? ((idx+1)/deck.length*100)+"%" : "0";
  if(!card){ $("front").innerHTML='<p class="loading">Zapni aspoň jednu kategorii.</p>'; $("back").innerHTML=""; return; }

  $("back").innerHTML = `
    <p class="grp">${card.set} · č. ${card.i} · ${card.g}</p>
    <p class="cz">${card.c}</p>
    ${card.l?`<p class="lat">${card.l}</p>`:""}
    ${card.n?`<p class="note">${card.n}</p>`:""}`;

  $("front").innerHTML = `<span class="num">${card.set} · č. ${card.i}</span><p class="loading">Načítám obrázek…</p>`;
  const token = card;
  const src = await imageFor(card);
  if(deck[idx] !== token) return;
  if(src){
    $("front").innerHTML = `<img src="${src}" alt="">
      <span class="num">${card.set} · č. ${card.i}</span>
      ${card.n?`<span class="hint">${card.n}</span>`:""}`;
  }else{
    $("front").innerHTML = `<span class="num">${card.set} · č. ${card.i}</span>
      <p class="failed">Obrázek se nenašel.<br><a href="https://commons.wikimedia.org/w/index.php?search=${encodeURIComponent(card.q||card.l||card.c)}&title=Special:MediaSearch" target="_blank" rel="noopener">Hledat na Commons</a></p>`;
  }
}
function step(n){
  if(!deck.length) return;
  idx = (idx + n + deck.length) % deck.length;
  flipped = false;
  show();
}
function flip(){ flipped = !flipped; $("card").classList.toggle("flipped", flipped); }

/* ---------------- přehled ---------------- */
function renderList(){
  const g = $("grid"); g.innerHTML = "";
  deck.forEach(card=>{
    const t = document.createElement("div"); t.className="tile";
    t.innerHTML = `<div class="ph"></div><div class="cap"><b>${card.c}</b><i>${card.l||card.g}</i></div>`;
    g.appendChild(t);
    imageFor(card).then(src=>{ if(src) t.querySelector(".ph").innerHTML = `<img src="${src}" alt="" loading="lazy">`; });
  });
}

/* ---------------- události ---------------- */
$("card").onclick = flip;
$("nextBtn").onclick = ()=>step(1);
$("prevBtn").onclick = ()=>step(-1);
$("setSel").onchange = ()=>{ renderChips(); build(); };
$("shuffleBtn").onclick = ()=>{ shuffled = true; build(); };
$("orderBtn").onclick = ()=>{ shuffled = false; build(); };
$("viewBtn").onclick = ()=>{
  listMode = !listMode;
  $("cardView").classList.toggle("hidden", listMode);
  $("listView").classList.toggle("hidden", !listMode);
  $("viewBtn").textContent = listMode ? "Zpět na kartičky" : "Přehled všech";
  listMode ? renderList() : show();
};
document.addEventListener("keydown", e=>{
  if(listMode) return;
  if(e.key===" "||e.key==="Enter"){ e.preventDefault(); flip(); }
  if(e.key==="ArrowRight") step(1);
  if(e.key==="ArrowLeft") step(-1);
});

renderChips();
build();
</script>
</body>
</html>
