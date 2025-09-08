---
permalink: /
title: "Kanta Ogawa"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---
<style>
/* Elegant Deep Blue Theme for cv.md */
html, body {
  background-color: #edf1f5; /* 淡く上品な青みがかったグレー */
  color: #1a1a2e;
  font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
  margin: 0;
  padding: 0;
  min-height: 100vh;
}

/* Headings */
h1, h2, h3, h4, h5 {
  color: #1c2c4c; /* 渋めの深いネイビーブルー */
}

/* Links */
a {
  color: #305c8e; /* 落ち着いたブルー */
  text-decoration: none;
  border-bottom: 1px dotted #305c8e;
  transition: color 0.3s ease, border-bottom 0.3s ease;
}

a:hover {
  color: #102944; /* 濃いめの青で強調 */
  border-bottom: 1px solid #102944;
}

/* Section box */
section {
  background-color: #ffffff;
  padding: 2rem;
  border-left: 5px solid #3a5276; /* 深みのある青グレー */
  box-shadow: 0 4px 10px rgba(26, 38, 58, 0.08);
  border-radius: 10px;
  margin: 2rem auto;
  transition: box-shadow 0.3s ease;
  max-width: 1000px;
  box-sizing: border-box;
}

section:hover {
  box-shadow: 0 6px 14px rgba(26, 38, 58, 0.15);
}

/* Lists */
ul {
  list-style-type: disc;
  padding-left: 1.5em;
}
</style>

<p>
  Hi, I'm Kanta Ogawa. I am currently a Ph.D. student at the Department of Economics at New York University.
</p>

<p>
  <strong>Email:</strong>
  <a id="email-link" href="#"></a>
</p>

<script>
  // メールアドレスを分割して定義
  var user = "ko2406";
  var domain = "nyu.edu";

  // メールアドレスを結合して、aタグのhrefとテキストに設定
  var emailAddress = user + "@" + domain;
  var emailLink = document.getElementById("email-link");

  emailLink.href = "mailto:" + emailAddress; // クリックしたらメーラーが起動するようにする
  emailLink.textContent = emailAddress;       // 見た目のテキストも設定する
</script>
