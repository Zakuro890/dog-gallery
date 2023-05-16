# dog-gallery
Reactを使用したチュートリアルです。
このコードは、Reactを使用して作成されたシンプルなウェブアプリケーションです。
<img =""
# コンポーネントの説明
Headerコンポーネント:<br>
ヘッダーセクションを表示するコンポーネントです。タイトル "Cute Dog Images" を表示します。

Imageコンポーネント:<br>
画像を表示するコンポーネントです。propsとして画像のURL（src）を受け取り、"cute dog!" の代替テキストとともに画像を表示します。

Loadingコンポーネント:<br>
ローディングメッセージを表示するコンポーネントです。"Loading..." のテキストを表示します。<br>

Galleryコンポーネント:<br>
画像のギャラリーを表示するコンポーネントです。propsとして画像のURLの配列（urls）を受け取り、ローディング中の場合はLoadingコンポーネントを表示します。urlsの各要素に対して、Imageコンポーネントを使用して画像を表示します。

Formコンポーネント:<br>
フォームを表示するコンポーネントです。ユーザーが犬の品種を選択し、「Reload」ボタンをクリックすることで画像を再読み込みします。フォームの送信時にはonFormSubmit関数が呼び出されます。<br>

Mainコンポーネント:<br>
メインコンテンツを表示するコンポーネントです。fetchImages関数を使用して初期画像（デフォルトは"shiba"）を取得し、Galleryコンポーネントに渡します。また、Formコンポーネントを含み、ユーザーがフォームを使用して画像を再読み込みできるようにします。<br>

Footerコンポーネント:<br>
フッターセクションを表示するコンポーネントです。Dog APIから犬の画像を取得していることを示すメッセージと、Dog APIへの寄付へのリンクを表示します。<br>

Appコンポーネント:<br>
アプリケーション全体を表示する親コンポーネントです。Header、Main、Footerコンポーネントを含みます。<br>

このコードは、Reactのコンポーネントを使用してヘッダー、メインセクション、フッターを構築し、フォームを通じてユーザーが画像を再読み込みできるシンプルなウェブアプリケーションを作成しています。<br>

fetchImages関数:<br>
この関数は、指定された犬の品種に基づいて犬の画像のURLを取得するために使用されます。fetchImages関数は非同期関数であり、指定された品種に応じてDog APIから画像のURLを取得します。<br>

Appコンポーネント:
このコンポーネントはアプリケーションのエントリーポイントであり、全体のレイアウトを定義します。Header、Main、Footerコンポーネントを含みます。<br>
# 機能の流れ
アプリケーションの機能の流れは次のとおりです：<br>

1.Headerコンポーネントはタイトルを表示します。<br>
2.Mainコンポーネントでは、FormコンポーネントとGalleryコンポーネントを含んでいます。初期状態では、"shiba" の画像が表示されます。<br>
3.ユーザーがFormコンポーネントのフォームを使用して犬の品種を選択し、「Reload」ボタンをクリックすると、reloadImages関数が呼び出され、新しい品種の画像が表示されます。<br>
4.Galleryコンポーネントは、取得した画像のURLを受け取り、それぞれのURLに対してImageコンポーネントを生成して表示します。<br>
5.Footerコンポーネントは、Dog APIから犬の画像を取得していることを示すメッセージと、Dog APIへの寄付へのリンクを表示します。<br>
このコードは、Reactを使用してシンプルな犬の画像ギャラリーアプリケーションを作成しています。ユーザーはフォームを使用して犬の品種を選択し、アプリケーションは選択された品種の画像を取得して表示します。<br>
