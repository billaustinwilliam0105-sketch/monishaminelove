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
I have an immense love for you. ❤️
There is no logic when it comes to you. You just have this way of making my heart forget everything and choose you, every single time. 🫠❤️
My love for you is eternal. ♾️❤️
Sometimes, I wonder… how can I show you, how can I shower you with all the love I hold within my heart for you?
If loving you is a choice, then trust me, my heart has already made its decision for a lifetime. ❤️‍🩹
You know what the problem with you is? The more I get to know you, the more reasons you give me to fall for you… and the funny part is, I wasn't even looking for a way out. 😉❤️
I wish you could borrow my eyes for a moment and see yourself the way I see you. Maybe then you'd understand why, even on my busiest days, a little thought of you is enough to make me smile like an idiot. 🫣❤️
I don't just want to love you when you're happy, beautiful, and everything feels right. I want to be there when you're tired, when life gets difficult, when you don't have the words to explain what's wrong, and when all you need is someone who understands you without asking you to explain yourself a hundred times. 🫶🏻
And honestly, how am I supposed to act normal around someone who can make my heart race with just one message and leave me smiling at my phone like I've completely lost my mind? 😂❤️‍🔥
I may never find the perfect words to explain how much you mean to me, but I want my actions to tell you what my words sometimes cannot.
I want to be someone you can trust, someone you can lean on, someone who celebrates your dreams as if they were his own, and someone whose love makes your life feel a little softer and your heart a little lighter.
I don't promise that I can give you a perfect life, but I promise that I'll keep trying to make life more beautiful for you, in every way I can. ❤️
And if you ever ask me what I want from you in return for all this love… well, just give me that smile of yours, let me steal a little of your time, and maybe let me be the reason behind a few of those butterflies in your stomach. 😉🦋❤️
Because, honestly, loving you comes so naturally to me that sometimes I wonder whether my heart knew you long before I ever did. ❤️♾️


   </p>
      <div class="signature">With affection, always ♡</div>
      <p style="font-size:.72rem;color:#9b7883;margin-top:12px">whenever and wherever I will love like my breath till my last day</p>
    </article>
    <button class="btn dark" style="margin-top:28px" onclick="goTo('timeline')">Walk through our story ↓</button>
  </div>
</section>

<section id="timeline">
  <div class="section-inner">
    <p class="section-kicker">02 · Memories</p>
    <h2>Our story, one moment at a time</h2>
    <p class="lead">A relationship is made of tiny moments as much as big ones.build day by with lots of love by forgiving everything after huge moments bein together everything LOVE IS NOT ABOUT FINDING NEW PEOPLE IT IS ABOUT CHOOSING SAME PERSON AGAIN AND AGAIN AFTER ALL FIGHTS.</p>
    <div class="timeline">
      <div class="moment"><span class="date">Melted in her eyes ·</span><h3>Awww Monishaaa...</h3><p>When I saw you for frist time i felt a connection that i couldn't explain. I had feel for before at that moment,still remember how it started like whole garden of memories filled by you everywhere.</p></div>
      <div class="moment"><span class="date">Caught in her smile ·</span><h3>A memory that stays</h3><p>We had a good understanding from the start. It was like we were meant to be together, and every moment since has been a reminder of that.never seeked for perfection but looking forward for an better connection beyond all flaws</p></div>
      <div class="moment"><span class="date">Kingdom of Love ·</span><h3>My Queen</h3><p>You are my frist priority of all time and i have been in that way for a long peroid of time when i have started loving you.What else you need"You are already Queen of my kingdom" being ready to crowned and treated as a queen by me nad my famiy too.</p></div>
      <div class="moment"><span class="date">Towards Destiny ·</span><h3>The next page</h3><p>No need to predict the whole future. Leave space for good conversations, new memories, and taking things one step at a time.I won't leave at any cost whatever i will find a way to feel better becoz you have me;I won't make you feel low or bad for choosing me everyday i will be celebrating with My Queen , Queen of My Heart</p></div>
    </div>
    <p class="note">I could make the whole world as a garden for if you want flowers same I can burn the entire world to save you in any circumstance.</p>
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
      To my Monishaaa… my Angel, my Stressburster, my Luckycharm… 🩷🥹
Heyyy, my Angel… 💗
There’s something my heart has been wanting to tell you, something that goes beyond ordinary words. No matter how much I try to explain it, I don't think I'll ever be able to put everything I feel for you into words. But today, I want to try.
You are truly a gifted soul in my life. Even when everything around me felt like chaos, when life was full of pain, stress, and uncertainty, you were there like the brightest light in the darkest room. You brought light into my difficult days in ways you might not even realise. Sometimes, just having you in my life made everything feel a little less painful and a little more beautiful. ❤️‍🩹✨
Seeing you happy, peaceful, successful, and proud of yourself is one of the things I genuinely wish for the most. Your dreams matter to me, your happiness matters to me, and your peace matters to me. Whenever life gets difficult for you, I want you to know that you don't have to face everything alone. I'll be there for you, my Angel, however you need me.
I'll be in front of you when you need someone to stand up for you, beside you when you need someone to walk with you, and behind you when you need someone to support you quietly. Wherever you need me, that's where I'll try to be. 🫂💗
Sometimes, when I look back at my life, I realise how many things have changed over the years. In 2023, I went through my major operation. In 2024, I received my job offer from Finulent. In 2025, I received my offer from Enphase. Those were important milestones in my life, moments I'll always remember.
But somewhere between all those struggles, changes, and achievements, there was you.
The days we met, the moments we shared, and the way you became part of my life are memories I'll always hold close to my heart. I can't explain it with logic, but your presence became one of those beautiful things that changed something within me.
You became my Angel when I needed light, my Stressburster when I needed a smile, and my Luckycharm when I needed a little hope. 🩷✨
Thank you for making my life more beautiful, for teaching me to become more responsible, and for helping me understand love in ways I didn't know before.
And thank you for something even more precious… thank you for being part of the person I'm becoming.
I know we haven't always had the easiest journey. We've had our fights, misunderstandings, difficult moments, and days when we struggled to understand each other. I'm not going to pretend that everything has always been perfect between us. But through everything, I've come to understand that a meaningful bond isn't about never having problems; it's about learning from them and becoming better people.
You've forgiven my mistakes, corrected me when I was wrong, and helped me recognise the things I needed to change. I don't take that lightly, Angel. I know that trust, respect, and peace have to be built through our actions, not just our words. And I want to keep becoming someone who brings you comfort, understanding, happiness, and security.
Sometimes I think about how rare it is for two people to know each other's imperfect sides and still find reasons to care. Out of billions of people in this world, our paths crossed, and we became part of each other's stories. That's something I'll always be grateful for.
Like the sun and the moon, life has its bright days and its quiet, difficult nights. But our journey has taught me that love isn't just about romantic words, cute messages, or happy moments. It's also about understanding, patience, accountability, forgiveness, and learning how to treat each other better.
One of the most meaningful things to me is seeing us learn to support each other and stand up for each other. That's the kind of bond I hope we continue building — one where we both feel safe, respected, understood, and genuinely happy. 💞
Now, my Angel, can I tell you what my heart truly wishes for? 🥹❤️
I don't just want to be someone who says, "I love you."
I want to be someone whose actions make you feel loved.
I want to celebrate your smallest achievements as if they're the biggest victories. I want to listen when you have a thousand thoughts running through your mind. I want to see you chase your dreams, become successful, and build a life that makes you proud of yourself.
I want to be there for your silly moments, your happiest days, your stressful evenings, and even the days when you don't feel like explaining anything at all.
I want to keep learning how to love you in the ways that make you feel loved.
And if life gives us the chance to build a future together, I dream of something simple and beautiful — a peaceful little home, silly arguments over the smallest things, cooking together, laughing over nonsense, sharing our everyday stories, and ending our days knowing we have someone who genuinely cares. Maybe a little 2BHK filled with our laughter, our dreams, and our own kind of happiness. 🏡💗
I dream of being the person you can share your victories with, the person you can be completely yourself around, and the person who never makes you feel that you have to face every difficulty alone.
Not because I expect you to depend on me for everything, but because I want us to be two individuals who support each other, grow together, and make each other's lives a little more beautiful.
I know love cannot be forced, and I never want my feelings to become a burden on your heart. I want whatever grows between us to be genuine, peaceful, and chosen by both of us. Your happiness matters to me, and so does what your heart truly feels.
But if you ask me what my heart wishes for…
It wishes for more beautiful memories with you. More laughter. More understanding. More chances to make you smile. More moments where we choose patience over anger and understanding over assumptions. And, if someday your heart feels the same, the beautiful privilege of calling you my person for life. 🩷🥹
Monishaaa, my Angel, my Stressburster, my Luckycharm…
I don't know exactly what tomorrow holds for us, but I know what I wish to bring into it: a softer heart, a better version of myself, more patience, more understanding, and a love that feels like peace rather than pressure.
I want us to look back at our journey someday and realise that even the difficult chapters taught us how to build something healthier, stronger, and more beautiful.
I don't expect every day to be perfect. I don't expect us to agree on everything. I just hope that, if we get the chance to write our future together, we can do it with honesty, respect, care, and the willingness to understand each other even when things aren't easy.
And if someday you look at me and ask, "Why me?"
I'll probably smile and say…
"I don't know how to explain it, Monisha. My heart just found something in you that it never wanted to treat as ordinary. You became someone whose happiness matters to me, whose smile can make my day, and whose presence has left a beautiful mark on my life." 🥹💗
Maybe I can't promise you a life without difficulties, but I can promise to keep working on myself, to respect your feelings, to celebrate your growth, and to be honest about mine. I want my love to be something you can feel through the way I treat you, not just something you read in a message.
And if life gives us that chance, I would love to turn all these little dreams into our reality — one day, one memory, and one step at a time. 💌🌹
With LOL — Lots of Love, from a heart that genuinely wishes for your happiness, your peace, your success, and a beautiful future for you.
Always my Angel, my Stressburster, my Luckycharm… 🩷🫂
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
      Monishaaa, my Angel… 🥹❤️

You deserve kindness on your hardest days, laughter on your ordinary days, and someone who makes you feel loved, respected, and appreciated in the little things.

And if you choose me, I want to be that person for you. I want to make you smile when you're stressed, celebrate your little achievements, listen to your endless stories, and stand beside you through every high and low. Even during our fights, I want us to learn, understand each other, and choose kindness over ego.

I can't promise to be perfect, but I promise to keep trying to be better for us. I want to be your safe place, your biggest supporter, and the person you can be yourself with, without pretending or hiding your feelings.

**I don't know what the future holds, but if I could choose, I'd love to make a beautiful little life with you, filled with silly fights, endless laughter, random hugs, and lots of love.** 🫂💗

Thank you for being part of my story, my Luckycharm. And if you let me, I'd love to be part of your forever. 🩷🌷
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
    <div id="finaleMessage" class="hidden" style="font:2rem 'Dancing Script',cursive;margin-top:22px">If i could Hug you now it might be a endless cuddle but for now A thousand virtual hugs for you 🤗♡</div>
  </div>
</section>
</main>

<footer>A small handmade gift · Made with care ♡</footer>
<!-- Optional: add a song file named "our-song.mp3" in the same folder. -->
<audio id="ourSong" loop preload="none"><source src="our-song.mp3" type="audio/mpeg"></audio>
<iframe data-testid="embed-iframe" style="border-radius:12px" src="https://open.spotify.com/embed/track/4nSwWiwtieiNmRAjy9fEXN?utm_source=generator&si=da544ffe60014865" width="100%" height="352" frameBorder="0" allowfullscreen="" allow="autoplay; clipboard-write; encrypted-media; fullscreen; picture-in-picture" loading="lazy"></iframe>
<script>
const roseNotes = [
  "I hope today gives you a reason to smile, even if it's a tiny one. 🌹  Will Love you as always more and more being with you makes me feel am completely fulfilled, I can just hold you in my arms like my child as you are",
  "I will be there in all your moments,of you life instances. Being a successful partner in life, I will always support you and stand by your side. Keep being curious, brave, and wonderfully yourself. You have so much ahead of you. 🌷",
  "I hope we never run out of little things to laugh about. 😂 Being responsible for your happiness is something I take seriously. I won't let you inner child die, I will nurture it and protect it with all my heart.",
  "You deserve to be heard, understood, and treated with kindness—always. ♡ I will always be there to listen, to understand, and to love you for who you are. 🌸 I will be your constant companion through every season of life.",
  "May you get closer to the dreams you're working so hard for. ✨ I will always be your biggest cheerleader, supporting you in every step of your journey. 🌹 I will celebrate your victories and help you through the challenges.",
  "This rose has one job: to remind you that someone wanted to make your day a little sweeter. 💗 being my loavable person i will always be there to make you feel loved, cherished, and appreciated. 🌺 I will always be your safe haven, your confidant, and your biggest fan."
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
