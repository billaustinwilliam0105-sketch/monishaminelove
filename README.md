<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#2c101e">
<title>For Monisha | A Little World of Us</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@400;500;600;700&family=Dancing+Script:wght@400;500;600;700&family=Manrope:wght@300;400;500;600&display=swap');
:root{--wine:#581d35;--rose:#d86c88;--blush:#f8dce3;--cream:#fff8f1;--ink:#4a2634;--gold:#d8b77c;--night:#24121e}
*{box-sizing:border-box}
html{scroll-behavior:smooth}
body{margin:0;background:var(--cream);color:var(--ink);font-family:Manrope,sans-serif;overflow-x:hidden}
button{font:inherit;cursor:pointer}
button:focus-visible,a:focus-visible{outline:3px solid var(--gold);outline-offset:4px}
#particles{position:fixed;inset:0;pointer-events:none;overflow:hidden;z-index:20}
.particle{position:absolute;bottom:-35px;animation:drift linear forwards;opacity:.75}
@keyframes drift{to{transform:translateY(-115vh) rotate(35deg);opacity:0}}
.hero{min-height:100svh;display:grid;place-items:center;text-align:center;padding:50px 20px;color:#fff4f2;background:radial-gradient(ellipse at 50% 20%,#78334c 0,#421d30 45%,#20121c 100%);position:relative;isolation:isolate;overflow:hidden}
.hero:before,.hero:after{content:"";position:absolute;border:1px solid #e9bdc13d;border-radius:50%;width:min(78vw,680px);aspect-ratio:1;z-index:-1;animation:rotate 35s linear infinite}
.hero:after{width:min(58vw,490px);animation-direction:reverse}
@keyframes rotate{to{transform:rotate(360deg)}}
.eyebrow{text-transform:uppercase;letter-spacing:.28em;font-size:.68rem;color:var(--gold);margin:0 0 20px}
h1,h2,h3,.script{font-family:"Dancing Script",cursive;font-weight:500}
.hero h1{font-size:clamp(4rem,11vw,8.5rem);line-height:.95;margin:0;color:#fff1ed}
.hero .sub{max-width:560px;line-height:1.9;margin:24px auto 28px;color:#f2dfe3;font-size:.95rem}
.glow-heart{font-size:2.8rem;display:block;margin-bottom:22px;filter:drop-shadow(0 0 18px #ff8eae);animation:beat 1.8s infinite}
@keyframes beat{0%,100%{transform:scale(1)}50%{transform:scale(1.12)}}
.btn{border:1px solid transparent;border-radius:999px;padding:13px 23px;background:linear-gradient(135deg,#e99aaf,#c9587a);color:white;box-shadow:0 9px 28px #68283b2b;transition:.25s}
.btn:hover{transform:translateY(-3px);box-shadow:0 12px 32px #68283b45}
.btn.ghost{background:transparent;color:inherit;border-color:currentColor;box-shadow:none}
.btn.dark{background:var(--wine)}
section{padding:88px 20px;text-align:center}
.section-inner{width:min(100%,1000px);margin:auto}
.section-kicker{font-size:.67rem;letter-spacing:.24em;text-transform:uppercase;color:#b45a75;margin-bottom:14px}
h2{font-size:clamp(2.8rem,7vw,5rem);line-height:1.02;margin:0 0 18px;color:var(--wine)}
.lead{max-width:640px;margin:0 auto 30px;line-height:1.85;color:#805b68;font-size:.94rem}
.hidden{display:none!important}
#letter{background:linear-gradient(180deg,#fff8f1,#f9e5e9)}
.envelope-wrap{width:min(90vw,440px);margin:34px auto 22px;perspective:1000px}
.envelope{height:260px;position:relative;background:#eab9c4;border-radius:4px 4px 12px 12px;box-shadow:0 25px 60px #6c293522;cursor:pointer;isolation:isolate}
.envelope:before{content:"";position:absolute;inset:0;background:linear-gradient(145deg,#f5d5d9,#e5a9b7);clip-path:polygon(0 0,50% 58%,100% 0);z-index:3;transform-origin:top;transition:transform 1s ease}
.envelope:after{content:"";position:absolute;inset:0;background:linear-gradient(35deg,#d88ea2,#f3cbd2);clip-path:polygon(0 100%,0 0,50% 56%,100% 0,100% 100%);z-index:2}
.envelope .seal{position:absolute;z-index:4;left:50%;top:53%;transform:translate(-50%,-50%);width:48px;height:48px;border-radius:50%;background:#9f3454;color:#fff4f2;display:grid;place-items:center;font-size:1.35rem;box-shadow:0 3px 9px #72253d44;transition:.4s}
.envelope .paper{position:absolute;z-index:1;left:7%;right:7%;bottom:5%;height:86%;background:#fffaf2;padding:25px 22px;text-align:center;display:flex;flex-direction:column;justify-content:center;transition:transform 1s ease,bottom 1s ease;box-shadow:0 2px 12px #652d3b18;overflow:hidden}
.envelope .paper strong{font:2.2rem "Dancing Script",cursive;color:#a34461}
.envelope .paper span{font-size:.72rem;line-height:1.6;margin-top:8px}
.envelope.open:before{transform:rotateX(180deg);z-index:0}
.envelope.open .seal{opacity:0;transform:translate(-50%,-50%) scale(.2)}
.envelope.open .paper{transform:translateY(-68px);bottom:5%;height:100%;z-index:5;transition-delay:.35s}
.envelope-hint{font-size:.76rem;color:#9e6b7b}
.letter-paper{max-width:720px;margin:28px auto 0;padding:clamp(25px,5vw,48px);background:#fffdf8;border:1px solid #f1d8dc;box-shadow:0 18px 45px #6c29350e;text-align:left;line-height:2;font-size:.95rem;white-space:pre-line}
.letter-paper .salutation,.letter-paper .signature{font:2rem "Dancing Script",cursive;color:#a34461}
#timeline{background:#fffdf9}
.timeline{max-width:760px;margin:45px auto 0;text-align:left;position:relative}
.timeline:before{content:"";position:absolute;left:20px;top:8px;bottom:8px;width:1px;background:#e7b8c5}
.moment{position:relative;padding:0 0 32px 58px}
.moment:last-child{padding-bottom:0}
.moment:before{content:"♡";position:absolute;left:7px;top:0;width:27px;height:27px;border-radius:50%;display:grid;place-items:center;background:#fff0f3;border:1px solid #e7b8c5;color:#bd5b78}
.moment .date{font-size:.67rem;text-transform:uppercase;letter-spacing:.17em;color:#b45a75}
.moment h3{font-size:2rem;margin:5px 0;color:var(--wine)}
.moment p{line-height:1.8;font-size:.88rem;color:#805b68;margin:0}
.note{font-size:.75rem;color:#9b7883;margin-top:25px}
#garden{background:linear-gradient(180deg,#f9e6eb,#fff7f0)}
.rose-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px;max-width:760px;margin:35px auto}
.rose-card{background:#ffffffb8;border:1px solid #fff;border-radius:18px;padding:22px 12px;min-height:155px;transition:.25s}
.rose-card:hover{transform:translateY(-5px)}
.rose{font-size:3rem;display:block;filter:drop-shadow(0 6px 7px #a63b5520);transition:transform .3s}
.rose-card:hover .rose{transform:rotate(-8deg) scale(1.12)}
.rose-card span:last-child{display:block;font-size:.76rem;margin-top:10px;color:#875467}
.rose-message{max-width:600px;min-height:75px;margin:20px auto 0;padding:20px;background:#fffdf9;border-radius:16px;font:1.8rem "Dancing Script",cursive;color:#a34461;box-shadow:0 8px 25px #6c29350c}
#reasons{background:#fffdf9}
.reason-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px;margin:38px auto;max-width:900px}
.reason-card{border:1px solid #f0d8dd;background:white;border-radius:18px;min-height:160px;padding:20px 15px;text-align:center;transition:.3s;position:relative;overflow:hidden}
.reason-card .front{display:flex;height:100%;min-height:115px;flex-direction:column;justify-content:center;align-items:center;gap:12px}
.reason-card .front b{font:1.7rem "Dancing Script",cursive;color:#a34461;font-weight:500}
.reason-card .back{display:none;font-size:.83rem;line-height:1.7;color:#805b68}
.reason-card.revealed{background:#fff0f3;transform:translateY(-3px)}
.reason-card.revealed .front{display:none}
.reason-card.revealed .back{display:block}
.reason-card .icon{font-size:1.6rem}
#future{background:linear-gradient(145deg,#2b1521,#572239);color:#f9e7e8}
#future h2{color:#fff0ed}
#future .lead{color:#e9cbd3}
.dream-card{max-width:720px;margin:30px auto;padding:35px;border:1px solid #e5b4c34a;border-radius:22px;background:#ffffff09;line-height:2;color:#f8e8e8}
#final{min-height:100svh;display:grid;place-items:center;background:radial-gradient(ellipse at center,#7a304b 0,#3a1b2b 54%,#1d1019 100%);color:#fff0ed;overflow:hidden;position:relative}
#final h2{color:#fff0ed}
#final .lead{color:#f2dce2}
.final-heart{font-size:4rem;filter:drop-shadow(0 0 20px #ff93b0);animation:beat 1.7s infinite}
.final-note{max-width:650px;margin:25px auto;padding:30px;border:1px solid #e6c0c34a;background:#ffffff08;border-radius:20px;line-height:2}
#song-controls{margin:20px auto;display:flex;gap:10px;justify-content:center;flex-wrap:wrap}
#music-status{font-size:.72rem;color:#e8cbd2;margin-top:12px}
footer{text-align:center;background:#1d1019;color:#cba8b4;padding:25px;font-size:.72rem;letter-spacing:.04em}
@media(max-width:620px){section{padding:70px 17px}.rose-grid,.reason-grid{grid-template-columns:repeat(2,minmax(0,1fr))}.envelope{height:225px}.letter-paper{font-size:.88rem}.dream-card{padding:25px 20px}}
@media(prefers-reduced-motion:reduce){*,*::before,*::after{animation-duration:.01ms!important;animation-iteration-count:1!important;scroll-behavior:auto!important;transition-duration:.01ms!important}}
</style>
</head>
<body>
<div id="particles" aria-hidden="true"></div>

<header class="hero">
  <div>
    <span class="glow-heart">♡</span>
    <p class="eyebrow">A little world made just for you</p>
    <h1>For Monisha</h1>
    <p class="sub">Some feelings are too special to fit into an ordinary message. So I made you a little place made of memories, roses, and words from my heart.</p>
    <button class="btn" onclick="goTo('letter')">Open your little surprise ✉</button>
    <p style="font-size:.7rem;color:#d8b7c2;margin-top:22px">Made with care, just for you</p>
  </div>
</header>

<main>
<section id="letter">
  <div class="section-inner">
    <p class="section-kicker">01 · A letter from my heart</p>
    <h2>Something for you</h2>
    <p class="lead">Tap the envelope to open it. Take your time—this little letter is meant to be read slowly.</p>
    <div class="envelope-wrap">
      <div class="envelope" id="envelope" role="button" tabindex="0" aria-label="Open the letter" onclick="openEnvelope()" onkeydown="if(event.key==='Enter'||event.key===' '){event.preventDefault();openEnvelope()}">
        <div class="paper"><strong>For you, Monisha</strong><span>A few words I wanted you to have, whenever you need them. ♡</span></div>
        <div class="seal">♡</div>
      </div>
    </div>
    <p class="envelope-hint" id="envelopeHint">Tap the envelope to open your letter</p>
    <article class="letter-paper hidden" id="letterPaper">
      <div class="salutation">My dear Monisha,</div>
      <p>
Sometimes, words don't quite capture what a person means to us. Still, I wanted to try.

You have a special place in my heart—not because every moment has been perfect, but because our story has mattered to me. We've shared memories, learned things, and grown through moments that weren't always easy.

I care about your happiness, your dreams, and the person you're becoming. I hope you always feel free to be yourself around the people who love you, and that you never have to make yourself smaller to be understood.

I don't want this little website to ask anything of you or put pressure on your heart. I simply wanted to make something thoughtful, something that might bring a smile to your face and remind you that you are appreciated.

So here's a small pocket of warmth, made just for you. Open it on a happy day, a difficult day, or an ordinary day when you could use a little kindness.

      </p>
      <div class="signature">With affection, always ♡</div>
      <p style="font-size:.72rem;color:#9b7883;margin-top:12px">Tip: edit this letter in the code so it sounds exactly like you.</p>
    </article>
    <button class="btn dark" style="margin-top:28px" onclick="goTo('timeline')">Walk through our story ↓</button>
  </div>
</section>

<section id="timeline">
  <div class="section-inner">
    <p class="section-kicker">02 · Little chapters</p>
    <h2>Our story, one moment at a time</h2>
    <p class="lead">A relationship is made of tiny moments as much as big ones. Replace these sample chapters with memories that are truly yours.</p>
    <div class="timeline">
      <div class="moment"><span class="date">Chapter 01 · Edit this</span><h3>The beginning</h3><p>Write about how you first met, the first conversation you remember, or the moment you started to feel close.</p></div>
      <div class="moment"><span class="date">Chapter 02 · Edit this</span><h3>A memory that stays</h3><p>Add a funny moment, a late-night conversation, a shared joke, or a little detail that only the two of you understand.</p></div>
      <div class="moment"><span class="date">Chapter 03 · Edit this</span><h3>What we learned</h3><p>Every chapter can teach us something. Write about patience, understanding, or how you hope to treat each other with care.</p></div>
      <div class="moment"><span class="date">Chapter 04 · Still unfolding</span><h3>The next page</h3><p>No need to predict the whole future. Leave space for good conversations, new memories, and taking things one step at a time.</p></div>
    </div>
    <p class="note">Only include memories and dates that you both feel comfortable having on this page.</p>
    <button class="btn dark" onclick="goTo('garden')">Visit the rose garden 🌹</button>
  </div>
</section>

<section id="garden">
  <div class="section-inner">
    <p class="section-kicker">03 · Pick a rose</p>
    <h2>A garden of little messages</h2>
    <p class="lead">Every rose holds a different note. Tap one to discover it.</p>
    <div class="rose-grid">
      <button class="rose-card" onclick="showRose(0)"><span class="rose">🌹</span><span>Rose of warmth</span></button>
      <button class="rose-card" onclick="showRose(1)"><span class="rose">🌷</span><span>Rose of admiration</span></button>
      <button class="rose-card" onclick="showRose(2)"><span class="rose">🌹</span><span>Rose of laughter</span></button>
      <button class="rose-card" onclick="showRose(3)"><span class="rose">🌸</span><span>Rose of kindness</span></button>
      <button class="rose-card" onclick="showRose(4)"><span class="rose">🌹</span><span>Rose of dreams</span></button>
      <button class="rose-card" onclick="showRose(5)"><span class="rose">🌺</span><span>Rose just for you</span></button>
    </div>
    <div class="rose-message" id="roseMessage" aria-live="polite">Choose a rose, and let it tell you something lovely ♡</div>
    <button class="btn" onclick="goTo('reasons')" style="margin-top:25px">Find your little reasons ✨</button>
  </div>
</section>

<section id="reasons">
  <div class="section-inner">
    <p class="section-kicker">04 · The little things</p>
    <h2>Reasons you make me smile</h2>
    <p class="lead">Tap each card. You can replace these with specific things you genuinely appreciate about her.</p>
    <div class="reason-grid">
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">😊</span><b>Your smile</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">Your smile has a way of making an ordinary moment feel a little brighter.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">✨</span><b>Your dreams</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">I admire that you have your own goals and a life you're building. I hope you keep believing in yourself.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">💬</span><b>Our conversations</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">The little things we talk about can become memories I carry with me.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">🌷</span><b>Your individuality</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">You don't need to be anyone else. Your own way of seeing the world is part of what makes you you.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">😂</span><b>Your funny side</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">Add an inside joke here—the kind that makes absolutely no sense to anyone else.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">🫶</span><b>The little details</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">Sometimes it's the smallest things about someone that stay in your heart the longest.</span></button>
    </div>
    <button class="btn dark" onclick="goTo('future')">A little dream 🌙</button>
  </div>
</section>

<section id="future">
  <div class="section-inner">
    <p class="section-kicker">05 · A gentle hope</p>
    <h2>A dream, not a demand</h2>
    <p class="lead">The future doesn't need to be figured out all at once.</p>
    <div class="dream-card">
      I like the idea of ordinary happiness: talking after a long day, laughing at something silly, sharing a meal, encouraging each other's dreams, and learning how to understand each other better.

      <br><br>
      I hope that whatever the future brings, it leaves room for honesty, patience, kindness, and the freedom for both of us to grow.

      <br><br>
      For now, this is simply a little gift—and a wish that today brings you something to smile about. ♡
    </div>
    <button class="btn" onclick="goTo('final')">One last little surprise ✨</button>
  </div>
</section>

<section id="final">
  <div class="section-inner">
    <p class="section-kicker">Just for you</p>
    <span class="final-heart">♡</span>
    <h2>One last thing, Monisha</h2>
    <p class="lead">If this little corner of the internet made you smile, then it has done exactly what I hoped.</p>
    <div class="final-note" id="finalNote">
      You deserve kindness on the hard days, laughter on the ordinary days, and people who make you feel respected and appreciated.

      <br><br>
      Thank you for being part of my story. I hope life brings you beautiful things, big and small.

      <br><br>
      <span style="font:2.3rem 'Dancing Script',cursive;color:#f1bdca">Made with care, just for you. ♡</span>
    </div>
    <div id="song-controls">
      <button class="btn" onclick="toggleMusic()" id="musicButton">♫ Play our song</button>
      <button class="btn ghost" onclick="finale()">A little shower of love ✨</button>
    </div>
    <p id="music-status">Add your own licensed audio file to enable the song button.</p>
    <div id="finaleMessage" class="hidden" style="font:2rem 'Dancing Script',cursive;margin-top:22px">A thousand virtual hugs for you 🤗♡</div>
  </div>
</section>
</main>

<footer>A small handmade gift · Made with care ♡</footer>

<!-- Optional: add a song file named "our-song.mp3" in the same folder. -->
<audio id="ourSong" loop preload="none"><source src="our-song.mp3" type="audio/mpeg"></audio>

<script>
const roseNotes = [
  "I hope today gives you a reason to smile, even if it's a tiny one. 🌹",
  "Keep being curious, brave, and wonderfully yourself. You have so much ahead of you. 🌷",
  "I hope we never run out of little things to laugh about. 😂",
  "You deserve to be heard, understood, and treated with kindness—always. ♡",
  "May you get closer to the dreams you're working so hard for. ✨",
  "This rose has one job: to remind you that someone wanted to make your day a little sweeter. 💗"
];

function goTo(id){
  const target=document.getElementById(id);
  if(target) target.scrollIntoView({behavior:"smooth",block:"start"});
}
function openEnvelope(){
  const env=document.getElementById("envelope");
  env.classList.add("open");
  document.getElementById("envelopeHint").textContent="A little letter, just for you ♡";
  setTimeout(()=>{
    document.getElementById("letterPaper").classList.remove("hidden");
    document.getElementById("letterPaper").scrollIntoView({behavior:"smooth",block:"center"});
  },650);
}
function showRose(index){
  document.getElementById("roseMessage").textContent=roseNotes[index];
}
function toggleReason(card){card.classList.toggle("revealed")}
const song=document.getElementById("ourSong");
async function toggleMusic(){
  const button=document.getElementById("musicButton");
  const status=document.getElementById("music-status");
  if(song.paused){
    try{
      await song.play();
      button.textContent="Ⅱ Pause our song";
      status.textContent="Playing your chosen song ♡";
    }catch(e){
      status.textContent="Add a file named our-song.mp3 beside index.html, then tap again. Some browsers also require a user tap before music can play.";
    }
  }else{
    song.pause();
    button.textContent="♫ Play our song";
    status.textContent="Paused. Tap when you'd like to listen again.";
  }
}
function finale(){
  document.getElementById("finaleMessage").classList.remove("hidden");
  for(let i=0;i<32;i++) makeParticle(true);
}
const particleRoot=document.getElementById("particles");
function makeParticle(burst=false){
  const p=document.createElement("span");
  p.className="particle";
  p.textContent=["♡","♥","✧","🌸"][Math.floor(Math.random()*4)];
  p.style.left=Math.random()*100+"vw";
  p.style.fontSize=(12+Math.random()*20)+"px";
  p.style.color=["#d86c88","#d8b77c","#f2b8c8","#ffffff"][Math.floor(Math.random()*4)];
  p.style.animationDuration=(burst?3:6+Math.random()*6)+"s";
  particleRoot.appendChild(p);
  setTimeout(()=>p.remove(),burst?3500:13000);
}
setInterval(()=>makeParticle(false),1100);
</script>
</body>
</html>
