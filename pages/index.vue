<template>
  <div id="spotlight">
    <div id="center">
      <div id="logo">
        <h1 id="title">Klavier Page</h1>
        <div id="social">
          <a href="https://twitter.com/miraxial" target="_blank" rel="noopener me" title="Twitter"><svg xmlns="http://www.w3.org/2000/svg" id="twitter" style="margin-bottom: .5rem;" width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"><path d="M23 3a10.9 10.9 0 0 1-3.14 1.53 4.48 4.48 0 0 0-7.86 3v1A10.66 10.66 0 0 1 3 4s-4 9 5 13a11.64 11.64 0 0 1-7 2c9 5 20 0 20-11.5a4.5 4.5 0 0 0-.08-.83A7.72 7.72 0 0 0 23 3z"></path></svg></a>
          <a href="https://atcoder.jp/users/miraxial" target="_blank" rel="noopener me"><img src="/atcoder.svg" width="66" height="56" title="atcoder" alt="atcoder" /></a>
          <a href="https://x.com/miraxial/status/1891058534722240902" target="_blank" rel="noopener me"><img src="/mahjong.jpg" width="56" height="56" title="mahjong" alt="mahjong" /></a>
          <a href="https://x.com/miraxial/status/1115020695778390016" target="_blank" rel="noopener me"><img src="/googleplay.png" width="56" height="56" title="googleplay" alt="googleplay" /></a>     
        </div>
      </div>
      <div id="wrapper">
        <div id="namecard">
          <div id="namecard-img">
            <nuxt-img src="/me.jpg" id="me-img" alt="me" width="89" height="89" />
          </div>
          <div>
            <p id="namecard-txt">システム管理ほか何でもどうぞ<br><a href="https://portfolio.klavier.page/">ポートフォリオ</a>・ご依頼はDMまで</p>
          </div>
        </div>
      </div>
    </div>
    <footer>
      <p>© {{ new Date().getFullYear() }}  Klavier Page</p>
    </footer>
  </div>
</template>

<style>
html {
  background: #494F5C;
  letter-spacing: .06em;
  line-height: 1.6;
}

body {
  color: #E8EEF2;
  font-family: trebuchet ms,Verdana,verdana ref,segoe ui,Candara,lucida grande,lucida sans unicode,lucida sans,Tahoma,sans-serif;
  margin: 0;
}

a {
  color: #E8EEF2;
}

#spotlight {
  align-items: center;
  display: flex;
  flex-direction: column;
  font-size: 1.5rem;
  justify-content: center;
  margin: auto;
  max-width: 93%;
  min-height: 100vh;
}

#center {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
  justify-content: center;
}

#logo {
  margin: 3rem 0;
}

#title {
  margin: 0;
  text-align: center;
}

#social {
  font-size: 3rem;
  margin-left: 1rem;
  opacity: .8;
  text-align: center;
}

#twitter {
  display: inline-block;
  height: 1em;
  vertical-align: -.125em;
  width: 1em;
}

#wrapper {
  position: relative;
  width: 100%;
}

#wrapper:before {
  content: '';
  display: block;
  padding-top: 75%; /* 高さを幅の75%に固定 */
}

#namecard {
  border: 1px solid #DDD;
  border-radius: 5px;
  bottom: 0;
  box-shadow: 0 2px 5px #CCC;
  font-size: 1rem;
  left: 0;
  position: absolute;
  right: 0;
  top: 0;
}

#namecard-img {
  text-align: center;
}

#me-img {
  border-radius: 3rem;
  margin-top: .5rem;
}

#namecard-txt {
  margin: 1rem .5rem;
  text-align: center;
}

footer {
  font-size: .6em;
  line-height: normal;
  text-align: center;
}

</style>
