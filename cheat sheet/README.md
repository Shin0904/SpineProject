#UnityでSpineアニメーションを動かしちゃおう！



##Spineアニメーション初期設定

###UnityでSpineアニメーションを動かすための準備
UnityでSpineを使う際にはランタイムが必要なので、下記のアドレスからZipファイルをダウンロードする。

https://github.com/EsotericSoftware/spine-runtimes

###Spineランタイムの設定
「spine-runtimes-master」内にある「spine-csharp」と「spine-unity」がSpineを使うのに必要なランタイムです。

「Assets」に「spine-csharp」のフォルダを作成し、「spine-csharp/src」の中身を「Assets/spine-csharp」にD&Dする。
![spine-csharp](spine-csharp.png)「spine-unity/Assets/spine-unity」のフォルダを「Assets」にD&Dする。
![spine-unity](spine-unity.png)

###Spine表示までの設定
「Assets」に「Examples/Spine/Dragon」のフォルダを作成し、
「spine-unity/Assets/Examples/Spine/Dragon」のフォルダにある
「dragon.atlas.txt」「dragon.json」「dragon.png」「dragon2.png」のファイルを
「Assets/Examples/Spine/Dragon」にD&Dする。
![spine-dragon](spine-dragon.png)
D&Dが完了すると、「dragon_Atlas」「dragon_dragon」「dragon_dragon2「dragon_SkeletonData」の４つが作成される。

![dragon](dragon.png)

###Hierarchy内にSpineSkeletonAnimationを作成
Hierarchy内の「Create」「Create Other」「Spine SkeletonAnimation」を選択する。

![SpineSkeletonAnimation](SpineSkeletonAnimation.png)

「Skeleton Animation」の「Skeleton Data Asset」に「dragon_SkeletonData」をD&Dする。

![SkeletonData](SkeletonData.png)

「Animation」を「flying」に設定する。
「Loop」にチェックを入れるとアニメーションがループ再生される。

![Animation](Animation.png)

最後にSceneのセーブ場所として、「Examples/Scenes」に「Dragon」のファイル名でセーブする。

![SaveScenes](SaveScenes.png)

Unityの実行ボタンを押すと、アニメーションが再生されます。

![Run](Run.png)

以上が簡単なSpineアニメーションの設定です。


