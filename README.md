■サービス概要
・小説とともに、youtube上のテーマソングなどを一緒に指定できる小説投稿サイトです。音楽を流しながら、小説を読むという新しいサービスを展開します。
・基本的な機能の検索機能、タグ機能、点数評価機能、また投稿大賞を決める大会期間中はユーザー交流を盛んにするためにSNS機能がつきます。
・感想についてはテキストでの感想文はもちろん「エモーショナルボタン」という悲しい、うれしい。たのしい、わらったなどのボタンを実装しようと思います。点数機能はなくてもいいかもしれません。
また、荒らし対策をしやすくなる管理画面などを作成しモデレーター等による管理を推進します。
・AIによる校閲機能（誤字脱字指摘）を実装したい。可能ならば（サービスを調べていくと自宅にサーバーを置いてローカルLLMを置く必要がある）

■ このサービスへの思い・作りたい理由
以前とある小説投稿サイト（https://coolier.net/　）に類似するサイトを作者として利用していたが検索機能が使えない、作成より２０年ほど経っており仕様が古くSNS連携機能やスマホでの閲覧機能が不便であること、ブックマーク機能などがないことなどあり不便さを感じていました。
その投稿していたサイトは２０２０年に閉鎖してしまったため、非常に寂しい思いをしたことを覚えています。当時の仲間の方の再開を望む声に答えるべく、また未だにSNSでは再開を望む声が多いので、その声に答えたいと思っています。できれば初心者と古くからいる人々の交流機能を持たせたいと思っています。
また創作ジャンルごとに使用されることを前提としており、様々なジャンルでその内部の人々の交流が盛んになればと思います。
最大手のpixivでは投稿大賞を決める大会はありますが、ユーザー間の交流機能はありません。以前にそういった大会を開催したところ非常に盛り上がりユーザーと作者が盛り上がっていたことを思い出しました。そのような機能を実装することができれば、仲間を作る楽しみを感じることができるかもしれません。

■ ユーザー層について
18-25歳と30歳からを想定してます。
18-25歳は読書家でアニメなどが好きな人が二次創作を見る場所として。現在はあにまんというサイトが短い小説とユーザー交流が同時にできるサイトの受け口として働いていますが、そこでは長い小説を読む機能がありません。
30歳からは、以前投稿していたが投稿をやめた人のリバイバルを目指すものです。
決めたユーザー層についてどうしてその層を対象にしたのかそれぞれ理由を教えてください。
　https://togetter.com/li/2233981　こちらは年に一度行われる人気投票ですがジャンル的には長命にも関わらず若年層が現在多数派になっています。故に長く続くプラットフォームが求められております。
また古くからのファンは熱心なクリエイターが多く、その３０代前後の年代の方の作品を若年層が読むというような構造になっています。

■サービスの利用イメージ
ユーザーがこのサービスをどのように利用できて、それによってどんな価値を得られるかを簡単に説明してください。
読者：レスポンシブデザインがあるためスマホからアクセスしやすい。主に想定している若年層はPCよりも寝る前にスマホなどで読んでいる。
作者：ブックマークやタグなどで傾向をつかめる。またサービスによって、作者や読者の間の交流が図れる。コミュニティの基盤として機能しているのは現在Twitterのみとなっているので様々な形で交流の場を設けたいと思いました。
■ ユーザーの獲得について
想定したユーザー層に対してそれぞれどのようにサービスを届けるのか現状考えていることがあれば教えてください。
https://touhougarakuta.com/news/201012/ ここで告知していただいたこともあるので、ここでおしらせをする。またツイッター上で作成途中などの情報を広めていく。
■ サービスの差別化ポイント・推しポイント
似たようなサービスが存在する場合、そのサービスとの明確な差別化ポイントとその差別化ポイントのどこが優れているのか教えてください。独自性の強いサービスの場合、このサービスの推しとなるポイントを教えてください。
Pixivなどがおそらく似た機能をもっていますがpixivでは作品についての交流機能がないのでそこを実装したい。あくまで作品ごとにSNSのような何かがつくイメージです。
・音楽は埋め込み機能で行います。
■ 機能候補
現状作ろうと思っている機能、案段階の機能をしっかりと固まっていなくても構わないのでMVPリリース時に作っていたいもの、本リリースまでに作っていたいものをそれぞれ分けて教えてください。
MVPリリース
１マルチ検索・オートコンプリート
２ブックマーク機能
３レコメンド機能
４音楽埋込機能
５SNS機能
６レスポンシブデザイン
７フェステイバルモード（イベントとしてコンペティションを開催する機能、普段の投稿画面とは別にするUIやデザインなども異なり、常にSNSがある）
本リリース
６誤字脱字修正Ai（可能ならば）

■ 機能の実装方針予定
一般的なCRUD以外の実装予定の機能についてそれぞれどのようなイメージ(使用するAPIや)で実装する予定なのか現状考えているもので良いので教えて下さい
１マルチ検索・オートコンプリート
JQuery
３音楽埋込機能
https://support.infocms.jp/faq/detail.html?pdid=275
4SNS機能
ActionCable（Rails標準）
６誤字脱字修正Ai
DeepSeek-R1-Distill-Qwen-14B/32B-Japanese
https://gihyo.jp/article/2025/01/deepseek-r1-japanese 
７メール（パスワード忘れなど）
Action Mailer 

