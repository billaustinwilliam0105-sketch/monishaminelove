<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<meta name="theme-color" content="#2c101e">
<title>For Monisha | A Little World of Us</title>
<style>
@import url('https://fonts.googleapis.com/css2?family=Dancing+Script:wght@400;500;600;700&family=Manrope:wght@300;400;500;600&display=swap');
:root{--wine:#581d35;--rose:#d86c88;--cream:#fff8f1;--ink:#4a2634;--gold:#d8b77c}
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
h1,h2,h3{font-family:"Dancing Script",cursive;font-weight:500}
.hero h1{font-size:clamp(4rem,11vw,8.5rem);line-height:.95;margin:0;color:#fff1ed}
.hero .sub{max-width:560px;line-height:1.9;margin:24px auto 28px;color:#f2dfe3;font-size:.95rem}
.glow-heart{font-size:2.8rem;display:block;margin-bottom:22px;filter:drop-shadow(0 0 18px #ff8eae);animation:beat 1.8s infinite}
@keyframes beat{0%,100%{transform:scale(1)}50%{transform:scale(1.12)}}
.btn{border:1px solid transparent;border-radius:999px;padding:13px 23px;background:linear-gradient(135deg,#e99aaf,#c9587a);color:#fff;box-shadow:0 9px 28px #68283b2b;transition:.25s}
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
.letter-paper{max-width:720px;margin:28px auto 0;padding:clamp(25px,5vw,48px);background:#fffdf8;border:1px solid #f1d8dc;box-shadow:0 18px 45px #6c29350e;text-align:left;line-height:1.95;font-size:.95rem}
.letter-paper p,.dream-card p,.final-note p{margin:0 0 1.2em}
.letter-paper .salutation,.letter-paper .signature{font:2rem "Dancing Script",cursive;color:#a34461;margin-bottom:.5em}
#timeline{background:#fffdf9}
.timeline{max-width:760px;margin:45px auto 0;text-align:left;position:relative}
.timeline:before{content:"";position:absolute;left:20px;top:8px;bottom:8px;width:1px;background:#e7b8c5}
.moment{position:relative;padding:0 0 32px 58px}
.moment:last-child{padding-bottom:0}
.moment:before{content:"♡";position:absolute;left:7px;top:0;width:27px;height:27px;border-radius:50%;display:grid;place-items:center;background:#fff0f3;border:1px solid #e7b8c5;color:#bd5b78}
.moment .date{font-size:.67rem;text-transform:uppercase;letter-spacing:.17em;color:#b45a75}
.moment h3{font-size:2rem;margin:5px 0;color:var(--wine)}
.moment p{line-height:1.8;font-size:.88rem;color:#805b68;margin:0}
.note{font-size:.85rem;color:#9b7883;margin:25px auto;max-width:560px;line-height:1.8}
#garden{background:linear-gradient(180deg,#f9e6eb,#fff7f0)}
.rose-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px;max-width:760px;margin:35px auto}
.rose-card{background:#ffffffb8;border:1px solid #fff;border-radius:18px;padding:22px 12px;min-height:155px;transition:.25s}
.rose-card:hover{transform:translateY(-5px)}
.rose{font-size:3rem;display:block;filter:drop-shadow(0 6px 7px #a63b5520);transition:transform .3s}
.rose-card:hover .rose{transform:rotate(-8deg) scale(1.12)}
.rose-card span:last-child{display:block;font-size:.76rem;margin-top:10px;color:#875467}
.rose-message{max-width:600px;min-height:75px;margin:20px auto 0;padding:20px;background:#fffdf9;border-radius:16px;font:1.6rem/1.5 "Dancing Script",cursive;color:#a34461;box-shadow:0 8px 25px #6c29350c}
#reasons{background:#fffdf9}
.reason-grid{display:grid;grid-template-columns:repeat(3,minmax(0,1fr));gap:15px;margin:38px auto;max-width:900px}
.reason-card{border:1px solid #f0d8dd;background:#fff;border-radius:18px;min-height:160px;padding:20px 15px;text-align:center;transition:.3s;position:relative;overflow:hidden}
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
.dream-card{max-width:720px;margin:30px auto;padding:35px;border:1px solid #e5b4c34a;border-radius:22px;background:#ffffff09;line-height:2;color:#f8e8e8;text-align:left}
#final{min-height:100svh;display:grid;place-items:center;background:radial-gradient(ellipse at center,#7a304b 0,#3a1b2b 54%,#1d1019 100%);color:#fff0ed;overflow:hidden;position:relative}
#final h2{color:#fff0ed}
#final .lead{color:#f2dce2}
.final-heart{font-size:4rem;display:block;filter:drop-shadow(0 0 20px #ff93b0);animation:beat 1.7s infinite}
.final-note{max-width:650px;margin:25px auto;padding:30px;border:1px solid #e6c0c34a;background:#ffffff08;border-radius:20px;line-height:2;text-align:left}
.song{max-width:480px;margin:28px auto 0}
.song p{font-size:.8rem;color:#e8cbd2;margin:0 0 10px}
.song iframe{border:0;border-radius:12px;width:100%}
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
    <p class="lead">Tap the envelope to open it. Take your time. This little letter is meant to be read slowly.</p>
    <div class="envelope-wrap">
      <div class="envelope" id="envelope" role="button" tabindex="0" aria-label="Open the letter" onclick="openEnvelope()" onkeydown="if(event.key==='Enter'||event.key===' '){event.preventDefault();openEnvelope()}">
        <div class="paper"><strong>For you, Monisha</strong><span>A few words I wanted you to have, whenever you need them. ♡</span></div>
        <div class="seal">♡</div>
      </div>
    </div>
    <p class="envelope-hint" id="envelopeHint">Tap the envelope to open your letter</p>
    <article class="letter-paper hidden" id="letterPaper">
      <div class="salutation">My dear Monisha,</div>
      <p>There is no logic when it comes to you. You have a way of making my heart forget everything else and choose you, every single time. ❤️</p>
      <p>The more I get to know you, the more reasons you give me to fall for you, and the funny part is, I was never looking for a way out. 😉</p>
      <p>I wish you could borrow my eyes for a moment and see yourself the way I see you. Maybe then you'd understand why, even on my busiest days, one little thought of you is enough to make me smile like an idiot. 🫣</p>
      <p>I don't just want to love you when you're happy and everything feels right. I want to be there when you're tired, when life gets difficult, and when you don't have the words to explain what's wrong, and all you need is someone who understands without making you explain a hundred times. 🫶🏻</p>
      <p>I may never find the perfect words for what you mean to me, so I want my actions to say what my words can't. I want to be someone you can trust and lean on, someone who celebrates your dreams as if they were his own.</p>
      <p>I can't promise a perfect life, but I promise to keep trying to make yours softer and more beautiful in every way I can. ❤️</p>
      <p>And if you ever ask what I want in return, just give me that smile of yours, let me steal a little of your time, and maybe let me be the reason for a few of those butterflies. 🦋</p>
      <div class="signature">With affection, always ♡</div>
      <p style="font-size:.78rem;color:#9b7883;margin-top:12px">Whenever and wherever, I will love you like my breath, till my last day.</p>
    </article>
    <button class="btn dark" style="margin-top:28px" onclick="goTo('timeline')">Walk through our story ↓</button>
  </div>
</section>

<section id="timeline">
  <div class="section-inner">
    <p class="section-kicker">02 · Memories</p>
    <h2>Our story, one moment at a time</h2>
    <p class="lead">A relationship is built from tiny moments as much as big ones: day by day, with a lot of love, and with forgiveness after the hard moments. Love is not about finding new people. It is about choosing the same person again and again, even after all the fights.</p>
    <div class="timeline">
      <div class="moment"><span class="date">Melted in her eyes</span><h3>Awww Monishaaa...</h3><p>When I saw you for the first time, I felt a connection I couldn't explain. I had never felt it before. I still remember how it started, like a whole garden of memories with you in every corner.</p></div>
      <div class="moment"><span class="date">Caught in her smile</span><h3>A memory that stays</h3><p>We understood each other from the start. It felt like we were meant to be together, and every moment since has reminded me of that. I never looked for perfection, only a better connection, flaws and all.</p></div>
      <div class="moment"><span class="date">Kingdom of Love</span><h3>My Queen</h3><p>You have been my first priority for as long as I've loved you. You are already the queen of my kingdom, and you will always be treated like one, by me and by my family too.</p></div>
      <div class="moment"><span class="date">Towards Destiny</span><h3>The next page</h3><p>No need to predict the whole future. Let's leave room for good conversations, new memories, and taking things one step at a time. I won't walk away, and I'll never make you feel low for choosing me. Every day with you, my Queen, is worth celebrating.</p></div>
    </div>
    <p class="note">I can't hand you the whole world, but I can promise to show up for you, in any situation, every time.</p>
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
    <p class="lead">Tap each card to see why.</p>
    <div class="reason-grid">
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">😊</span><b>Your smile</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">Your smile can turn an ordinary moment into the best part of my day.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">✨</span><b>Your dreams</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">I admire the goals you have and the life you're building. Keep believing in yourself. I'm cheering for you.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">💬</span><b>Our talks</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">I could listen to your endless stories forever. Even the smallest chats become memories I carry with me.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">🩷</span><b>Angel</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">You showed up like light in my hardest days. That is why you'll always be my Angel.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">😂</span><b>Stressburster</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">However heavy my day is, you can make me laugh and the stress just melts away.</span></button>
      <button class="reason-card" onclick="toggleReason(this)"><span class="front"><span class="icon">🍀</span><b>Luckycharm</b><span style="font-size:.7rem">Tap to reveal</span></span><span class="back">You gave me hope when I needed it most. Meeting you is the luckiest thing that happened to me.</span></button>
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
      <p>To my Monishaaa… my Angel, my Stressburster, my Luckycharm… 🩷🥹</p>
      <p>There's something my heart has been wanting to tell you. I don't think I'll ever fit everything I feel into words, but today I want to try.</p>
      <p>Even when everything around me felt like chaos, when life was full of pain, stress, and uncertainty, you were there like the brightest light in a dark room. You brought light into my difficult days in ways you might not even realise. ❤️‍🩹</p>
      <p>Seeing you happy, peaceful, successful, and proud of yourself is one of the things I wish for most. Whenever life gets hard for you, you don't have to face it alone. I'll be in front of you when you need someone to stand up for you, beside you when you need someone to walk with you, and behind you when you need quiet support. 🫂</p>
      <p>When I look back, so much has changed. In 2023, I went through my major operation. In 2024, I received my offer from Finulent. In 2025, I received my offer from Enphase. Those are milestones I'll always remember.</p>
      <p>But somewhere between all those struggles, changes, and achievements, there was you.</p>
      <p>Thank you for making my life more beautiful, for teaching me to be more responsible, and for helping me understand love in ways I didn't know before. Thank you for being part of the person I'm becoming.</p>
      <p>I know we haven't always had the easiest journey. We've had fights, misunderstandings, and days when we struggled to understand each other. I won't pretend it has all been perfect. But I've learned that a meaningful bond isn't about never having problems. It's about learning from them and becoming better people.</p>
      <p>You've forgiven my mistakes, corrected me when I was wrong, and helped me see what I needed to change. I don't take that lightly. Trust, respect, and peace are built through actions, not just words, and I want to keep becoming someone who brings you comfort and security. 💞</p>
      <p>I don't just want to be someone who says "I love you." I want to be someone whose actions make you feel loved. I want to celebrate your smallest achievements like they're the biggest victories, listen when you have a thousand thoughts running through your mind, and be there for your silly moments, your happy days, your stressful evenings, and the days you don't feel like explaining anything at all.</p>
      <p>And if life gives us the chance to build a future together, I dream of something simple and beautiful: a peaceful little home, silly arguments over small things, cooking together, laughing over nonsense, and ending each day with someone who genuinely cares. Maybe a little 2BHK filled with our laughter and our own kind of happiness. 🏡</p>
      <p>I know love can't be forced, and I never want my feelings to become a burden on your heart. I want whatever grows between us to be genuine, peaceful, and chosen by both of us. Your happiness matters to me, and so does what your heart truly feels.</p>
      <p>But if you ask what my heart wishes for… more beautiful memories with you. More laughter. More understanding. More moments where we choose patience over anger. And, if someday your heart feels the same, the privilege of calling you my person for life. 🩷</p>
      <p>And if you ever ask me, "Why me?", I'll probably smile and say: "I don't know how to explain it, Monisha. My heart found something in you it never wanted to treat as ordinary." 🥹</p>
      <p>I can't promise a life without difficulties, but I can promise to keep working on myself, to respect your feelings, and to be honest about mine. I want my love to be something you feel in the way I treat you, not just something you read in a message. 💌</p>
      <p style="margin:0">With lots of love, always your Angel's… Stressburster's… Luckycharm's person. 🌹</p>
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
      <p>Monishaaa, my Angel… 🥹❤️</p>
      <p>You deserve kindness on your hardest days, laughter on your ordinary days, and someone who makes you feel loved, respected, and appreciated in the little things.</p>
      <p>If you choose me, I want to be that person. I want to make you smile when you're stressed, celebrate your little wins, listen to your endless stories, and stand beside you through every high and low. Even during our fights, I want us to learn, understand each other, and choose kindness over ego.</p>
      <p>I can't promise to be perfect, but I promise to keep trying to be better for us. I want to be your safe place and your biggest supporter, the person you can be yourself with, without pretending.</p>
      <p><strong>I don't know what the future holds, but if I could choose, I'd love to build a beautiful little life with you, filled with silly fights, endless laughter, random hugs, and lots of love.</strong> 🫂</p>
      <p>Thank you for being part of my story, my Luckycharm. And if you let me, I'd love to be part of your forever. 🩷🌷</p>
      <p style="font:2.3rem 'Dancing Script',cursive;color:#f1bdca;margin:0">Made with care, just for you. ♡</p>
    </div>
    <div class="song">
      <p>♫ Our song</p>
      <iframe data-testid="embed-iframe" src="https://open.spotify.com/embed/track/4nSwWiwtieiNmRAjy9fEXN?utm_source=generator" height="152" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy" title="Our song"></iframe>
    </div>
    <div style="margin-top:24px"><button class="btn ghost" onclick="finale()">A little shower of love ✨</button></div>
    <div id="finaleMessage" class="hidden" style="font:2rem 'Dancing Script',cursive;margin-top:22px">If I could hug you right now, it would be an endless cuddle. For now, a thousand virtual hugs for you 🤗♡</div>
  </div>
</section>
</main>

<footer>A small handmade gift · Made with care ♡</footer>

<script>
const roseNotes = [
  "I hope today gives you a reason to smile, even a tiny one. 🌹 Being with you makes me feel completely fulfilled, and I'll keep loving you more every day.",
  "I'll be there in all the moments of your life, and I'll always stand by your side. Keep being curious, brave, and wonderfully yourself. You have so much ahead of you. 🌷",
  "I hope we never run out of little things to laugh about. 😂 Your happiness is something I take seriously, and I'll always protect the playful, joyful side of you.",
  "You deserve to be heard, understood, and treated with kindness, always. ♡ I'll be there to listen and to love you for exactly who you are. 🌸",
  "May you get closer to every dream you're working so hard for. ✨ I'll be your biggest cheerleader, celebrating your victories and standing with you through the challenges. 🌹",
  "This rose has one job: to remind you that someone wanted to make your day a little sweeter. 💗 I'll always be your safe place, your confidant, and your biggest fan. 🌺"
];
function goTo(id){
  const t=document.getElementById(id);
  if(t) t.scrollIntoView({behavior:"smooth",block:"start"});
}
function openEnvelope(){
  document.getElementById("envelope").classList.add("open");
  document.getElementById("envelopeHint").textContent="A little letter, just for you ♡";
  setTimeout(()=>{
    const l=document.getElementById("letterPaper");
    l.classList.remove("hidden");
    l.scrollIntoView({behavior:"smooth",block:"center"});
  },650);
}
function showRose(i){document.getElementById("roseMessage").textContent=roseNotes[i]}
function toggleReason(c){c.classList.toggle("revealed")}
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
