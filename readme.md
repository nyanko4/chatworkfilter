<a href="https://render.com/deploy?repo=https://github.com/nyanko4/chatworkfilter.git">
<img src="https://render.com/images/deploy-to-render-button.svg" alt="Deploy to Render">
</a><br>
上のボタンを押しBlueprint Nameに適当に入れ、Deploy Blueprintを押す。<br>
Create web service chatworkfilterと書かれている部分のchatworkfilterを押す。<br>
押した後、https://chatworkfilter・・・と続く部分をコピーし<a href="https://www.chatwork.com">Chatwork</a>に移動しする。<br>
botにしたいaccountのaccountIdをコピーしておく。(自分のコメントを引用し、aid=に続く数字をコピーすると良い)<br>
画面右上にある自分のアイコン、名前が書かれている部分をタップ、サービス連携を押し、<a href="https://www.chatwork.com/service/packages/chatwork/subpackages/api/token.php">APIトークン</a>をコピーする。次に<a href="https://www.chatwork.com/service/packages/chatwork/subpackages/webhook/list.php">webhook</a>と書かれている部分を押す。<br>
新規作成を押し、webhook名は適当に入れ、先程コピーしたURLを入れその後に/getchatと入れる。<br>
イベントと書かれている部分はルームイベントの方を選択しメッセージ作成、メッセージ更新の両方にチェックを入れる。<br>
ルームID:と書かれている部分にfilterを入れたい部屋のルームIDを入れ、作成を押す。<br>
作成を押した後下の方にトークンと書かれた部分があるのでそれをコピーする。<br>
renderの方に戻り、Environmentを押すEditを押し、accountIdに先程コピーしたaccountIdを入れ、CWapitokenの方に<a href="https://www.chatwork.com/service/packages/chatwork/subpackages/api/token.php">APIトークン</a>を入れる。またwebhookTokenの方にトークンを入れる。<br>
Save, rebuild, and deployを押し、少し待てばbot化します。
