# Exhausting A Daijiro
###  MZNLAB


まず、ターミナルを使えるようにしよう！
Other > Terminal で開いて、コピペする 
```
xcode-select --install
```
次に、これダウンロードしよう！（ターミナルで）
```
git clone https://github.com/kkshmz/ExhaustingADaijiro
```
Homebrewっていうものを入れます。
Other > Terminal で開いて、コピペする 
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```
ブワーーーーーーってなるので、ちょっとお茶でもしましょう。
終わったら、以下のを叩こう！

```
brew install node
```
ここで、またバーってなる感じ、お茶美味しいですね。
またコピペ。
```
npm --version
```
ここで、v.x.x.みたいになると思います。
そうであれば、成功。

次に、ディレクトリーに移動します。

```
cd ExhaustingADaijiro
```
で以下をコピペしていく


```
npm install -g tsd
npm install 
tsd reinstall
npm start
```
Chromeとか開いて、 localhost:5000をアドレスに入れて検索する

サーバーにおきたかったら、聞いてね。


### 新しい場所の入れ方
Add new location name to index.js (line 61)

```
var sites = ['london', 'netherlands', 'birmingham', 'gwangju'];
```
に自分の入れたい場所を入れる。


Add new location metadata to typescript/frontend.ts (line 9).
→型式は以下

```
london: {
        id: 0,
        playlist: 'PLscUku2aaZnFE-7wKovrbi76b26VKxIT-',
        videoDurations: [7650, 4941, 7424, 7264, 6835, 7128],
        startTime: "April 15, 2015 15:00:00",
        modulusHours: 12
    },
```


Add new location to public/index.html in the public_sites variable.

これね。

```
var public_sites = [
        { id: 'london', text: 'london' },
        { id: 'netherlands', text: 'netherlands' },
        { id: 'birmingham', text: 'birmingham, uk' }
        // { id: 'gwangju', text: 'gwangju' }
    ];
```

Create a new logo for the top right corner called logo-site.png where site is the name.

ロゴ入れたかったら。
→logo-site.pngっていう名前で。
/publicとかに入れとこう。



Add credits to public/index.html

クレジット系を記入。型は以下。

```
<h1>EXHAUSTING A CROWD</h1>
        <p>BIRMINGHAM, UK</p>
        <div class="credits-divider"><span></span>2O17<span></span></div>
        <p><span class="for">by</span> <a href="http://kylemcdonald.net/">KYLE MCDONALD</a></p>
        <p><span class="for">with</span> <a href="http://halfdanj.dk/">JONAS JONGEJAN</a> / COLLABORATION &amp; SITE DEVELOPMENT</p>
        <p>COMMISSIONED <span class="for">by</span> <a href="http://www.bom.org.uk/">BIRMINGHAM OPEN MEDIA</a></p>
        <p>FIRST COMMISSIONED <span class="for">by</span> <a href="http://www.vam.ac.uk/">VICTORIA AND ALBERT MUSEUM</a> <span class="for">for</span> <a href="http://www.vam.ac.uk/content/exhibitions/all-of-this-belongs-to-you/">ALL OF THIS BELONGS TO YOU</a></p>
        <p><a href="https://twitter.com/carlscottdavies">CARL DAVIES</a> <span class="for">/</span> VIDEO</p>
        <p>SPECIAL THANKS <span class="for">to</span> LOUISE LATTER</p>
        <div class="credits-divider"><span></span>on location at<span></span></div>
        <p>VICTORIA SQUARE, BIRMINGHAM <span class="for">on</span> AUGUST 21</p>
```

Run `tsc --outDir public/compiled/ typescript/* `to update TypeScript definitions.

→`tsc --outDir public/compiled/ typescript/* `を入れて、アップデートって感じ。

