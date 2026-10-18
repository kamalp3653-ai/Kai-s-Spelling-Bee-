<!doctype html>
<html lang="en">
<head>
<meta charset="utf-8">
<meta name="viewport" content="width=device-width, initial-scale=1">
<title>Spelling Bee: Word Champion</title>
<style>
:root{--bg:#101522;--panel:#1a2233;--panel2:#232e43;--text:#f5f7fb;--muted:#b8c3d8;--accent:#facc15;--good:#4ade80;--bad:#fb7185}
*{box-sizing:border-box}
body{margin:0;background:radial-gradient(circle at top,#253252 0,#101522 52%);color:var(--text);font-family:system-ui,-apple-system,Segoe UI,Roboto,Arial,sans-serif;min-height:100vh}
main{width:min(1050px,94vw);margin:0 auto;padding:28px 0 48px}
header{text-align:center;margin-bottom:22px}
h1{font-size:clamp(2rem,5vw,3.5rem);line-height:1.05;margin:0 0 8px;letter-spacing:-1.5px}
header p{margin:0;color:var(--muted)}
.panel{background:rgba(26,34,51,.96);border:1px solid #34415b;border-radius:20px;padding:22px;box-shadow:0 14px 40px #0003;margin-bottom:18px}
h2{margin:0 0 7px;font-size:1.35rem}
.small{color:var(--muted);font-size:.92rem;line-height:1.5}
.mode-grid{display:grid;grid-template-columns:repeat(auto-fit,minmax(190px,1fr));gap:12px;margin-top:17px}
.mode{color:#fff;border:0;border-radius:14px;padding:15px;text-align:left;cursor:pointer;min-height:100px;box-shadow:inset 0 -4px #0002;transition:transform .12s,filter .12s;font:inherit}
.mode:hover{transform:translateY(-2px);filter:brightness(1.08)}
.mode:focus-visible,button:focus-visible,input:focus-visible{outline:3px solid white;outline-offset:3px}
.mode strong{display:block;font-size:1.08rem;margin-bottom:5px}
.mode span{display:block;font-size:.84rem;line-height:1.35}
.beginner{background:#22a447}.novice{background:#76a817}.moderate{background:#b88b00}.advanced{background:#d65d0b}.expert{background:#d73545}.genius{background:#8b45c7}.master{background:#514dc4}.randomiser{background:#078ba9}.learn{background:#0e9b85}.charg{background:#d93688}
.hidden{display:none!important}
.stats{display:grid;grid-template-columns:repeat(4,1fr);gap:10px;margin:16px 0}
.stat{background:var(--panel2);border-radius:12px;padding:12px;text-align:center}
.stat label{display:block;color:var(--muted);font-size:.78rem}
.stat strong{font-size:1.4rem}
.game-top{display:flex;align-items:center;justify-content:space-between;gap:12px;flex-wrap:wrap}
.pill{background:#303c53;color:#e8eefc;border-radius:999px;padding:7px 11px;font-size:.85rem}
.word-area{text-align:center;padding:18px 0 10px}
.word-area .prompt{color:var(--muted);font-size:.92rem;margin-bottom:10px}
.word-area h2{font-size:clamp(1.5rem,4vw,2.3rem);overflow-wrap:anywhere}
input[type=text]{width:100%;background:#0e1421;border:2px solid #45536d;border-radius:12px;color:#fff;padding:15px 14px;font:inherit;font-size:1.05rem}
input[type=text]::placeholder{color:#7e8ba3}
.controls{display:flex;gap:10px;flex-wrap:wrap;margin-top:12px}
button.action{border:0;border-radius:10px;padding:11px 15px;font:inherit;font-weight:700;cursor:pointer;background:#e5eaf4;color:#152033}
button.action.primary{background:var(--accent);color:#211b00}
button.action.secondary{background:#34425b;color:#fff}
button.action.danger{background:#7f2939;color:#fff}
button:disabled{opacity:.45;cursor:not-allowed}
.feedback{min-height:27px;margin-top:12px;font-weight:700}
.feedback.good{color:var(--good)}.feedback.bad{color:var(--bad)}
.learn-box{background:#102d32;border:1px solid #1f7778;border-radius:12px;padding:14px;margin:12px 0}
.syllables{display:flex;gap:7px;flex-wrap:wrap;justify-content:center;margin:10px 0}
.syllable{background:#1a7778;padding:7px 10px;border-radius:8px;font-weight:800}
.footer-note{font-size:.82rem;color:var(--muted);margin-top:14px}
@media(max-width:600px){main{padding-top:18px}.panel{padding:16px}.stats{grid-template-columns:repeat(2,1fr)}.mode-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.mode{padding:12px;min-height:105px}}
</style>
</head>
<body>
<main>
<header>
<h1>🐝 Spelling Bee</h1>
<p>Listen closely. Spell boldly. Become the Word Champion.</p>
</header>

<section class="panel" id="menu">
<h2>Choose your mode</h2>
<p class="small">Pick a color-coded mode. Competition modes end after 3 mistakes; turn on Practice Mode to learn without strikes.</p>
<div class="mode-grid" id="modeGrid"></div>
<div class="controls">
<button class="action secondary" id="practiceToggle" aria-pressed="false">Practice Mode: OFF</button>
<button class="action secondary" id="soundToggle" aria-pressed="true">Sound Effects: ON</button>
</div>
<p class="footer-note">Your best scores are saved in this browser on this device. Words are spoken using your browser's built-in speech voice.</p>
</section>

<section class="panel hidden" id="game">
<div class="game-top">
<div><h2 id="modeTitle">Beginner</h2><div class="small" id="modeDescription"></div></div>
<span class="pill" id="roundLabel">Round 1</span>
</div>
<div class="stats">
<div class="stat"><label>Score</label><strong id="score">0</strong></div>
<div class="stat"><label>Streak</label><strong id="streak">0</strong></div>
<div class="stat"><label>Strikes</label><strong id="strikes">0 / 3</strong></div>
<div class="stat"><label>High score</label><strong id="highScore">0</strong></div>
</div>
<div class="word-area">
<div class="prompt" id="prompt">Listen to the word, then spell it below.</div>
<h2 id="wordStatus">🔊 Ready?</h2>
<button class="action secondary" id="speakBtn" type="button">🔊 Hear word again</button>
</div>
<form id="answerForm">
<label class="small" for="answer">Type the spelling</label>
<input id="answer" type="text" autocomplete="off" autocapitalize="off" spellcheck="false" placeholder="Type the word here…" required>
<div class="controls">
<button class="action primary" type="submit" id="submitBtn">Submit spelling</button>
<button class="action secondary" type="button" id="hintBtn">Get a hint</button>
<button class="action secondary" type="button" id="nextBtn">Next word</button>
<button class="action danger" type="button" id="menuBtn">Back to modes</button>
</div>
</form>
<div class="feedback" id="feedback" aria-live="polite"></div>
<div class="learn-box hidden" id="learnBox">
<strong>Learn it syllable by syllable</strong>
<p class="small" id="learnInstructions">Listen and practice each chunk.</p>
<div class="syllables" id="syllables"></div>
<div class="controls">
<button class="action secondary" id="prevSyllable" type="button">Previous chunk</button>
<button class="action primary" id="hearSyllable" type="button">Hear current chunk</button>
<button class="action secondary" id="nextSyllable" type="button">Next chunk</button>
</div>
</div>
<p class="footer-note" id="endNote"></p>
</section>
</main>

<script>
const CHARG = "Chargoggagoggmanchauggagoggchaubunagungamaugg";

const modes = [
{name:"Beginner",cls:"beginner",desc:"Friendly everyday words to get started."},
{name:"Novice",cls:"novice",desc:"A little trickier, but you’ve got this."},
{name:"Moderate",cls:"moderate",desc:"Watch those silent letters and tricky vowels."},
{name:"Advanced",cls:"advanced",desc:"Longer words and tougher spelling patterns."},
{name:"Expert",cls:"expert",desc:"Challenging vocabulary for serious spellers."},
{name:"Genius",cls:"genius",desc:"Rare words that test your word knowledge."},
{name:"Master",cls:"master",desc:"A big collection of difficult dictionary words."},
{name:"Randomiser",cls:"randomiser",desc:"A surprise word from any difficulty level."},
{name:"Learn",cls:"learn",desc:"Learn long words in chunks, syllable by syllable."},
{name:"Charg",cls:"charg",desc:"Chargoggagoggmanchauggagoggchaubunagungamaugg on repeat 🔥🔥🔥"}
];

const banks = {
Beginner:"apple|basket|bright|button|candle|captain|castle|cheese|chicken|cloud|corner|crayon|doctor|dragon|family|feather|garden|gentle|happen|jacket|kitten|little|market|monkey|morning|number|orange|pencil|picnic|planet|pocket|rabbit|rainbow|school|silver|sunshine|thunder|ticket|window|yellow".split("|"),

Novice:"adventure|alphabet|bicycle|calendar|careful|celebrate|chocolate|climate|complete|curious|delicious|different|dinosaur|discover|electric|excellent|favorite|February|football|generous|hospital|imagine|important|language|medicine|mystery|opposite|paragraph|popular|probably|remember|separate|surprise|tomorrow|triangle|umbrella|vacation|vegetable|whisper|yesterday".split("|"),

Moderate:"accommodate|achievement|amateur|awkward|boundary|category|conscience|definite|desperate|embarrass|environment|exaggerate|existence|familiar|foreign|government|guarantee|harass|immediately|independent|interrupt|leisure|maintenance|mischievous|necessary|occasion|privilege|pronunciation|recommend|restaurant|rhythm|secretary|sincerely|successful|temperature|threshold|twelfth|vacuum|weird|withhold".split("|"),

Advanced:"aberration|abstemious|anachronism|bellwether|capricious|circumlocution|conscientious|deleterious|desiccate|eclectic|effervescent|ephemeral|equanimity|idiosyncrasy|incontrovertible|indefatigable|ineffable|juxtaposition|magnanimous|onomatopoeia|ostensible|paradigm|perspicacious|pharaoh|quintessential|recalcitrant|sacrilegious|serendipity|surreptitious|vicissitude".split("|"),

Expert:"Acetylglucocoroglaucigenin|Acrocephalopolydactylousdysplasia|Adrenocorticotrophin|Anthropomorphisation|Antidisestablishmentarianism|Antixerophthalmic|Bourgeoisification|Bromochlorodifluoromethane|Canaliculodacryocystorhinostomy|Cholangiocholecystocholedochectomy|Cholangiopancreatography|Chondromyxohemangioendotheliosarcoma|Convolvulaceous|Corticopontocerebellar|Corynebacteriumpseudotuberculosis|Counterimmunoelectrophoresis|Dehydrothiotoluidine|Dermatofibrosarcomaprotuberans|Dextrodeorsumversion|Dichlorodiphenyltrichloroethane|Diisopropylfluorophosphate|Dermatofibrosislenticularisdisseminata|Dimethyldioctadecylammoniumchloride|Eellogofusciouhipoppokunurious|Encephalocraniocutaneouslipomatosis|Erythrocytapheresis|Esophagogastroduodenoscopy|Oesophagogastroduodenoscopy|Ferriprotoporphyrin|Floccinaucinihilipilification|Fluorotetraferriphlogopite|Fructosebisphosphatetriosephosphatelyase|Funkenzwangsvorstellung|Gastrocnemiosemimembranous|Gegenstandstheorie|Haematospectrophotometrically|Hexakosioihexekontahexaphobia|Hippopotomonstrosesquippedaliophobia|Honourificabilitudinity|Hexanitrohexaazatricyclododecanedione|Hypothalamicpituitaryadrenocortical|Immunoelectrochemiluminescence|Inositolphosphorylceramide|Laparohysterosalpingooophorectomy|Laryngotracheobronchitis|Loncastuximabtesirine|Lymphangioleiomyomatosis|Micropachycephalosaurus|Neohesperidindihydrochalcone|Nonanonacontanonactanonaliagon|Nucleotidylexotransferase|Orotatephosphoribosyltransferase|Otorhinolaryngological|Paroxysmalnocturnalhemoglobinuria|Percutaneousendoscopicgastrostomy|Photoplethysmography|Phosphorodiamidatemorpholinooligomer|Pneumoencephalography|Pneumonoultramicroscopicsilicovolcanoconiosis|Polyphiloprogenitive|Pseudopseudohypoparathyroidism|Pseudorhombicuboctahedron|Psychoneuroendocrinological|Psychophysicotherapeutics|Pyrrolizidinealkaloidosis|Ribulosebisphosphatecarboxylaseoxygenase|Scaphotrapeziotrapezoidosteoarthritis|Sclerectoiridectomy|Subacutesclerosingpanencephalitis|Spectrophotofluorometry|Sulfoquinovosyldiacylglycerol|Sphenopalatineganglioneuralgia|Sphygmomanometer|Stereoelectroencephalography|Supercalifragilisticexpialidocious|Thymicstromallymphopoietin|Thyroparathyroidectomy|Tonsillopharyngitis|Uridinediphosphateglycosyltransferase|Uvulopalatopharyngoplasty|Ventriculocisternostomy|Xanthogranulomatouspyelonephritis|Zoanthroprosopometamorphopsia".split("|"),

Genius:"antidisestablishmentarianism|floccinaucinihilipilification|pneumonoultramicroscopicsilicovolcanoconiosis|pseudopseudohypoparathyroidism|hippopotomonstrosesquippedaliophobia|incomprehensibility|uncharacteristically|disproportionableness|otorhinolaryngological|electroencephalography|intersubjectivity|counterrevolutionaries|institutionalization|indistinguishability|compartmentalization|unconstitutionality|deinstitutionalization|psychopharmacological|spectrophotometrically|thyroparathyroidectomy".split("|"),

Master:"Acetylglucocoroglaucigenin|Acrocephalopolydactylousdysplasia|Antidisestablishmentarianism|Canaliculodacryocystorhinostomy|Cholangiocholecystocholedochectomy|Chondromyxohemangioendotheliosarcoma|Counterimmunoelectrophoresis|Dermatofibrosarcomaprotuberans|Dimethyldioctadecylammoniumchloride|Encephalocraniocutaneouslipomatosis|Floccinaucinihilipilification|Fructosebisphosphatetriosephosphatelyase|Haematospectrophotometrically|Hexakosioihexekontahexaphobia|Hippopotomonstrosesquippedaliophobia|Immunoelectrochemiluminescence|Laparohysterosalpingooophorectomy|Lymphangioleiomyomatosis|Neohesperidindihydrochalcone|Nonanonacontanonactanonaliagon|Orotatephosphoribosyltransferase|Paroxysmalnocturnalhemoglobinuria|Phosphorodiamidatemorpholinooligomer|Pneumonoultramicroscopicsilicovolcanoconiosis|Pseudopseudohypoparathyroidism|Psychoneuroendocrinological|Ribulosebisphosphatecarboxylaseoxygenase|Scaphotrapeziotrapezoidosteoarthritis|Stereoelectroencephalography|Sulfoquinovosyldiacylglycerol|Uridinediphosphateglycosyltransferase|Xanthogranulomatouspyelonephritis|Zoanthroprosopometamorphopsia|sesquipedalian|antediluvian|defenestration|pulchritudinous|intransigence|obfuscation|perspicacious|recalcitrant|vicissitude|pusillanimous|logorrhea|lachrymose|synecdoche|chiaroscuro|appoggiatura|zeugma|callipygian|psammophile|zeugmatography".split("|")
};

const learnWords = [
"Antidisestablishmentarianism",
"Pneumonoultramicroscopicsilicovolcanoconiosis",
"Supercalifragilisticexpialidocious",
"Hippopotomonstrosesquippedaliophobia",
"Floccinaucinihilipilification",
"Pseudopseudohypoparathyroidism",
CHARG,
"Dichlorodiphenyltrichloroethane",
"Incomprehensibilities",
"Spectrophotofluorometrically",
"Acrocephalopolydactylousdysplasia",
"Canaliculodacryocystorhinostomy",
"Zoanthroprosopometamorphopsia"
];

const $ = id => document.getElementById(id);
let selectedMode="Beginner",practice=false,soundOn=true,currentWord="",score=0,streak=0,strikes=0,round=0,hintUsed=false,gameOver=false,usedWords=[],syllableParts=[],syllableIndex=0,randomDifficulty="Beginner",speakTimer=null;

function highKey(mode){return "spellingBeeHigh_"+mode}
function getHigh(mode){try{return Number(localStorage.getItem(highKey(mode))||0)}catch{return 0}}
function saveHigh(){
 if(practice)return getHigh(selectedMode);
 let old=getHigh(selectedMode);
 if(score>old){try{localStorage.setItem(highKey(selectedMode),String(score))}catch{}return score}
 return old;
}
function renderModes(){
 const grid=$("modeGrid");grid.innerHTML="";
 modes.forEach(m=>{
  const b=document.createElement("button");
  b.className="mode "+m.cls;
  const title=document.createElement("strong");title.textContent=m.name;
  const desc=document.createElement("span");desc.textContent=m.desc;
  b.append(title,desc);
  b.addEventListener("click",()=>startGame(m.name));
  grid.appendChild(b);
 });
}
function playTone(freq=600,duration=.09,type="sine"){
 if(!soundOn)return;
 try{
  const ctx=new(window.AudioContext||window.webkitAudioContext)();
  const osc=ctx.createOscillator(),gain=ctx.createGain();
  osc.type=type;osc.frequency.value=freq;gain.gain.value=.07;
  osc.connect(gain);gain.connect(ctx.destination);osc.start();
  gain.gain.exponentialRampToValueAtTime(.001,ctx.currentTime+duration);
  osc.stop(ctx.currentTime+duration);osc.onended=()=>ctx.close();
 }catch(e){}
}
function speak(text){
 if(!("speechSynthesis"in window)){setFeedback("Speech isn't supported in this browser. Try Chrome or Edge.",false);return}
 speechSynthesis.cancel();
 const u=new SpeechSynthesisUtterance(text);
 u.rate=selectedMode==="Learn"?.72:.88;u.pitch=1;u.lang="en-US";
 speechSynthesis.speak(u);
}
function chooseWord(){
 if(selectedMode==="Charg")return CHARG;
 if(selectedMode==="Learn")return learnWords[Math.floor(Math.random()*learnWords.length)];
 let bank;
 if(selectedMode==="Randomiser"){
  const names=["Beginner","Novice","Moderate","Advanced","Expert","Genius","Master"];
  randomDifficulty=names[Math.floor(Math.random()*names.length)];
  bank=banks[randomDifficulty];
  $("modeTitle").textContent="Randomiser — "+randomDifficulty;
 }else bank=banks[selectedMode]||banks.Beginner;
 let available=bank.filter(w=>!usedWords.includes(w.toLowerCase()));
 if(!available.length){usedWords=[];available=bank.slice()}
 const word=available[Math.floor(Math.random()*available.length)];
 usedWords.push(word.toLowerCase());
 return word;
}
function startGame(mode){
 if(speakTimer)clearTimeout(speakTimer);
 if("speechSynthesis"in window)speechSynthesis.cancel();
 selectedMode=mode;score=0;streak=0;strikes=0;round=0;usedWords=[];gameOver=false;
 $("nextBtn").textContent="Next word";
 $("menu").classList.add("hidden");$("game").classList.remove("hidden");
 $("modeTitle").textContent=mode;
 $("modeDescription").textContent=modes.find(m=>m.name===mode).desc;
 $("learnBox").classList.toggle("hidden",mode!=="Learn");
 $("endNote").textContent="";
 nextWord();
}
function updateStats(){
 $("score").textContent=score;
 $("streak").textContent=streak;
 $("strikes").textContent=practice?`${strikes} / ∞`:`${strikes} / 3`;
 $("highScore").textContent=getHigh(selectedMode);
 $("roundLabel").textContent="Round "+round;
}
function setFeedback(msg,good){
 $("feedback").textContent=msg;
 $("feedback").className="feedback "+(good?"good":"bad");
}
function nextWord(){
 if(gameOver)return;
 if(speakTimer)clearTimeout(speakTimer);
 currentWord=chooseWord();round++;hintUsed=false;
 $("answer").value="";$("answer").disabled=false;
 $("submitBtn").disabled=false;$("hintBtn").disabled=false;$("nextBtn").disabled=false;
 $("wordStatus").textContent="🔊 Listen and spell";
 $("prompt").textContent=selectedMode==="Learn"?"Learn the word in chunks, then spell the whole word.":"Listen to the word, then type its spelling.";
 $("feedback").textContent="";$("feedback").className="feedback";
 $("endNote").textContent="";
 if(selectedMode==="Learn"){
  syllableParts=splitSyllables(currentWord);syllableIndex=0;renderSyllables();
 }else $("syllables").innerHTML="";
 updateStats();
 speakTimer=setTimeout(()=>{if(!gameOver&&!$("game").classList.contains("hidden"))speak(currentWord)},250);
 $("answer").focus();
}
function normalize(s){return s.trim().toLocaleLowerCase().replace(/[\s'-]/g,"")}
function submitAnswer(ev){
 ev.preventDefault();
 if(gameOver)return;
 const answer=$("answer").value;
 if(!answer.trim()){setFeedback("Type your spelling first!",false);return}
 if(normalize(answer)===normalize(currentWord)){
  const points=Math.max(10,currentWord.length*2)+(streak>=2?streak*3:0)+(hintUsed?0:5);
  score+=points;streak++;
  saveHigh();playTone(850,.12);
  setFeedback(`Correct! +${points} points${streak>=3?" — "+streak+" word streak!":""}`,true);
  $("wordStatus").textContent="Correct!";
  $("endNote").textContent="The word was: "+currentWord;
  $("answer").disabled=true;$("submitBtn").disabled=true;$("hintBtn").disabled=true;
  updateStats();
 }else{
  streak=0;playTone(180,.18,"triangle");
  if(!practice){
   strikes++;
   setFeedback(`Not quite. The correct spelling is ${currentWord}.`,false);
  }else{
   setFeedback(`Not quite — Practice Mode has no strikes. Correct spelling: ${currentWord}.`,false);
  }
  $("wordStatus").textContent="Try the next word";
  $("answer").disabled=true;$("submitBtn").disabled=true;
  $("endNote").textContent="Correct spelling: "+currentWord;
  updateStats();
  if(!practice&&strikes>=3){
   gameOver=true;saveHigh();
   $("endNote").textContent=`GAME OVER! Final score: ${score}. The word was ${currentWord}.`;
   $("nextBtn").textContent="Play again";
   setFeedback("Three strikes! Game over.",false);
   $("answer").disabled=true;$("hintBtn").disabled=true;
  }
 }
}
function hint(){
 if(gameOver)return;
 hintUsed=true;
 const w=currentWord;
 if(selectedMode==="Learn"){
  setFeedback("Hint: practice the highlighted chunks below, one at a time.",true);
  return;
 }
 setFeedback(`Hint: ${w.length} letters. It starts with "${w.slice(0,Math.min(2,w.length))}" and ends with "${w.slice(-1)}".`,true);
 playTone(500,.08);
}
function splitSyllables(word){
 if(word===CHARG)return ["Char","gog","ga","gog","man","chau","gga","gog","chaub","u","na","gun","ga","maugg"];
 const chunks=word.match(/[^aeiouy]*[aeiouy]+(?:[^aeiouy](?![aeiouy]))?/gi)||[word];
 let out=chunks.flatMap(c=>c.length>8?c.match(/.{1,5}/g):[c]).filter(Boolean);
 if(out.join("").toLowerCase()!==word.toLowerCase())return word.match(/.{1,4}/g)||[word];
 return out;
}
function renderSyllables(){
 const holder=$("syllables");holder.innerHTML="";
 syllableParts.forEach((part,i)=>{
  const span=document.createElement("span");
  span.className="syllable";span.textContent=part;
  if(i===syllableIndex)span.style.outline="3px solid #facc15";
  holder.appendChild(span);
 });
 $("learnInstructions").textContent=`Chunk ${syllableIndex+1} of ${syllableParts.length}. Listen, say it, and practice the chunks together.`;
}
$("answerForm").addEventListener("submit",submitAnswer);
$("speakBtn").addEventListener("click",()=>speak(currentWord));
$("hintBtn").addEventListener("click",hint);
$("nextBtn").addEventListener("click",()=>{
 if(gameOver){startGame(selectedMode)}else nextWord();
});
$("menuBtn").addEventListener("click",()=>{
 if(speakTimer)clearTimeout(speakTimer);
 if("speechSynthesis"in window)speechSynthesis.cancel();
 $("game").classList.add("hidden");$("menu").classList.remove("hidden");
 gameOver=false;
});
$("practiceToggle").addEventListener("click",()=>{
 practice=!practice;
 $("practiceToggle").textContent="Practice Mode: "+(practice?"ON":"OFF");
 $("practiceToggle").setAttribute("aria-pressed",String(practice));
 $("practiceToggle").style.background=practice?"#4ade80":"";
 updateStats();
});
$("soundToggle").addEventListener("click",()=>{
 soundOn=!soundOn;
 $("soundToggle").textContent="Sound Effects: "+(soundOn?"ON":"OFF");
 $("soundToggle").setAttribute("aria-pressed",String(soundOn));
 $("soundToggle").style.background=soundOn?"":"#34425b";
});
$("prevSyllable").addEventListener("click",()=>{
 syllableIndex=Math.max(0,syllableIndex-1);renderSyllables();
});
$("nextSyllable").addEventListener("click",()=>{
 syllableIndex=Math.min(syllableParts.length-1,syllableIndex+1);renderSyllables();
});
$("hearSyllable").addEventListener("click",()=>speak(syllableParts[syllableIndex]||currentWord));
renderModes();
</script>
</body>
</html>
