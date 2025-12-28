---
layout: default
title: Meme
nav_order: 3
permalink: /meme/
---

# Meme
_Brainrot Meets High-Brow: A Loopy Mutation_

---

<img
  src="{{ '/assets/images/meme.gif' | relative_url }}"
  alt="Static image of a golden retriever puppy shaking off water; the image itself jitters while the puppy remains still."
  style="width:50%; height:auto;">

---

## **Tiny Moves** by Bleachers  
<iframe allow="encrypted-media *; fullscreen *; clipboard-write"
        frameborder="0" 
        height="175" 
        style="width:100%;max-width:660px;overflow:hidden;border-radius:10px;" 
        sandbox="allow-forms allow-popups allow-same-origin allow-scripts allow-storage-access-by-user-activation allow-top-navigation-by-user-activation" 
        src="https://embed.music.apple.com/song/tiny-moves/1712730492">
</iframe>

---

<div
  class="embed-container"
  style="max-width:670px; margin:0 auto;"
  aria-label="Chart: Market yield on U.S. Treasury securities at 10-year constant maturity, quoted on an investment basis.">
  <iframe
    src="https://fred.stlouisfed.org/graph/graph-landing.php?g=1PihU&width=670&height=475"
    title="Chart: Market yield on U.S. Treasury securities at 10-year constant maturity, quoted on an investment basis."
    scrolling="no"
    frameborder="0"
    style="overflow:hidden; width:670px; height:525px;"
    loading="lazy">
    Chart: Market yield on U.S. Treasury securities at 10-year constant maturity, quoted on an investment basis.
  </iframe>
</div>

<script src="https://fred.stlouisfed.org/graph/js/embed.js" type="text/javascript"></script>

---

<div style="height:480px">
  <div id="tv_chart"></div>
</div>

<script src="https://s3.tradingview.com/tv.js"></script>
<script>
new TradingView.widget({
  "container_id": "tv_chart",
  "symbol": "TVC:US10Y",
  "interval": "D",
  "autosize": true
});
</script>

---

<iframe 
    src="https://fred.stlouisfed.org/graph/graph-v1.php?g=1v6Vj&width=600&height=400" 
    style="border:none;" 
    width="600" 
    height="450" 
    allowfullscreen>
</iframe>

---

<div id="te-widget-chart" style="width:100%; height:400px;">
    <script src="https://widgets.tradingeconomics.com/ec.js" async>
        {
            "symbol": "INTEREST RATE",
            "country": "united states",
            "height": 400,
            "width": "100%",
            "range": "max"
        }
    </script>
</div>

---

<div class="tradingview-widget-container">
  <div id="tradingview_chart"></div>
  <script type="text/javascript" src="https://s3.tradingview.com/tv.js"></script>
  <script type="text/javascript">
  new TradingView.widget({
    "width": "100%",
    "height": 400,
    "symbol": "ECONOMICS:USINTR",
    "interval": "D",
    "timezone": "Etc/UTC",
    "theme": "light",
    "style": "2",
    "locale": "en",
    "toolbar_bg": "#f1f3f6",
    "enable_publishing": false,
    "hide_top_toolbar": true,
    "save_image": false,
    "container_id": "tradingview_chart"
  });
  </script>
</div>

---

<iframe src="https://ourworldindata.org/grapher/interest-rates-on-government-bonds" 
        loading="lazy" 
        style="width: 100%; height: 600px; border: 0px none;">
</iframe>

---

> <div class="hindi" lang="hi" dir="ltr">
>   <div class="verses">
>     <div class="line">किस ने भीगे हुए बालों से ये झटका पानी</div>
>     <div class="line">झूम कर आई घटा टूट के बरसा पानी</div>
>     <div class="poet">— आरज़ू लखनवी</div>
>   </div>
> </div>

---

<!-- Federal Funds Rate Chart (1954-Present) -->
<iframe src="https://fred.stlouisfed.org/graph/graph-landing.php?g=1trSv&width=670&height=475" 
        scrolling="no" 
        frameborder="0" 
        style="overflow:hidden; width:670px; height:525px;" 
        allowTransparency="true" 
        loading="lazy">
</iframe>

---

<!-- Fed Funds Rate Chart -->
<iframe src="https://www.macrotrends.net/assets/php/chart.php?t=fed-funds-rate&s=fed-funds-rate" 
        width="100%" 
        height="600" 
        frameborder="0" 
        scrolling="no">
</iframe>

---

<!-- 10-Year Treasury Yield (since 1962) -->
<iframe src="https://www.macrotrends.net/assets/php/chart.php?t=10-year-treasury&s=10-year-treasury" 
        width="100%" 
        height="600" 
        frameborder="0">
</iframe>

---

<!-- Investing.com HTML5 chart widget (example parameters) -->
<iframe
  height="480"
  width="650"
  src="https://ssltvc.investing.com/?pair_ID=8849&height=480&width=650&interval=300&plotStyle=candles&domain_ID=6&lang_ID=1&timezone_ID=21"
  frameborder="0"
  allowtransparency="true"
  marginwidth="0"
  marginheight="0">
</iframe>

---

<div style="max-width:900px">
  <canvas id="termSofrChart" height="120"></canvas>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/papaparse@5.4.1/papaparse.min.js"></script>
<script>
  const CSV_URL = "https://www.federalreserve.gov/econres/notes/feds-notes/FED_Note_Term_SOFR.csv";

  // You may need to inspect the CSV headers once to set these correctly:
  const DATE_COL = "Date";
  const VALUE_COL = "Term SOFR";  // adjust to the actual header name in the file

  fetch(CSV_URL).then(r => r.text())
    .then(t => Papa.parse(t, { header:true, dynamicTyping:true }).data)
    .then(rows => rows.filter(r => r[DATE_COL] && r[VALUE_COL] != null))
    .then(rows => {
      new Chart(document.getElementById("termSofrChart"), {
        type: "line",
        data: {
          labels: rows.map(r => r[DATE_COL]),
          datasets: [{ label: VALUE_COL, data: rows.map(r => r[VALUE_COL]) }]
        },
        options: { parsing: false, animation: false }
      });
    });
</script>

---

<iframe
  src="https://stooq.com/q/?s=10yusy.b"
  width="900"
  height="650"
  frameborder="0">
</iframe>

---

<div style="max-width:900px">
  <canvas id="tsyChart" height="120"></canvas>
</div>

<script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
<script src="https://cdn.jsdelivr.net/npm/papaparse@5.4.1/papaparse.min.js"></script>
<script>
  // Treasury provides CSV/XML feeds for daily rates (see their “Interest Rates” data pages).
  // Replace CSV_URL with the specific Treasury CSV feed you want (e.g., yield curve or daily treasury rates).
  const CSV_URL = "PASTE_TREASURY_CSV_FEED_URL_HERE";

  // Update these for the chosen dataset:
  const DATE_COL = "Date";
  const VALUE_COL = "10 Yr";   // example label — adjust to the actual column header in the CSV

  fetch(CSV_URL)
    .then(r => r.text())
    .then(text => Papa.parse(text, { header: true, dynamicTyping: true }).data)
    .then(rows => rows.filter(r => r[DATE_COL] && r[VALUE_COL] != null))
    .then(rows => {
      const labels = rows.map(r => r[DATE_COL]);
      const data = rows.map(r => r[VALUE_COL]);

      new Chart(document.getElementById("tsyChart"), {
        type: "line",
        data: { labels, datasets: [{ label: VALUE_COL, data }] },
        options: { parsing: false, animation: false }
      });
    });
</script>

---

<!-- US Interest Rate Historical Chart -->
<iframe src="https://d3fy651gv2fhd3.cloudfront.net/embed/?s=unitedstaintererate&v=202512261048V20230410&d1=19250101&h=300&w=600" 
        width="600" 
        height="350" 
        frameborder="0" 
        scrolling="no">
</iframe>

---

<!-- TradingView Advanced Chart Widget -->
<div class="tradingview-widget-container">
  <div class="tradingview-widget-container__widget"></div>
  <script type="text/javascript" src="https://s3.tradingview.com/external-embedding/embed-widget-advanced-chart.js" async>
  {
    "width": "980",
    "height": "610",
    "symbol": "ECONOMICS:USINTR",
    "interval": "M",
    "timezone": "America/New_York",
    "theme": "light",
    "style": "1",
    "locale": "en",
    "enable_publishing": false,
    "range": "ALL",
    "allow_symbol_change": false,
    "calendar": false,
    "support_host": "https://www.tradingview.com"
  }
  </script>
</div>

---

<!-- Or for 10-Year Treasury (back to 1962) -->
<iframe src="https://fred.stlouisfed.org/graph/graph-landing.php?g=DGS10&width=670&height=475" 
        scrolling="no" 
        frameborder="0" 
        style="overflow:hidden; width:670px; height:525px;" 
        allowTransparency="true">
</iframe>

---

<div class="urdu" lang="ur" dir="rtl">
  <div class="verses">
    <div class="misra">حاصلِ کن ہے یہ جہانِ خراب</div>
    <div class="misra">یہی ممکن تھا اتنی عجلت میں</div>
    <div class="poet">— جون ایلیا</div>
  </div>
</div>

---

🦗🦗  
   
🚪
