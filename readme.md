## Exhausting A Daijiro



git clone
xcode-select --install


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


``
npm install -g tsd
npm install 
tsd reinstall
npm start
```
Chromeとか開いて、 localhost:5000をアドレスに入れて検索する



### 新しい場所の入れ方
Add new location name to index.js (line 61)
Add new location metadata to typescript/frontend.ts (line 9).
Add new location to public/index.html in the public_sites variable.
Create a new logo for the top right corner called logo-site.png where site is the name.
Add credits to public/index.html.
Run tsc --outDir public/compiled/ typescript/* to update TypeScript definitions.