<!DOCTYPE html>
<html>
<head>
  <meta charset="utf-8">
  <title>猴硐的過去與現在</title>
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
  <style>
    body {
      background-image: url('B.jpeg');
      background-size: cover;
      background-repeat: no-repeat;
      background-attachment: fixed;
      background-position: center;
    }
    body { margin: 0; font-family: sans-serif; }
    header {
  padding: 1em;
  background-image: url('B.jpeg');
  background-size: cover;
  background-position: center;
  color: black;
  text-align: center;
  font-size: 1.5em;
  font-weight: bold;
}
    .description {
  padding: 1em;
  background-image: url('B.jpeg');
  background-size: cover;
  background-position: center;
  font-size: 1em;
  text-align: center;
  color: black;
}
    #map { height: calc(100vh - 180px); }
    .info-panel {
      background: white;
      padding: 10px;
      max-width: 90vw;
      width: 100%;
      font-size: 14px;
      word-wrap: break-word;
      overflow-wrap: break-word;
      box-sizing: border-box;
    }
    .photo-toggle {
      margin: 5px 5px 0 0;
      padding: 5px 10px;
    }
    .photo-toggle.visited {
      background-color: #cfc;
    }
    .marker-visited {
      filter: hue-rotate(180deg);
    }
    #completionMessage, #introMessage {
      display: none;
      position: fixed;
      top: 30%;
      left: 50%;
      transform: translate(-50%, -50%);
      background: white;
      padding: 20px;
      border: 2px solid black;
      font-size: 18px;
      z-index: 9999;
      text-align: center;
    }
    #introMessage button {
      margin-top: 10px;
      padding: 10px 20px;
      font-size: 16px;
    }
    footer {
  background-image: url('B.jpeg');
  background-size: cover;
  background-position: center;
  padding: 1em;
  font-size: 12px;
  text-align: left;
  color: black;
}
    .glow-line {
      stroke: green;
      stroke-width: 6;
      stroke-dasharray: 5, 10;
      filter: none;
      transition: filter 0.3s ease;
      pointer-events: stroke;
    }
    .glow-line.hover-effect {
      filter: drop-shadow(0 0 6px #0f0) drop-shadow(0 0 10px #0f0);
      cursor: pointer;
    }
    .glow-line-solid {
      stroke-width: 6;
      filter: none;
      transition: filter 0.3s ease;
      pointer-events: stroke;
    }
    .glow-line-solid.hover-effect {
      filter: drop-shadow(0 0 6px #333) drop-shadow(0 0 10px #000);
      cursor: pointer;
    }
  </style>
</head>
<body>
  <header>猴硐的過去與現在</header>
  <div class="description">
    點選地圖上的地點，可切換照片對照過去與現在，並閱讀相關故事。
  </div>
  <div id="map"></div>
  <div id="introMessage">
    <p>民國79年礦場熄燈後，猴硐靜了下來。<br>但故事沒散去，只是藏進山裡，等你來打開。</p>
    <button onclick="startExperience()">開始探索</button>
  </div>
  <div id="completionMessage">
  <p>你完成了所有地點的探索！</p>
  <p>記憶已翻開，歡迎親自走進猴硐，看看山裡還留著的故事。</p>
  <p>故事在地圖上展開，更在你的腳步中浮現。別讓記憶只停在螢幕，實地走一趟，讓猴硐的風聲、礦道與人情，成為你自己的體驗。</p>
  <p>🚉 <strong>交通方式</strong>：搭乘台鐵至「猴硐車站」，出站後即可抵達主要導覽範圍。</p>
  <p>🗺️ <a href="https://maps.google.com/?q=猴硐車站" target="_blank">查看 Google 地圖</a></p>
</div>
  <footer>
    <strong>一、參考使用（非創用CC授權，僅作為非商業文化用途引用）</strong><br>
    書籍文字參考：《黑暗的世界：猴硐礦工回憶錄》，作者：周朝南、李依倪，出版者：周朝南；媒體來源：聯合報新聞影像與資料；歌詞引用：《猴硐的一板橋》，演唱：張羽偉＆焦炭樂團，專輯《張羽偉專輯4－輕輕鬆鬆談戀愛》，出版：喜瑪拉雅音樂事業股份有限公司<br><br>
    <strong>二、創用CC授權使用（CC BY-NC 3.0 TW）</strong><br>
    圖片〈復興礦〉／提供者：周朝南；吊橋文字／撰寫者：柯宛伶；圖片〈瑞三鑛業公司中元普渡祭祀-11〉／來源：文化部國家文化記憶庫，創作者：周朝南，撰寫者：王新衡，資料管理單位：新北市政府文化局；圖片〈瑞三鑛業機關車庫礦車行經-1〉／來源：文化記憶庫，創作者：周朝南，撰寫者：王新衡；圖片〈民國60年代復興坑機關車出坑照〉／來源：文化記憶庫，圖片創作者：周朝南，文字撰寫者：李依倪；文字〈臺灣煤礦耆老訪談－吳寶銀〉／資料來源：109年度新北文化記憶庫礦業文史資材徵集與數位化建置計畫，訪談者：王新衡；圖片〈瑞三福利餐廳及工寮〉／來源：文化記憶庫，創作者：周朝南，撰寫者：王新衡
  </footer>

  <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>
  <script>
    function startExperience() {
      document.getElementById('introMessage').style.display = 'none';
    }

    function checkCompletion() {
      if (viewedPastSet.size === locations.length) {
        document.getElementById('completionMessage').style.display = 'block';
      }
    }

    function togglePhoto(title, time) {
      var img = document.getElementById('img-' + title);
      var story = document.getElementById('story-' + title);
      var loc = locations.find(l => l.title === title);
      if (!img || !story || !loc) return;

      if (time === 'now') {
        img.src = loc.nowImg;
        story.style.display = 'none';
      } else if (time === 'past') {
        img.src = loc.pastImg;
        story.innerHTML = loc.pastStory || '';
        story.style.display = 'block';
        viewedPastSet.add(loc.title);

        var pastBtn = document.getElementById(`past-btn-${loc.title}-past`);
        if (pastBtn) pastBtn.classList.add('visited');

        var markerElem = markerRefs[loc.title]?.getElement();
        if (markerElem) markerElem.classList.add('marker-visited');

        checkCompletion();
      }
    }

    document.addEventListener('DOMContentLoaded', function () {
      document.getElementById('introMessage').style.display = 'block';

      window.viewedPastSet = new Set();
      window.markerRefs = {};
      window.locations = [
        { coords: [25.08163, 121.82432], title: "柴油機關車庫", nowImg: "0205.JPG", pastImg: "048.jpg", pastStory: "下午兩三點，礦工出坑，機關車庫前響起笑聲與呼喊，一掃早上坑外抽菸時的沉重。交還裝備、洗去煤灰後，有些人趕著踩上開往選洗煤場的礦車，雙腳分踏兩車之間，手扶車邊，省下步行到火車站的體力。雖屬違規，但一天勞動下來，體力早已透支，見車便搭。當礦車駛出坑口，黑暗盡頭透出一道白光，像是「看到明天的希望」。坑口站著迎接的身影，哼唱聲隨風傳出，笑聲與煤塵一同飄進午後陽光。" },
        { coords: [25.08127, 121.82580], title: "復興坑運輸隧道", nowImg: "0211.JPG", pastImg: "011.jpg", pastStory: "復興坑隧道是瑞三礦業運煤的通道，煤炭自斜坑出口，由柴油機關車拖行炭車，穿越狹長坑道、經猴硐礦業所與整煤橋，送往選洗煤場。隧道口旁立著一座土地公廟，礦工每天清晨六點多經過會合掌祈禱：「土地公伯啊，我要入坑了，把命交給你了……」黑暗中的坑道不見天日，誰也不能保證今天是否能平安回家。傍晚出坑後，再站回廟前致謝：「土地公伯啊，今天平安，謝謝你顧著。」這裡是進入黑暗的起點，也是每日命運的交接站，一如礦場生活中，無聲卻堅定的信仰與生存儀式。" },
        { coords: [25.08100, 121.82442], title: "本坑吊橋", nowImg: "0207.JPG", pastImg: "007.jpg", pastStory: "吊橋曾是煤運的通道，也是家人等待的地方。從日治時期到民國七十年代，礦工從這裡走過，孩子在這裡玩，大人在橋上散步看河景。過去，橋面鋪木板、鋼索固定，一端連到猴硐本鑛坑口，一端接向對岸。小孩搖橋試膽，大人走橋回家，有人仍未歸來。現在鋼索已斷，只剩橋墩留在河床的巨石上。但這條橋還留在人們記憶裡。" },
        { coords: [25.0806, 121.8242], title: "瑞三本礦坑口", nowImg: "0209.JPG", pastImg: "003.jpg", pastStory: "民國58年7月7日早上9點半，瑞三本礦第二斜坑突發粉塵爆炸，為侯硐最嚴重的礦災。災後家屬聚集坑口，盼著一絲希望。爆炸造成坑內燃燒、坍塌，一氧化碳瀰漫。初期救援完全仰賴礦工自組隊伍入坑，在高溫與毒氣中，只靠帽燈微光摸索。隊伍反覆進出七八次，在倒塌與濃煙間搜尋；多名救援者中毒倒下，靠經驗與意志力撐持。生還者形容坑道內「那裡是地獄」。坑外迅速設立臨時指揮中心，準備鹽水、藥箱應對中毒與脫水。醫療人員、軍警與礦工合力維持秩序與協助轉送，搜救行動持續至深夜十點。" },
        { coords: [25.0791, 121.82598], title: "復興坑礦口", nowImg: "0212.JPG", pastImg: "009.jpg", pastStory: "民國79年瑞三礦業停止作業，復興坑口被磚塊封住，只留下一個小孔。這孔除了排氣，也被說是留給迷路的礦工靈魂出路。礦場關閉後，猴硐重歸寧靜，整煤場停擺、礦車不再穿行，只有這口小孔提醒著人們——有些靈魂，至今仍在坑裡徘徊。每年中元節前後，聚落準備祭品、設壇張羅，進入一種介於人間與陰界的節奏，只為讓那些未歸的人，有機會走出來" },
        { coords: [25.08853, 121.82915], title: "介壽橋頭工寮", nowImg: "0332.jpg", pastImg: "004.jpg", pastStory: "下午準備晚飯時，工寮裡六口爐灶輪著用，婦女們排隊煮飯，鍋煙瀰漫，空氣中混著柴火味與焦慮。一邊翻動鍋裡的菜，又頻頻望向窗外——等著家人出坑，最怕的是有人突然跑來，一開口就是出事的消息。礦工手上握著「卡嚕仔」，上頭記著每天工資，雖未領薪，卻能憑卡在福利社記帳買菜、借錢、吃飯。工作風險高，活在當下，吃下去的才算賺到，花出去的才是自己的。下工後，大家常聚在福利餐廳吃飯、喝酒、請客，慶生與尾牙也都在這裡舉辦。再往前走，是瑞三介壽堂。它原為公司開會的正式場所，後來也辦舞蹈研習班、慶生會、歌唱比賽，還兼作電影院，播放《八百壯士》《梁山伯與祝英台》等電影。曾是礦工們重要的娛樂空間，也承載著整個聚落的生活記憶。" },
        { coords: [25.08327, 121.82594], title: "美援厝", nowImg: "0214.JPG", pastImg: "045.jpg", pastStory: "中元普渡是礦場一年最重要的儀式。瑞三公司選定美援厝舉行公普，礦車載供、坑木搭桌，以「排」為單位祭拜——礦業所、整煤場、本鐵、復興坑及各領班分別設案，並請道士作法、跳鍾馗，引渡礦場亡魂。這裡普渡的不只是死者，也是活人的焦慮。像七七災變那年，三十七名礦工殞命，讓信仰成為唯一安撫的方式。普渡讓礦工安心再入坑也讓家屬相信——那些走失的靈魂，還有人記得、有人等。" }
      ];

      map = L.map('map').setView([25.0828, 121.8272], 17);
      L.tileLayer('https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}', {
        attribution: 'Tiles © Esri'
      }).addTo(map);

      locations.forEach(function(loc) {
        var container = L.DomUtil.create('div', 'info-panel');
        container.innerHTML = `
          <strong>${loc.title}</strong><br>
          <img id="img-${loc.title}" src="${loc.nowImg}" width="250" oncontextmenu="return false" draggable="false" style="pointer-events: none;"><br>
          <button class="photo-toggle" id="past-btn-${loc.title}" onclick="togglePhoto('${loc.title}', 'now')">現在</button>
          <button class="photo-toggle" id="past-btn-${loc.title}-past" onclick="togglePhoto('${loc.title}', 'past')">過去</button>
          <div id="story-${loc.title}" style="display:none; margin-top:5px;"></div>
        `;
        var marker = L.marker(loc.coords).addTo(map).bindPopup(container);
        markerRefs[loc.title] = marker;
      });

      const paths = [
        [locations[4].coords, locations[6].coords],
        [locations[3].coords, locations[6].coords]
      ];

      const afternoonPath = [
        locations[3].coords,
        locations[2].coords,
        locations[0].coords,
        locations[5].coords
      ];

      const morningPath = [
        locations[1].coords,
        locations[4].coords
      ];

      const afternoonLine = L.polyline(afternoonPath, {
        color: 'black',
        weight: 6,
        opacity: 1,
        className: 'glow-line-solid'
      }).addTo(map);

      afternoonLine.on('mouseover', function (e) {
        const el = afternoonLine.getElement();
        if (el) el.classList.add('hover-effect');
        const tooltip = L.tooltip({ permanent: false, direction: 'top' })
          .setLatLng(e.latlng)
          .setContent("午後下班路")
          .addTo(map);
        afternoonLine._tooltip = tooltip;
      });

      afternoonLine.on('mouseout', function () {
        const el = afternoonLine.getElement();
        if (el) el.classList.remove('hover-effect');
        if (afternoonLine._tooltip) {
          map.removeLayer(afternoonLine._tooltip);
          afternoonLine._tooltip = null;
        }
      });

      const morningLine = L.polyline(morningPath, {
        color: 'red',
        weight: 6,
        opacity: 1,
        className: 'glow-line-solid'
      }).addTo(map);

      morningLine.on('mouseover', function (e) {
        const el = morningLine.getElement();
        if (el) el.classList.add('hover-effect');
        const tooltip = L.tooltip({ permanent: false, direction: 'top' })
          .setLatLng(e.latlng)
          .setContent("早晨寄命路")
          .addTo(map);
        morningLine._tooltip = tooltip;
      });

      morningLine.on('mouseout', function () {
        const el = morningLine.getElement();
        if (el) el.classList.remove('hover-effect');
        if (morningLine._tooltip) {
          map.removeLayer(morningLine._tooltip);
          morningLine._tooltip = null;
        }
      });

      paths.forEach(function(path) {
        const polyline = L.polyline(path, {
          color: 'green',
          weight: 6,
          dashArray: '5, 10',
          opacity: 1,
          className: 'glow-line'
        }).addTo(map);

        polyline.on('mouseover', function (e) {
          const el = polyline.getElement();
          if (el) el.classList.add('hover-effect');
          const tooltip = L.tooltip({ permanent: false, direction: 'top' })
            .setLatLng(e.latlng)
            .setContent("迷失靈魂之路")
            .addTo(map);
          polyline._tooltip = tooltip;
        });

        polyline.on('mouseout', function () {
          const el = polyline.getElement();
          if (el) el.classList.remove('hover-effect');
          if (polyline._tooltip) {
            map.removeLayer(polyline._tooltip);
            polyline._tooltip = null;
          }
        });
      });
    });
  </script>
</body>
</html>
