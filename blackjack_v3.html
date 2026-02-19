<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0, maximum-scale=1.0">
<meta name="apple-mobile-web-app-capable" content="yes">
<meta name="apple-mobile-web-app-status-bar-style" content="black">
<title>Blackjack Trainer</title>
<style>
* { box-sizing: border-box; margin: 0; padding: 0; }
html, body {
  background: #0a0d0f;
  color: #fff;
  font-family: -apple-system, 'Helvetica Neue', Arial, sans-serif;
  min-height: 100%;
  -webkit-tap-highlight-color: transparent;
  -webkit-text-size-adjust: 100%;
}

/* SCREENS */
.screen { display: none; min-height: 100vh; flex-direction: column; }
.screen.active { display: flex; }

/* TOP BAR */
.top-bar {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 14px 16px;
  border-bottom: 1px solid rgba(255,255,255,0.07);
  background: rgba(0,0,0,0.5);
}
.back-btn {
  background: transparent;
  border: 1px solid rgba(255,255,255,0.15);
  border-radius: 8px;
  padding: 8px 14px;
  color: #888;
  font-size: 14px;
  cursor: pointer;
}
.top-title {
  font-size: 16px;
  font-weight: 600;
  color: #c9a84c;
  letter-spacing: 1px;
}
.top-acc { font-size: 13px; color: #444; min-width: 70px; text-align: right; }

/* FELT TABLE */
.felt {
  flex: 1;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  padding: 24px 16px 20px;
  background: radial-gradient(ellipse at center, #0e2918 0%, #091a0f 60%, #060f09 100%);
}
.zone { width: 100%; max-width: 460px; text-align: center; }
.zone-label {
  font-size: 11px;
  letter-spacing: 3px;
  color: #4a4a4a;
  text-transform: uppercase;
  margin-bottom: 10px;
}
.zone-label b { color: #c9a84c; font-weight: 600; }
.cards-row { display: flex; gap: 9px; justify-content: center; flex-wrap: wrap; }
.table-line {
  width: 160px; height: 1px;
  background: linear-gradient(to right, transparent, rgba(255,255,255,0.06), transparent);
}

/* PLAYING CARDS */
.card {
  width: 68px; height: 98px;
  border-radius: 8px;
  display: flex; flex-direction: column; justify-content: space-between;
  padding: 5px 6px;
  flex-shrink: 0;
  transition: transform 0.3s;
}
.card-face {
  background: #fff;
  border: 1px solid #ccc;
  box-shadow: 0 4px 16px rgba(0,0,0,0.6);
}
.card-back {
  background: repeating-linear-gradient(45deg,#1a1a2e,#1a1a2e 5px,#16213e 5px,#16213e 10px);
  border: 1px solid rgba(201,168,76,0.3);
  box-shadow: 0 4px 16px rgba(0,0,0,0.7);
  align-items: center; justify-content: center;
}
.card-back-diamond {
  font-size: 32px; color: rgba(201,168,76,0.5); line-height: 1;
}
.card-corner { font-weight: 700; line-height: 1.1; }
.card-corner .cr { font-size: 15px; }
.card-corner .cs { font-size: 11px; }
.card-mid { font-size: 28px; line-height: 1; text-align: center; }
.card-corner-bot { transform: rotate(180deg); font-weight: 700; line-height: 1.1; }
.card-corner-bot .cr { font-size: 15px; }
.card-corner-bot .cs { font-size: 11px; }
.red  { color: #d93025; }
.blk  { color: #1a1a1a; }

/* ACTION BUTTONS */
.actions { display: flex; flex-wrap: wrap; gap: 8px; justify-content: center; }
.act-btn {
  font-weight: 700;
  letter-spacing: 1px;
  text-transform: uppercase;
  border-radius: 10px;
  padding: 13px 14px;
  font-size: 13px;
  cursor: pointer;
  border-width: 1.5px;
  border-style: solid;
  min-width: 88px;
  transition: opacity 0.1s;
}
.act-btn:active { opacity: 0.6; }
.act-btn.dim { opacity: 0.18; pointer-events: none; }

/* FEEDBACK */
.feedback-box {
  border-radius: 12px;
  padding: 14px 16px;
  margin-top: 10px;
}
.feedback-header {
  display: flex;
  align-items: center;
  gap: 8px;
  margin-bottom: 7px;
  flex-wrap: wrap;
}
.feedback-verdict { font-size: 16px; font-weight: 700; }
.feedback-diff { font-size: 13px; color: #666; margin-left: auto; }
.feedback-text { font-size: 13px; line-height: 1.55; color: #aaa; }

/* RESULT */
.result-msg { text-align: center; font-size: 16px; font-weight: 600; padding: 10px; }
.next-btn {
  display: block; margin: 10px auto 0;
  background: rgba(201,168,76,0.12);
  border: 1.5px solid rgba(201,168,76,0.4);
  border-radius: 11px;
  padding: 15px 44px;
  color: #c9a84c;
  font-size: 14px; font-weight: 700;
  letter-spacing: 2px; text-transform: uppercase;
  cursor: pointer;
}
.next-btn:active { opacity: 0.7; }
.drill-badge {
  font-size: 12px; letter-spacing: 2px; text-transform: uppercase;
  color: #c9a84c; margin-bottom: 8px;
}

/* ── MENU ── */
#screen-menu {
  align-items: center; justify-content: center;
  padding: 40px 20px;
  background: #0a0d0f;
}
.logo-title {
  font-size: 42px; font-weight: 700;
  letter-spacing: 8px; color: #c9a84c;
  text-shadow: 0 0 40px rgba(201,168,76,0.25);
  line-height: 1;
}
.logo-sub {
  font-size: 11px; letter-spacing: 5px; color: #555;
  margin-top: 8px; text-transform: uppercase;
}
.gold-line {
  width: 100px; height: 1px;
  background: linear-gradient(to right, transparent, #c9a84c, transparent);
  margin: 14px auto;
}
.logo-rules { font-size: 10px; letter-spacing: 3px; color: #333; text-transform: uppercase; }
.session-pill {
  display: none;
  border: 1px solid rgba(201,168,76,0.2);
  border-radius: 99px; padding: 8px 22px;
  background: rgba(201,168,76,0.05); color: #c9a84c;
  font-size: 12px; letter-spacing: 2px;
  margin-bottom: 24px; text-align: center;
}
.menu-btns { width: 100%; max-width: 320px; display: flex; flex-direction: column; gap: 10px; margin-bottom: 16px; }
.menu-btn {
  width: 100%; border-radius: 12px; padding: 18px 20px;
  text-align: left; cursor: pointer;
  display: flex; align-items: center; gap: 14px;
  border: 1.5px solid rgba(255,255,255,0.08);
  background: rgba(255,255,255,0.02);
  color: #fff; transition: opacity 0.15s;
}
.menu-btn:active { opacity: 0.7; }
.menu-btn.primary {
  background: rgba(201,168,76,0.08);
  border-color: rgba(201,168,76,0.3);
}
.menu-btn-icon { font-size: 22px; }
.menu-btn-title { font-size: 16px; font-weight: 600; color: #f0f0f0; }
.menu-btn-sub { font-size: 11px; letter-spacing: 1px; color: #555; text-transform: uppercase; margin-top: 2px; }
.sec-btns { display: flex; gap: 10px; margin-bottom: 32px; }
.sec-btn {
  background: transparent;
  border: 1px solid rgba(255,255,255,0.1);
  border-radius: 8px; padding: 10px 20px;
  color: #666; font-size: 12px; letter-spacing: 1px;
  text-transform: uppercase; cursor: pointer;
}
.sec-btn:active { color: #aaa; }

/* ── STATS ── */
.stats-inner { max-width: 400px; width: 100%; margin: 0 auto; padding: 24px 16px 40px; }
.page-title { font-size: 26px; font-weight: 700; color: #c9a84c; margin-bottom: 2px; }
.page-sub { font-size: 10px; letter-spacing: 3px; color: #333; text-transform: uppercase; margin-bottom: 24px; }
.acc-ring {
  width: 130px; height: 130px; border-radius: 50%;
  border: 3px solid #555;
  display: flex; flex-direction: column; align-items: center; justify-content: center;
  background: rgba(0,0,0,0.3); margin: 0 auto 24px;
}
.acc-ring-pct { font-size: 36px; font-weight: 700; line-height: 1; }
.acc-ring-lbl { font-size: 9px; letter-spacing: 3px; color: #444; margin-top: 4px; text-transform: uppercase; }
.totals-row { display: flex; gap: 8px; margin-bottom: 20px; }
.total-card {
  flex: 1; text-align: center; padding: 12px 6px;
  background: rgba(255,255,255,0.02);
  border: 1px solid rgba(255,255,255,0.06); border-radius: 10px;
}
.total-card-num { font-size: 26px; font-weight: 700; }
.total-card-lbl { font-size: 9px; letter-spacing: 2px; color: #444; text-transform: uppercase; margin-top: 2px; }
.cat-box {
  padding: 16px; background: rgba(255,255,255,0.02);
  border: 1px solid rgba(255,255,255,0.06); border-radius: 12px; margin-bottom: 16px;
}
.cat-title { font-size: 9px; letter-spacing: 3px; color: #444; text-transform: uppercase; margin-bottom: 14px; }
.sbar { margin-bottom: 12px; }
.sbar-row { display: flex; justify-content: space-between; margin-bottom: 5px; }
.sbar-lbl { font-size: 11px; letter-spacing: 1px; text-transform: uppercase; color: #999; }
.sbar-pct { font-size: 13px; font-weight: 700; }
.sbar-pct-sub { font-size: 11px; color: #555; }
.sbar-track { height: 4px; border-radius: 99px; background: rgba(255,255,255,0.06); overflow: hidden; }
.sbar-fill { height: 100%; border-radius: 99px; }
.mistakes-box {
  padding: 16px; background: rgba(231,76,60,0.04);
  border: 1px solid rgba(231,76,60,0.14); border-radius: 12px;
}
.mistakes-title { font-size: 9px; letter-spacing: 3px; color: #e74c3c; text-transform: uppercase; margin-bottom: 12px; }
.mistake-item { margin-bottom: 10px; padding-bottom: 10px; }
.mistake-item:last-child { margin-bottom: 0; padding-bottom: 0; }
.mistake-hand { font-size: 13px; color: #888; }
.mistake-diff { font-size: 12px; color: #555; margin-top: 3px; }

/* ── STRATEGY REF ── */
.ref-inner { max-width: 540px; width: 100%; margin: 0 auto; padding: 20px 14px 40px; overflow-x: auto; }
.ref-section { font-size: 10px; letter-spacing: 3px; color: #c9a84c; text-transform: uppercase; margin-bottom: 7px; }
.ref-table { border-collapse: collapse; margin-bottom: 20px; }
.ref-th { font-size: 10px; color: #555; width: 32px; text-align: center; padding-bottom: 4px; }
.ref-th-lbl { font-size: 10px; color: #444; text-align: left; padding-right: 8px; padding-bottom: 4px; width: 52px; }
.ref-td-lbl { font-size: 11px; color: #666; padding-right: 8px; white-space: nowrap; }
.ref-cell { width: 32px; height: 26px; text-align: center; font-size: 10px; font-weight: 700; border: 1px solid rgba(255,255,255,0.04); }
.ref-legend { display: flex; gap: 10px; flex-wrap: wrap; margin-bottom: 16px; }
.ref-legend-item { display: flex; align-items: center; gap: 4px; }
.ref-legend-dot { width: 14px; height: 14px; border-radius: 3px; border: 1px solid; display: flex; align-items: center; justify-content: center; font-size: 8px; font-weight: 700; }
.ref-legend-name { font-size: 11px; color: #555; }
.ref-note {
  margin-top: 4px; padding: 12px; font-size: 11px;
  background: rgba(255,255,255,0.02);
  border: 1px solid rgba(255,255,255,0.06); border-radius: 8px;
  color: #444; line-height: 1.6;
}
</style>
</head>
<body>

<!-- MENU -->
<div id="screen-menu" class="screen active">
  <div style="text-align:center; margin-bottom:32px">
    <div class="logo-title">&#9824; BLACKJACK</div>
    <div class="logo-sub">Basic Strategy Trainer</div>
    <div class="gold-line"></div>
    <div class="logo-rules">6 Deck &middot; S17 &middot; DAS &middot; Late Surrender</div>
  </div>
  <div id="session-pill" class="session-pill"></div>
  <div class="menu-btns">
    <button class="menu-btn primary" id="btn-normal">
      <span class="menu-btn-icon" style="color:#c9a84c">&#9830;</span>
      <div>
        <div class="menu-btn-title">Normal Mode</div>
        <div class="menu-btn-sub">Full hand simulation</div>
      </div>
    </button>
    <button class="menu-btn" id="btn-drill">
      <span class="menu-btn-icon" style="color:#888">&#9671;</span>
      <div>
        <div class="menu-btn-title">Drill Mode</div>
        <div class="menu-btn-sub">Targeted edge cases</div>
      </div>
    </button>
  </div>
  <div class="sec-btns">
    <button class="sec-btn" id="btn-stats">Statistics</button>
    <button class="sec-btn" id="btn-ref">Strategy Chart</button>
  </div>
  <div style="font-size:10px; letter-spacing:3px; color:#252525; text-transform:uppercase; text-align:center">
    Keyboard: H &middot; S &middot; D &middot; P &middot; R
  </div>
</div>

<!-- GAME -->
<div id="screen-game" class="screen">
  <div class="top-bar">
    <button class="back-btn" id="btn-game-back">&#8592; Menu</button>
    <div class="top-title" id="game-mode-lbl">&#9824; NORMAL MODE</div>
    <div class="top-acc" id="game-acc-lbl">&#8212;</div>
  </div>
  <div class="felt">
    <div class="zone">
      <div class="zone-label" id="dealer-lbl">DEALER</div>
      <div class="cards-row" id="dealer-cards-el"></div>
    </div>
    <div class="table-line"></div>
    <div class="zone">
      <div class="drill-badge" id="drill-badge" style="display:none"></div>
      <div class="zone-label" id="player-lbl">YOUR HAND</div>
      <div class="cards-row" id="player-cards-el"></div>
    </div>
    <div class="zone" id="action-zone">
      <div class="actions" id="actions-el"></div>
      <div id="feedback-el"></div>
      <div id="result-el"></div>
    </div>
  </div>
</div>

<!-- STATS -->
<div id="screen-stats" class="screen">
  <div class="top-bar">
    <button class="back-btn" id="btn-stats-back">&#8592; Back</button>
    <div class="top-title">Statistics</div>
    <div></div>
  </div>
  <div class="stats-inner">
    <div class="page-title">Statistics</div>
    <div class="page-sub">Performance Overview</div>
    <div class="acc-ring" id="acc-ring-el">
      <div class="acc-ring-pct" id="acc-ring-pct">&#8212;</div>
      <div class="acc-ring-lbl">Accuracy</div>
    </div>
    <div class="totals-row">
      <div class="total-card"><div class="total-card-num" id="st-total" style="color:#aaa">0</div><div class="total-card-lbl">Total</div></div>
      <div class="total-card"><div class="total-card-num" id="st-correct" style="color:#2ecc71">0</div><div class="total-card-lbl">Correct</div></div>
      <div class="total-card"><div class="total-card-num" id="st-wrong" style="color:#e74c3c">0</div><div class="total-card-lbl">Incorrect</div></div>
    </div>
    <div class="cat-box">
      <div class="cat-title">By Category</div>
      <div id="bar-hard"></div>
      <div id="bar-soft"></div>
      <div id="bar-pair"></div>
    </div>
    <div id="mistakes-el"></div>
  </div>
</div>

<!-- STRATEGY REF -->
<div id="screen-ref" class="screen">
  <div class="top-bar">
    <button class="back-btn" id="btn-ref-back">&#8592; Back</button>
    <div class="top-title">Strategy Chart</div>
    <div></div>
  </div>
  <div class="ref-inner" id="ref-inner-el"></div>
</div>

<script>
/* ================================================================
   STRATEGY ENGINE
================================================================ */
var SUITS = ['S','H','D','C'];
var SUITS_DISPLAY = {'S':'&#9824;','H':'&#9829;','D':'&#9830;','C':'&#9827;'};
var RANKS = ['2','3','4','5','6','7','8','9','10','J','Q','K','A'];
var RANK_VALUES = {'2':2,'3':3,'4':4,'5':5,'6':6,'7':7,'8':8,'9':9,'10':10,'J':10,'Q':10,'K':10,'A':11};
var RED_SUITS = {'H':true,'D':true};

function makeCard(rank, suit) { return {rank:rank, suit:suit}; }
function cardValue(c) { return RANK_VALUES[c.rank]; }

function buildShoe(n) {
  var cards = [];
  var i, d, s, r;
  for (d = 0; d < n; d++) {
    for (s = 0; s < SUITS.length; s++) {
      for (r = 0; r < RANKS.length; r++) {
        cards.push(makeCard(RANKS[r], SUITS[s]));
      }
    }
  }
  for (i = cards.length - 1; i > 0; i--) {
    var j = Math.floor(Math.random() * (i + 1));
    var tmp = cards[i]; cards[i] = cards[j]; cards[j] = tmp;
  }
  return cards;
}

function handTotal(cards) {
  var t = 0, aces = 0, i;
  for (i = 0; i < cards.length; i++) {
    t += cardValue(cards[i]);
    if (cards[i].rank === 'A') aces++;
  }
  while (t > 21 && aces > 0) { t -= 10; aces--; }
  return t;
}

function isSoft(cards) {
  var t = 0, aces = 0, i;
  for (i = 0; i < cards.length; i++) {
    t += cardValue(cards[i]);
    if (cards[i].rank === 'A') aces++;
  }
  while (t > 21 && aces > 0) { t -= 10; aces--; }
  return aces > 0 && t <= 21;
}

function isPair(cards) {
  return cards.length === 2 && cards[0].rank === cards[1].rank;
}

function isBlackjack(cards, split) {
  return !split && cards.length === 2 && handTotal(cards) === 21;
}

function handCategory(cards) {
  if (isPair(cards)) return 'pair';
  if (isSoft(cards)) return 'soft';
  return 'hard';
}

/* Strategy tables */
var PAIR_SPLIT = {
  'A': {2:1,3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1},
  '8': {2:1,3:1,4:1,5:1,6:1,7:1,8:1,9:1,10:1,11:1},
  '5': {}, '10':{}, 'J':{}, 'Q':{}, 'K':{},
  '2': {2:1,3:1,4:1,5:1,6:1,7:1},
  '3': {2:1,3:1,4:1,5:1,6:1,7:1},
  '4': {5:1,6:1},
  '6': {2:1,3:1,4:1,5:1,6:1},
  '7': {2:1,3:1,4:1,5:1,6:1,7:1},
  '9': {2:1,3:1,4:1,5:1,6:1,8:1,9:1}
};

var SOFT_TABLE = {
  13:{2:'HIT',3:'HIT',4:'HIT',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'},
  14:{2:'HIT',3:'HIT',4:'HIT',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'},
  15:{2:'HIT',3:'HIT',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'},
  16:{2:'HIT',3:'HIT',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'},
  17:{2:'HIT',3:'DOUBLE',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'},
  18:{2:'STAND',3:'DOUBLE',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'STAND',8:'STAND',9:'HIT',10:'HIT',11:'HIT'},
  19:{2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'DOUBLE',7:'STAND',8:'STAND',9:'STAND',10:'STAND',11:'STAND'},
  20:{2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'STAND',8:'STAND',9:'STAND',10:'STAND',11:'STAND'},
  21:{2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'STAND',8:'STAND',9:'STAND',10:'STAND',11:'STAND'}
};

var HARD_TABLE = (function() {
  var h = {}, t, u;
  for (t = 4; t <= 8; t++) { h[t]={}; for(u=2;u<=11;u++) h[t][u]='HIT'; }
  h[9] ={2:'HIT',3:'DOUBLE',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'};
  h[10]={2:'DOUBLE',3:'DOUBLE',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'DOUBLE',8:'DOUBLE',9:'DOUBLE',10:'HIT',11:'HIT'};
  h[11]={2:'DOUBLE',3:'DOUBLE',4:'DOUBLE',5:'DOUBLE',6:'DOUBLE',7:'DOUBLE',8:'DOUBLE',9:'DOUBLE',10:'DOUBLE',11:'HIT'};
  h[12]={2:'HIT',3:'HIT',4:'STAND',5:'STAND',6:'STAND',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'};
  h[13]={2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'};
  h[14]={2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'HIT',8:'HIT',9:'HIT',10:'HIT',11:'HIT'};
  h[15]={2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'HIT',8:'HIT',9:'HIT',10:'SURRENDER',11:'HIT'};
  h[16]={2:'STAND',3:'STAND',4:'STAND',5:'STAND',6:'STAND',7:'HIT',8:'HIT',9:'SURRENDER',10:'SURRENDER',11:'SURRENDER'};
  for (t=17;t<=21;t++) { h[t]={}; for(u=2;u<=11;u++) h[t][u]='STAND'; }
  return h;
})();

function getOptimalAction(cards, dealer, canSplit, canDouble, canSurrender) {
  var uv = cardValue(dealer);
  var first2 = cards.length === 2;
  var t, a, row;
  if (canSplit && isPair(cards)) {
    var ss = PAIR_SPLIT[cards[0].rank] || {};
    if (ss[uv]) return 'SPLIT';
  }
  if (isSoft(cards)) {
    t = handTotal(cards);
    if (t < 13) t = 13;
    if (t > 21) t = 21;
    row = SOFT_TABLE[t] || {};
    a = row[uv] || 'STAND';
    if (a === 'DOUBLE' && (!canDouble || !first2)) a = 'HIT';
    return a;
  }
  t = handTotal(cards);
  if (t < 4) t = 4;
  if (t > 21) t = 21;
  row = HARD_TABLE[t] || {};
  a = row[uv] || (t >= 17 ? 'STAND' : 'HIT');
  if (a === 'SURRENDER' && (!canSurrender || !first2)) a = t <= 16 ? 'HIT' : 'STAND';
  if (a === 'DOUBLE' && (!canDouble || !first2)) a = 'HIT';
  return a;
}

function getExplanation(cards, dealer, action) {
  var uv = cardValue(dealer);
  var total = handTotal(cards);
  var soft = isSoft(cards);
  var q = soft ? 'Soft' : 'Hard';
  var ds = dealer.rank === 'A' ? 'Ace' : String(uv);
  var rank;
  if (isPair(cards)) {
    rank = cards[0].rank;
    if (action === 'SPLIT') {
      if (rank === 'A') return 'Always split Aces. Each ace gets a fresh card — two chances at 21 instead of a weak soft 12.';
      if (rank === '8') return 'Always split 8s. Hard 16 is the worst hand — two fresh starts are better.';
      return 'Splitting ' + rank + 's vs dealer ' + ds + ' creates two stronger starting hands.';
    } else {
      if (rank === '10' || rank === 'J' || rank === 'Q' || rank === 'K') return 'Never split 10-value cards. Hard 20 wins most of the time — never break it up.';
      if (rank === '5') return 'Never split 5s. Hard 10 is a powerful doubling hand. Two 5s are far weaker.';
      return 'Pair of ' + rank + 's vs dealer ' + ds + ': keep as ' + q + ' ' + total + ' and ' + action.toLowerCase() + '.';
    }
  }
  if (action === 'SURRENDER') {
    if (total === 16) return 'Hard 16 vs ' + ds + ': surrender loses 50% of your bet. Playing out loses more than 50% long-term.';
    if (total === 15) return 'Hard 15 vs 10: surrendering cuts your loss in half versus playing it out.';
    return q + ' ' + total + ' vs ' + ds + ': surrender is the least-negative option here.';
  }
  if (action === 'DOUBLE') return q + ' ' + total + ' vs dealer ' + ds + ': strong chance of a powerful hand. Double to maximize your edge.';
  if (action === 'STAND') {
    if (uv >= 2 && uv <= 6) return q + ' ' + total + ' vs dealer ' + ds + ': dealer has a bust card (2-6). Stand and let them take the risk.';
    return q + ' ' + total + ' vs dealer ' + ds + ': your total is strong enough — bust risk outweighs drawing another card.';
  }
  if (soft) return 'Soft ' + total + ' vs dealer ' + ds + ': you cannot bust on the next card. Hit — your total is too weak to stand.';
  return 'Hard ' + total + ' vs dealer ' + ds + ': your total needs improvement. Hitting gives a better chance than standing here.';
}

/* Drill scenarios */
var DRILLS = [
  {p:['8','8'],d:'10',desc:'Pair of 8s vs 10'},
  {p:['A','7'],d:'9', desc:'Soft 18 vs 9'},
  {p:['10','6'],d:'10',desc:'Hard 16 vs 10'},
  {p:['10','6'],d:'9', desc:'Hard 16 vs 9'},
  {p:['10','5'],d:'10',desc:'Hard 15 vs 10'},
  {p:['10','2'],d:'4', desc:'Hard 12 vs 4'},
  {p:['10','2'],d:'2', desc:'Hard 12 vs 2'},
  {p:['A','6'], d:'3', desc:'Soft 17 vs 3'},
  {p:['6','5'], d:'9', desc:'Hard 11 vs 9'},
  {p:['5','4'], d:'3', desc:'Hard 9 vs 3'},
  {p:['A','2'], d:'5', desc:'Soft 13 vs 5'},
  {p:['9','9'], d:'7', desc:'Pair 9s vs 7'},
  {p:['9','9'], d:'9', desc:'Pair 9s vs 9'},
  {p:['7','7'], d:'8', desc:'Pair 7s vs 8'},
  {p:['4','4'], d:'6', desc:'Pair 4s vs 6'},
  {p:['A','8'], d:'6', desc:'Soft 19 vs 6'},
  {p:['A','5'], d:'4', desc:'Soft 16 vs 4'},
  {p:['10','6'],d:'A', desc:'Hard 16 vs Ace'},
  {p:['A','A'], d:'5', desc:'Pair Aces vs 5'},
  {p:['K','K'], d:'6', desc:'Pair Kings vs 6'},
  {p:['6','6'], d:'2', desc:'Pair 6s vs 2'},
  {p:['2','2'], d:'8', desc:'Pair 2s vs 8'}
];

/* ================================================================
   GAME STATE
================================================================ */
var stats = {
  total:0, correct:0,
  hard:{total:0,correct:0},
  soft:{total:0,correct:0},
  pair:{total:0,correct:0},
  mistakes:[]
};

var shoe = buildShoe(6);
var playerCards = [];
var dealerCards = [];
var dealerRevealed = false;
var isSplitHand = false;
var canSplitF = true, canDoubleF = true, canSurrenderF = true;
var phase = 'awaiting';
var currentMode = 'normal';
var handCount = 0;
var lastFeedback = null;

function dealCard() {
  if (shoe.length < 52) shoe = buildShoe(6);
  return shoe.pop();
}

function getAvail() {
  var first2 = playerCards.length === 2;
  var acts = ['HIT', 'STAND'];
  if (canDoubleF && first2) acts.push('DOUBLE');
  if (canSplitF && first2 && isPair(playerCards)) acts.push('SPLIT');
  if (canSurrenderF && first2) acts.push('SURRENDER');
  return acts;
}

function inAvail(action) {
  var av = getAvail();
  for (var i = 0; i < av.length; i++) { if (av[i] === action) return true; }
  return false;
}

function descHand(cards) {
  var t = handTotal(cards);
  if (isPair(cards)) return 'Pair of ' + cards[0].rank + 's';
  if (isSoft(cards)) return 'Soft ' + t;
  return 'Hard ' + t;
}

function recordDecision(cat, ok, desc, chosen, optimal) {
  stats.total++;
  stats[cat].total++;
  if (ok) { stats.correct++; stats[cat].correct++; }
  else {
    stats.mistakes.push({desc:desc, chosen:chosen, optimal:optimal});
    if (stats.mistakes.length > 10) stats.mistakes.shift();
  }
}

/* ================================================================
   RENDERING
================================================================ */
function cardHTML(card, faceDown) {
  if (faceDown) {
    return '<div class="card card-back"><div class="card-back-diamond">&#9830;</div></div>';
  }
  var isRed = RED_SUITS[card.suit];
  var cls = isRed ? 'red' : 'blk';
  var sd = SUITS_DISPLAY[card.suit];
  return '<div class="card card-face">'
    + '<div class="card-corner ' + cls + '"><div class="cr">' + card.rank + '</div><div class="cs">' + sd + '</div></div>'
    + '<div class="card-mid ' + cls + '">' + sd + '</div>'
    + '<div class="card-corner-bot ' + cls + '"><div class="cr">' + card.rank + '</div><div class="cs">' + sd + '</div></div>'
    + '</div>';
}

function renderCards() {
  var pc = document.getElementById('player-cards-el');
  var dc = document.getElementById('dealer-cards-el');
  var i, html;
  html = '';
  for (i = 0; i < playerCards.length; i++) html += cardHTML(playerCards[i], false);
  pc.innerHTML = html;
  html = '';
  for (i = 0; i < dealerCards.length; i++) html += cardHTML(dealerCards[i], !dealerRevealed && i === 1);
  dc.innerHTML = html;
}

var ACT_META = {
  HIT:      {label:'[H] Hit',       color:'#2ecc71'},
  STAND:    {label:'[S] Stand',     color:'#e74c3c'},
  DOUBLE:   {label:'[D] Double',    color:'#f1c40f'},
  SPLIT:    {label:'[P] Split',     color:'#9b59b6'},
  SURRENDER:{label:'[R] Surrender', color:'#e67e22'}
};
var ACT_ORDER = ['HIT','STAND','DOUBLE','SPLIT','SURRENDER'];

function renderActions() {
  var el = document.getElementById('actions-el');
  if (phase !== 'awaiting') { el.innerHTML = ''; return; }
  var av = getAvail();
  var html = '', i, a, m, dis, bg, style;
  for (i = 0; i < ACT_ORDER.length; i++) {
    a = ACT_ORDER[i];
    m = ACT_META[a];
    dis = !inAvail(a);
    var r = parseInt(m.color.slice(1,3),16);
    var g = parseInt(m.color.slice(3,5),16);
    var b = parseInt(m.color.slice(5,7),16);
    bg = 'rgba(' + r + ',' + g + ',' + b + ',0.1)';
    style = 'background:' + bg + ';border-color:' + m.color + ';color:' + m.color;
    html += '<button class="act-btn' + (dis ? ' dim' : '') + '" data-action="' + a + '" style="' + style + '">' + m.label + '</button>';
  }
  el.innerHTML = html;
}

function renderZoneLabels() {
  var dl = document.getElementById('dealer-lbl');
  var pl = document.getElementById('player-lbl');
  var dt = dealerRevealed ? handTotal(dealerCards) : 0;
  dl.innerHTML = 'DEALER' + (dt ? ' &nbsp;<b>' + dt + '</b>' : '');
  var pDesc = playerCards.length > 0 ? descHand(playerCards) : '';
  var pTotal = handTotal(playerCards);
  pl.innerHTML = 'YOUR HAND' + (pDesc ? ' &nbsp;<b>' + pDesc + ' (' + pTotal + ')</b>' : '');
}

function renderFeedback(fb) {
  var el = document.getElementById('feedback-el');
  if (!fb) { el.innerHTML = ''; return; }
  var ok = fb.correct;
  var bg = ok ? 'rgba(46,204,113,0.07)' : 'rgba(231,76,60,0.07)';
  var bc = ok ? 'rgba(46,204,113,0.28)' : 'rgba(231,76,60,0.28)';
  var nc = ok ? '#2ecc71' : '#e74c3c';
  var diffHTML = ok ? '' : '<span class="feedback-diff">You: <span style="color:#e74c3c">' + fb.chosen + '</span> &rarr; Correct: <span style="color:#2ecc71">' + fb.optimal + '</span></span>';
  el.innerHTML = '<div class="feedback-box" style="background:' + bg + ';border:1px solid ' + bc + '">'
    + '<div class="feedback-header">'
    + '<span style="font-size:18px">' + (ok ? '&#10003;' : '&#10007;') + '</span>'
    + '<span class="feedback-verdict" style="color:' + nc + '">' + (ok ? 'Correct' : 'Incorrect') + '</span>'
    + diffHTML
    + '</div>'
    + '<div class="feedback-text">' + fb.explanation + '</div>'
    + '</div>';
}

function renderResult(msg) {
  var el = document.getElementById('result-el');
  if (!msg) { el.innerHTML = ''; return; }
  var color = (msg.indexOf('win') >= 0 || msg.indexOf('Blackjack') >= 0) ? '#c9a84c'
            : msg.indexOf('Push') >= 0 ? '#aaa' : '#e74c3c';
  el.innerHTML = '<div class="result-msg" style="color:' + color + '">' + msg + '</div>'
    + '<button class="next-btn" id="btn-next">Next Hand &rarr;</button>';
  var nb = document.getElementById('btn-next');
  if (nb) nb.addEventListener('click', nextHand);
}

function renderAccBar() {
  var el = document.getElementById('game-acc-lbl');
  if (stats.total === 0) { el.textContent = '—'; el.style.color = '#444'; return; }
  var acc = Math.round(stats.correct / stats.total * 100);
  el.textContent = acc + '% #' + handCount;
  el.style.color = acc >= 80 ? '#2ecc71' : acc >= 60 ? '#f1c40f' : '#e74c3c';
}

function renderAll(fb, resultMsg) {
  renderCards();
  renderZoneLabels();
  renderActions();
  renderFeedback(fb || null);
  renderResult(resultMsg || null);
  renderAccBar();
}

/* ================================================================
   GAME LOGIC
================================================================ */
function dealNormal() {
  shoe = buildShoe(6);
  var p1 = shoe.pop(), d1 = shoe.pop(), p2 = shoe.pop(), d2 = shoe.pop();
  playerCards = [p1, p2];
  dealerCards = [d1, d2];
  dealerRevealed = false;
  isSplitHand = false;
  canSplitF = true; canDoubleF = true; canSurrenderF = true;
  phase = 'awaiting'; lastFeedback = null;
  document.getElementById('drill-badge').style.display = 'none';
  renderAll(null, null);
  if (isBlackjack([p1, p2])) {
    dealerRevealed = true;
    phase = 'complete';
    var dbj = isBlackjack([d1, d2]);
    renderAll(null, dbj ? '&#129309; Push — Both Blackjack' : '&#127183; Blackjack! You win 3:2');
  }
}

function dealDrill() {
  var sc = DRILLS[Math.floor(Math.random() * DRILLS.length)];
  var i;
  playerCards = [];
  for (i = 0; i < sc.p.length; i++) {
    playerCards.push(makeCard(sc.p[i], SUITS[Math.floor(Math.random() * 4)]));
  }
  var dCard = makeCard(sc.d, SUITS[Math.floor(Math.random() * 4)]);
  dealerCards = [dCard, dealCard()];
  dealerRevealed = false; isSplitHand = false;
  canSplitF = true; canDoubleF = true; canSurrenderF = true;
  phase = 'awaiting'; lastFeedback = null;
  var badge = document.getElementById('drill-badge');
  badge.textContent = '&#127919; ' + sc.desc;
  badge.style.display = 'block';
  renderAll(null, null);
}

function nextHand() {
  document.getElementById('drill-badge').style.display = 'none';
  if (currentMode === 'normal') dealNormal();
  else dealDrill();
}

function doAction(action) {
  if (phase !== 'awaiting') return;
  if (!inAvail(action)) return;

  var dealer = dealerCards[0];
  var optimal = getOptimalAction(
    playerCards, dealer,
    canSplitF && isPair(playerCards),
    canDoubleF && playerCards.length === 2,
    canSurrenderF && playerCards.length === 2
  );
  var ok = action === optimal;
  var explanation = getExplanation(playerCards, dealer, optimal);
  var cat = handCategory(playerCards);
  recordDecision(cat, ok, descHand(playerCards), action, optimal);
  handCount++;
  phase = 'feedback';
  lastFeedback = {chosen:action, optimal:optimal, correct:ok, explanation:explanation};
  renderAll(lastFeedback, null);

  setTimeout(function() {
    var nc, newCards;
    if (action === 'SURRENDER') {
      phase = 'complete';
      renderAll(lastFeedback, '&#9729; Surrendered — Half bet saved');
      return;
    }
    if (action === 'STAND') {
      revealDealer(playerCards.slice(), lastFeedback);
      return;
    }
    if (action === 'DOUBLE') {
      nc = dealCard();
      newCards = playerCards.concat([nc]);
      playerCards = newCards;
      if (handTotal(playerCards) > 21) {
        dealerRevealed = true; phase = 'complete';
        renderAll(lastFeedback, '&#128165; Busted!');
      } else {
        revealDealer(playerCards.slice(), lastFeedback);
      }
      return;
    }
    if (action === 'HIT') {
      nc = dealCard();
      newCards = playerCards.concat([nc]);
      playerCards = newCards;
      if (handTotal(playerCards) > 21) {
        dealerRevealed = true; phase = 'complete';
        renderAll(lastFeedback, '&#128165; Busted!');
      } else {
        phase = 'awaiting';
        canSurrenderF = false; canDoubleF = false;
        renderAll(null, null);
      }
      return;
    }
    if (action === 'SPLIT') {
      nc = dealCard();
      var first = playerCards[0];
      playerCards = [first, nc];
      isSplitHand = true;
      canSplitF = first.rank !== 'A';
      canDoubleF = true; canSurrenderF = false;
      phase = 'awaiting';
      renderAll(null, null);
      return;
    }
  }, 850);
}

function revealDealer(pCards, fb) {
  dealerRevealed = true;
  while (handTotal(dealerCards) < 17) dealerCards = dealerCards.concat([dealCard()]);
  var dt = handTotal(dealerCards), pt = handTotal(pCards);
  var msg;
  if (dt > 21)     msg = '&#127881; Dealer busted! You win with ' + pt;
  else if (pt > dt) msg = '&#9989; You win! ' + pt + ' beats ' + dt;
  else if (pt === dt) msg = '&#129309; Push &mdash; ' + pt + ' ties ' + dt;
  else              msg = '&#10060; Dealer wins &mdash; ' + dt + ' beats ' + pt;
  phase = 'complete';
  renderAll(fb, msg);
}

/* ================================================================
   STATS RENDERING
================================================================ */
function renderStats() {
  var acc = stats.total > 0 ? Math.round(stats.correct / stats.total * 100) : 0;
  var ring = acc >= 80 ? '#2ecc71' : acc >= 60 ? '#f1c40f' : '#e74c3c';
  var ringEl = document.getElementById('acc-ring-el');
  ringEl.style.borderColor = ring;
  ringEl.style.boxShadow = '0 0 28px ' + ring + '44';
  var pctEl = document.getElementById('acc-ring-pct');
  pctEl.textContent = stats.total > 0 ? acc + '%' : '—';
  pctEl.style.color = ring;
  document.getElementById('st-total').textContent = stats.total;
  document.getElementById('st-correct').textContent = stats.correct;
  document.getElementById('st-wrong').textContent = stats.total - stats.correct;

  function bar(id, label, correct, total) {
    var pct = total > 0 ? Math.round(correct / total * 100) : 0;
    var c = pct >= 80 ? '#2ecc71' : pct >= 60 ? '#f1c40f' : '#e74c3c';
    document.getElementById(id).innerHTML =
      '<div class="sbar">'
      + '<div class="sbar-row"><span class="sbar-lbl">' + label + '</span>'
      + '<span class="sbar-pct" style="color:' + c + '">' + pct + '% <span class="sbar-pct-sub">(' + correct + '/' + total + ')</span></span></div>'
      + '<div class="sbar-track"><div class="sbar-fill" style="width:' + pct + '%;background:' + c + '"></div></div>'
      + '</div>';
  }
  bar('bar-hard', 'Hard Totals', stats.hard.correct, stats.hard.total);
  bar('bar-soft', 'Soft Totals', stats.soft.correct, stats.soft.total);
  bar('bar-pair', 'Pairs', stats.pair.correct, stats.pair.total);

  var mel = document.getElementById('mistakes-el');
  if (stats.mistakes.length === 0) { mel.innerHTML = ''; return; }
  var recent = stats.mistakes.slice().reverse().slice(0, 5);
  var html = '<div class="mistakes-box"><div class="mistakes-title">Recent Mistakes</div>';
  var i, m;
  for (i = 0; i < recent.length; i++) {
    m = recent[i];
    html += '<div class="mistake-item" style="' + (i < recent.length - 1 ? 'border-bottom:1px solid rgba(255,255,255,0.04)' : '') + '">'
      + '<div class="mistake-hand">' + m.desc + '</div>'
      + '<div class="mistake-diff">You chose <span style="color:#e74c3c">' + m.chosen + '</span> &rarr; Correct: <span style="color:#2ecc71">' + m.optimal + '</span></div>'
      + '</div>';
  }
  mel.innerHTML = html + '</div>';
}

/* ================================================================
   STRATEGY REFERENCE
================================================================ */
var ACT_COLORS = {HIT:'#2ecc71',STAND:'#e74c3c',DOUBLE:'#f1c40f',SPLIT:'#9b59b6',SURRENDER:'#e67e22'};
var ACT_ABBR   = {HIT:'H',STAND:'S',DOUBLE:'D',SPLIT:'SP',SURRENDER:'R'};
var UCV = [2,3,4,5,6,7,8,9,10,11];
var UCL = ['2','3','4','5','6','7','8','9','10','A'];

function buildRefHTML() {
  var i, t, u, a, c, r, row, rows, html;

  var hardRows = [];
  for (t = 8; t <= 17; t++) {
    row = [];
    for (u = 0; u < UCV.length; u++) {
      a = (HARD_TABLE[t] || {})[UCV[u]] || (t >= 17 ? 'STAND' : 'HIT');
      row.push(a);
    }
    hardRows.push({label:'Hard '+t, row:row});
  }

  var softRows = [];
  var softTotals = [13,14,15,16,17,18,19];
  for (i = 0; i < softTotals.length; i++) {
    t = softTotals[i];
    row = [];
    for (u = 0; u < UCV.length; u++) {
      a = (SOFT_TABLE[t] || {})[UCV[u]] || 'STAND';
      row.push(a);
    }
    softRows.push({label:'Soft '+t, row:row});
  }

  var pairDefs = [
    ['A','A-A'],['2','2-2'],['3','3-3'],['4','4-4'],
    ['5','5-5'],['6','6-6'],['7','7-7'],['8','8-8'],['9','9-9']
  ];
  var pairRows = [];
  for (i = 0; i < pairDefs.length; i++) {
    var rank = pairDefs[i][0], label = pairDefs[i][1];
    var ss = PAIR_SPLIT[rank] || {};
    row = [];
    for (u = 0; u < UCV.length; u++) {
      if (ss[UCV[u]]) a = 'SPLIT';
      else if (rank === '9') a = 'STAND';
      else a = 'HIT';
      row.push(a);
    }
    pairRows.push({label:label, row:row});
  }

  function tableHTML(title, rows) {
    var h = '<div class="ref-section">' + title + '</div><div style="overflow-x:auto"><table class="ref-table">';
    h += '<thead><tr><th class="ref-th-lbl">Hand</th>';
    for (i = 0; i < UCL.length; i++) h += '<th class="ref-th">' + UCL[i] + '</th>';
    h += '</tr></thead><tbody>';
    var ri;
    for (ri = 0; ri < rows.length; ri++) {
      r = rows[ri];
      h += '<tr><td class="ref-td-lbl">' + r.label + '</td>';
      for (u = 0; u < r.row.length; u++) {
        a = r.row[u]; c = ACT_COLORS[a] || '#555';
        var rr = parseInt(c.slice(1,3),16), gg = parseInt(c.slice(3,5),16), bb = parseInt(c.slice(5,7),16);
        h += '<td class="ref-cell" style="background:rgba('+rr+','+gg+','+bb+',0.12);color:'+c+'">' + ACT_ABBR[a] + '</td>';
      }
      h += '</tr>';
    }
    h += '</tbody></table></div>';
    return h;
  }

  var actList = ['HIT','STAND','DOUBLE','SPLIT','SURRENDER'];
  var legend = '<div class="ref-legend">';
  for (i = 0; i < actList.length; i++) {
    a = actList[i]; c = ACT_COLORS[a];
    var rr2 = parseInt(c.slice(1,3),16), gg2 = parseInt(c.slice(3,5),16), bb2 = parseInt(c.slice(5,7),16);
    legend += '<div class="ref-legend-item"><div class="ref-legend-dot" style="background:rgba('+rr2+','+gg2+','+bb2+',0.12);border-color:'+c+';color:'+c+'">' + ACT_ABBR[a] + '</div><span class="ref-legend-name">'+a+'</span></div>';
  }
  legend += '</div>';

  return '<div style="font-size:10px;letter-spacing:3px;color:#333;text-transform:uppercase;margin-bottom:14px">6 Deck &middot; S17 &middot; DAS &middot; Late Surrender</div>'
    + legend
    + tableHTML('HARD TOTALS', hardRows)
    + tableHTML('SOFT TOTALS', softRows)
    + tableHTML('PAIRS', pairRows)
    + '<div class="ref-note"><b style="color:#555">Rules:</b> Double on any 2 cards &middot; Double after split (DAS) &middot; Late surrender &middot; No re-split aces</div>';
}

/* ================================================================
   SCREEN NAVIGATION
================================================================ */
function showScreen(name) {
  var screens = document.querySelectorAll('.screen');
  var i;
  for (i = 0; i < screens.length; i++) screens[i].classList.remove('active');
  document.getElementById('screen-' + name).classList.add('active');
  if (name === 'stats') renderStats();
  if (name === 'ref') {
    var ri = document.getElementById('ref-inner-el');
    if (!ri.innerHTML) ri.innerHTML = buildRefHTML();
  }
  if (name === 'menu') {
    var pill = document.getElementById('session-pill');
    if (stats.total > 0) {
      var acc = Math.round(stats.correct / stats.total * 100);
      pill.textContent = 'SESSION: ' + acc + '% accuracy (' + stats.total + ' decisions)';
      pill.style.display = 'block';
    }
  }
  window.scrollTo(0, 0);
}

/* ================================================================
   EVENT LISTENERS — all attached via JS, no inline onclick
================================================================ */
function ready(fn) {
  if (document.readyState !== 'loading') fn();
  else document.addEventListener('DOMContentLoaded', fn);
}

ready(function() {
  /* Menu buttons */
  document.getElementById('btn-normal').addEventListener('click', function() {
    currentMode = 'normal'; handCount = 0;
    document.getElementById('game-mode-lbl').textContent = '\u2660 NORMAL MODE';
    showScreen('game');
    dealNormal();
  });
  document.getElementById('btn-drill').addEventListener('click', function() {
    currentMode = 'drill'; handCount = 0;
    document.getElementById('game-mode-lbl').textContent = '\u2660 DRILL MODE';
    showScreen('game');
    dealDrill();
  });
  document.getElementById('btn-stats').addEventListener('click', function() { showScreen('stats'); });
  document.getElementById('btn-ref').addEventListener('click', function() { showScreen('ref'); });

  /* Back buttons */
  document.getElementById('btn-game-back').addEventListener('click', function() { showScreen('menu'); });
  document.getElementById('btn-stats-back').addEventListener('click', function() { showScreen('menu'); });
  document.getElementById('btn-ref-back').addEventListener('click', function() { showScreen('menu'); });

  /* Action buttons — delegated on parent */
  document.getElementById('actions-el').addEventListener('click', function(e) {
    var btn = e.target;
    while (btn && btn !== this) {
      if (btn.dataset && btn.dataset.action) { doAction(btn.dataset.action); return; }
      btn = btn.parentNode;
    }
  });

  /* Keyboard (desktop) */
  document.addEventListener('keydown', function(e) {
    if (!document.getElementById('screen-game').classList.contains('active')) return;
    if (phase !== 'awaiting') return;
    var map = {h:'HIT', s:'STAND', d:'DOUBLE', p:'SPLIT', r:'SURRENDER'};
    var a = map[e.key.toLowerCase()];
    if (a && inAvail(a)) doAction(a);
  });
});
</script>
</body>
</html>
