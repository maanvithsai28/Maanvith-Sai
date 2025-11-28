<!DOCTYPE html>
<html lang="en">
<head>
<!-- Google tag (gtag.js) -->
<script async src="https://www.googletagmanager.com/gtag/js?id=G-499PR15CBC"></script>
<script>
  window.dataLayer = window.dataLayer || [];
  function gtag(){dataLayer.push(arguments);}
  gtag('js', new Date());

  gtag('config', 'G-499PR15CBC');
</script>
<meta charset="UTF-8">
<title>WordsWise AI Dictionary & Encyclopedia</title>
<meta name="viewport" content="width=device-width,initial-scale=1">
<script src="https://cdnjs.cloudflare.com/ajax/libs/html2pdf.js/0.10.1/html2pdf.bundle.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/tesseract.js@4.0.2/dist/tesseract.min.js"></script>
<style>
:root { 
    --bg: linear-gradient(135deg, #eef2f8 0%, #d1e7ff 100%); 
    --card:#fff; 
    --text:#111; 
    --accent:#0078ff; 
}
body.dark { 
    --bg: linear-gradient(135deg, #1c1c1c 0%, #2a2a2a 100%); 
    --card:#242424; 
    --text:#eee; 
}
body { 
    background: var(--bg); 
    color:var(--text); 
    padding:20px; 
    font-family:'Segoe UI',sans-serif; 
    transition:.25s; 
    background-attachment: fixed; /* Ensures the gradient stays fixed on scroll */
}
.container { max-width:920px; margin:auto; text-align:center; }
h1 { font-size: 4em; font-weight: bold; margin-bottom: 10px; }
input,button,select,textarea { padding:10px; margin:6px; border-radius:8px; border:1px solid #888; font-size:15px; transition:.15s; }
textarea { width: 80%; height: 100px; resize: vertical; }
button { background:var(--accent); color:#fff; border:none; cursor:pointer; }
button:hover { transform:scale(1.03); }
#result { margin-top:18px; padding:18px; background:var(--card); border-radius:12px; box-shadow:0 6px 24px rgba(0,0,0,.12); text-align:left; min-height:60px; }
.small { font-size:13px; color:#555; }
.controls { display:flex; flex-wrap:wrap; gap:12px; justify-content:center; }
.voice-bar { height:10px; width:100%; background:#ddd; border-radius:5px; margin-top:6px; overflow:hidden; position:relative; display:none; }
.voice-level { height:100%; background:var(--accent); width:0%; transition:0.1s; }
.gallery { display:flex; flex-wrap:wrap; gap:6px; margin-top:10px; }
.gallery img { max-width:100px; border-radius:8px; cursor:pointer; }
#cameraContainer { display:none; margin-top:20px; }
#cameraVideo { width:100%; max-width:400px; border-radius:8px; }
#cameraCanvas { display:none; }
footer { margin-top:30px; opacity:0.85; text-align:center; font-weight:bold; }
#paragraphTranslatorSection { display: none; margin-top: 20px; }
</style>
</head>
<body>
<div class="container">
<h1>WordsWise AI </h1>
<h2>Dictionary & Encyclopedia</h2>
<h3>-Ultimate Edition-</h3>

<div>
<input id="wordInput" placeholder="Search here anything" style="width:55%;" oninput="clearSuggestions()"/>
<select id="langSelect">
  <!-- Indian Languages -->
  <option value="en">English</option>
  <option value="hi">Hindi</option>
  <option value="ta">Tamil</option>
  <option value="te">Telugu</option>
  <option value="kn">Kannada</option>
  <option value="ml">Malayalam</option>
  <option value="mr">Marathi</option>
  <option value="bn">Bengali</option>
  <option value="gu">Gujarati</option>
  <option value="pa">Punjabi</option>
  <option value="or">Odia</option>
  <option value="as">Assamese</option>
  <option value="sd">Sindhi</option>
  <option value="ur">Urdu</option>
  <!-- Global Languages -->
  <option value="es">Spanish</option>
  <option value="fr">French</option>
  <option value="de">German</option>
  <option value="ja">Japanese</option>
  <option value="it">Italian</option>
  <option value="ru">Russian</option>
  <option value="ar">Arabic</option>
  <option value="pt">Portuguese</option>
  <option value="zh">Chinese</option>
  <option value="ko">Korean</option>
  <option value="tr">Turkish</option>
</select>
<div id="suggestions" class="small"></div>
</div>

<div class="controls">
<button onclick="searchWord()">🔍 Search</button>
<button onclick="startVoiceSearch()">🎤 Voice Search</button>
<button onclick="toggleParagraphTranslator()">📝 Paragraph Translater</button>
<button onclick="startCameraTranslate()">📷 Translating Lens</button>
<button onclick="toggleTheme()">🌙☀️Theme</button>
<button onclick="downloadPDF()">📄 PDF</button>
</div>

<!-- Paragraph Translator Section -->
<div id="paragraphTranslatorSection">
<h3>Paragraph Translator</h3>
<textarea id="paragraphInput" placeholder="Enter a paragraph to translate"></textarea>
<button onclick="translateParagraph()">🌐 Translate Paragraph</button>
<div id="translatedParagraph" style="margin-top: 10px; padding: 10px; background: var(--card); border-radius: 8px; display: none;"></div>
</div>

<div class="voice-bar" id="voiceBar"><div class="voice-level" id="voiceLevel"></div></div>
<p id="voiceStatus" class="small"></p>
<div id="cameraContainer">
<video id="cameraVideo" autoplay></video>
<button onclick="captureImage()">📸 Capture</button>
<canvas id="cameraCanvas"></canvas>
</div>
<div id="result">Search anything or use voice/camera features.</div>
</div>

<footer>A Creation and Programmatic Masterpiece by Maanvith Sai</footer>
<footer> 
    <div class="ai-disclaimer">
        <span style="font-size: 0.8em; font-family: 'Your Chosen Font', sans-serif; color: #777;">
            Still under experiments. Our AI can make mistakes. Please re-check the information.
        </span>
    </div>
    
</footer>
<script>
function logErr(e){ console.error(e); }
function toggleTheme(){ document.body.classList.toggle('dark'); }
function clearSuggestions(){ document.getElementById('suggestions').innerHTML=''; }

function toggleParagraphTranslator() {
    const section = document.getElementById('paragraphTranslatorSection');
    section.style.display = section.style.display === 'none' ? 'block' : 'none';
}

async function searchWord(){
const wordInput = document.getElementById('wordInput');
let word = wordInput.value.trim();
const targetLang = document.getElementById('langSelect').value;
const res = document.getElementById('result');

if(!word){ res.innerHTML='Enter a word or topic to search.'; return; }

res.innerHTML='⏳ Asking Ai...';

// Special Maanvith profile
if(word.toLowerCase() === 'maanvith'){
res.innerHTML = `<h2>Maanvith Sai — Creator & Programmer</h2>
<p><b>Role:</b> Developer & Creator</p>
<p><b>Skills:</b> Full-stack, JavaScript, Web, AI Tools</p>
<img src="https://i.imgur.com/6XH8VxL.jpeg" style="max-width:220px;border-radius:12px;">
<p>Designed and programmed entirely by <b>Maanvith Sai</b>.</p>`;
return;
}

let def=null, example=null, synonyms=[], entryWord=word, images=[];

// 1) Dictionary API
try {
let dResp = await fetch(`https://api.dictionaryapi.dev/api/v2/entries/en/${encodeURIComponent(word)}`);
let dJson = await dResp.json();
if(Array.isArray(dJson) && dJson[0]){
let entry=dJson[0], meaning=entry.meanings?.[0];
entryWord=entry.word;
def=meaning?.definitions?.[0]?.definition || null;
example=meaning?.definitions?.[0]?.example || null;
synonyms=meaning?.definitions?.[0]?.synonyms || [];
}
}catch(e){ logErr(e); }

// 2) Wikipedia API
try{
let w = await fetch(`https://en.wikipedia.org/api/rest_v1/page/summary/${encodeURIComponent(word)}`);
let wj = await w.json();
if(wj?.extract){
def=def || wj.extract;
example=example || `Refers to: ${wj.description || entryWord}`;
entryWord=wj.title || entryWord;
if(wj.originalimage) images.push(wj.originalimage.source);
}
}catch(e){ logErr(e); }

// 3) Google Custom Search fallback
if(!def){
try{
let gRes = await fetch(`https://www.googleapis.com/customsearch/v1?key=YOUR_GOOGLE_API_KEY&cx=YOUR_CX&q=${encodeURIComponent(word)}`);
let gj = await gRes.json();
if(gj.items && gj.items[0]){
def = gj.items[0].snippet || gj.items[0].title;
entryWord = gj.items[0].title || entryWord;
if(gj.items[0].pagemap?.cse_image?.[0]?.src) images.push(gj.items[0].pagemap.cse_image[0].src);
}
}catch(e){ logErr(e); }
}


// 4) Unsplash images (movies, sports, topics)
try{
let imgResp = await fetch(`https://api.unsplash.com/search/photos?query=${encodeURIComponent(word)}&per_page=6&client_id=YOUR_UNSPLASH_ACCESS_KEY`);
let imgJson = await imgResp.json();
if(imgJson.results) images.push(...imgJson.results.map(img=>img.urls.small));
}catch(e){ logErr(e); }

if(!def){ 
    let html = "No results found.";
    if(images.length>0){
        html += `<div class="gallery">${images.map(img=>`<img src="${img}" onclick="window.open('${img}','_blank')">`).join('')}</div>`;
    }
    res.innerHTML = html;
    return; 
}

let easy = def.length>90 ? def.split(" ").slice(0,15).join(" ")+'...' : def;

// Translation
let translated=entryWord;
try{
let tRes = await fetch(`https://api.mymemory.translated.net/get?q=${encodeURIComponent(entryWord)}&langpair=en|${targetLang}`);
let tj = await tRes.json();
translated = tj.responseData?.translatedText || entryWord;
}catch(e){}

let html = `<h2>${entryWord} <button onclick="speak('${entryWord}')">🔊</button></h2>
<p><b>Definition:</b> ${def} <button onclick="speak(\`${def}\`)">🔊</button></p>
<p><b>Easy Meaning:</b> ${easy} <button onclick="speak(\`${easy}\`)">🔊</button></p>
<p><b>Example:</b> ${example || "No example"} <button onclick="speak(\`${example}\`)">🔊</button></p>
<p><b>Synonyms:</b> ${synonyms.slice(0,6).join(', ') || 'None'}</p>
<p><b>Translated (${targetLang}):</b> ${translated}</p>`;

if(images.length>0){
html += `<div class="gallery">${images.map(img=>`<img src="${img}" onclick="window.open('${img}','_blank')">`).join('')}</div>`;
}

res.innerHTML = html;
}

// Paragraph Translator Function
async function translateParagraph() {
    const paragraphInput = document.getElementById('paragraphInput');
    const paragraph = paragraphInput.value.trim();
    const targetLang = document.getElementById('langSelect').value;
    const translatedDiv = document.getElementById('translatedParagraph');

    if (!paragraph) {
        translatedDiv.style.display = 'block';
        translatedDiv.innerHTML = 'Enter a paragraph to translate.';
        return;
    }

    translatedDiv.style.display = 'block';
    translatedDiv.innerHTML = '⏳ Translating...';

    try {
        let tRes = await fetch(`https://api.mymemory.translated.net/get?q=${encodeURIComponent(paragraph)}&langpair=en|${targetLang}`);
        let tj = await tRes.json();
        const translatedText = tj.responseData?.translatedText || 'Translation failed.';
        translatedDiv.innerHTML = `<h4>Translated Paragraph (${targetLang}):</h4><p>${translatedText}</p>`;
    } catch (e) {
        translatedDiv.innerHTML = 'Translation error.';
        logErr(e);
    }
}

// SPEECH
function speak(text){ let u = new SpeechSynthesisUtterance(text); u.lang="en-US"; speechSynthesis.speak(u); }

// VOICE SEARCH with animated bar
let voiceRec=null, animInterval=null;
function startVoiceSearch(){
const SR=window.SpeechRecognition||window.webkitSpeechRecognition;
if(!SR){ alert("Browser not supported"); return; }
const status=document.getElementById("voiceStatus");
const voiceBar=document.getElementById("voiceBar");
const voiceLevel=document.getElementById("voiceLevel");
voiceBar.style.display="block";
status.innerHTML="🎙 Listening...";
voiceLevel.style.width="0%";

voiceRec=new SR();
voiceRec.lang="en-US";
voiceRec.interimResults=false;
voiceRec.maxAlternatives=1;

voiceRec.onresult=e=>{
const text=e.results[0][0].transcript;
document.getElementById("wordInput").value=text;
stopVoiceAnimation();
status.innerHTML="Detected: "+text;
searchWord();
};
voiceRec.onerror=e=>{
stopVoiceAnimation();
status.innerHTML="Voice error";
logErr(e);
};
voiceRec.onend=()=>stopVoiceAnimation();
voiceRec.start();
animInterval=setInterval(()=>{ voiceLevel.style.width=(Math.random()*100)+"%"; },100);
}
function stopVoiceAnimation(){ clearInterval(animInterval); document.getElementById("voiceBar").style.display="none"; }

// CAMERA TRANSLATE
let stream = null;
async function startCameraTranslate(){
    const video = document.getElementById('cameraVideo');
    const container = document.getElementById('cameraContainer');
    const res = document.getElementById('result');
    res.innerHTML = '⏳ Starting camera...';
    try {
        stream = await navigator.mediaDevices.getUserMedia({ video: true });
        video.srcObject = stream;
        container.style.display = 'block';
        res.innerHTML = 'Camera active. Click Capture to scan text.';
    } catch (e) {
        res.innerHTML = 'Camera access denied or not supported.';
        logErr(e);
    }
}

function captureImage(){
    const video = document.getElementById('cameraVideo');
    const canvas = document.getElementById('cameraCanvas');
    const ctx = canvas.getContext('2d');
    const res = document.getElementById('result');
    canvas.width = video.videoWidth;
    canvas.height = video.videoHeight;
    ctx.drawImage(video, 0, 0);
    const imageData = canvas.toDataURL('image/png');
    res.innerHTML = '⏳ Processing image...';
    // Stop camera
    if (stream) {
        stream.getTracks().forEach(track => track.stop());
        document.getElementById('cameraContainer').style.display = 'none';
    }
    // OCR with Tesseract
    Tesseract.recognize(imageData, 'eng', { logger: m => console.log(m) })
        .then(({ data: { text } }) => {
            if (text.trim()) {
                // Translate the extracted text
                const targetLang = document.getElementById('langSelect').value;
                fetch(`https://api.mymemory.translated.net/get?q=${encodeURIComponent(text.trim())}&langpair=en|${targetLang}`)
                    .then(response => response.json())
                    .then(data => {
                        const translatedText = data.responseData?.translatedText || 'Translation failed.';
                        res.innerHTML = `<h4>Extracted Text:</h4><p>${text.trim()}</p><h4>Translated (${targetLang}):</h4><p>${translatedText}</p>`;
                    })
                    .catch(e => {
                        res.innerHTML = `<h4>Extracted Text:</h4><p>${text.trim()}</p><p>Translation failed.</p>`;
                        logErr(e);
                    });
            } else {
                res.innerHTML = 'No text detected in image.';
            }
        })
        .catch(e => {
            res.innerHTML = 'OCR failed.';
            logErr(e);
        });
}


// PDF
function downloadPDF(){ html2pdf().from(document.getElementById("result")).save("WordsWise.pdf"); }
</script>
</body>
</html>
