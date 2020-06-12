# VisualEffectGraphSimpleTest2
[![Image from Gyazo](https://i.gyazo.com/9d934be77647fca66771b7e3d7633f99.gif)](https://gyazo.com/9d934be77647fca66771b7e3d7633f99)  
[Visual Effect Graph 入門](https://qiita.com/tan-y/items/cd6fc58674d6f0c54d0b)  
これに乗ってる内容を頭から作ってみた。  
いくつかUnityのバージョン違いが記事にあって困った。

# 記事との相違
## Bloom
### VFXカラーの設定
[![Image from Gyazo](https://i.gyazo.com/530182a3a378900872bfec8c0d9565cb.png)](https://gyazo.com/530182a3a378900872bfec8c0d9565cb)
Visual Effect GraphのOutputパートのカラー設定でIntensityを5とか数値を設定する。これだけで光る


### シーンの設定
シーン設定もすると光方に空気感が追加される感じ  
[![Image from Gyazo](https://i.gyazo.com/e36826d10b0c815905a276c84d9a0dcc.png)](https://gyazo.com/e36826d10b0c815905a276c84d9a0dcc)  
- シーンに空のGameObjectを作成
    - 名前は例えば"ForVolume"とかつける
- ForVolumeの"Add Component"を押してVolumeを追加
    - Profileボタンを押す。HDRPDefaultResourcesの中の"Sky and Fog Settings Profile"が表示されるので、とりあえずそれを選んでおく
    - Add Overrideボタンを押して"Bloomを追加"。BloomのIntensityにチェックを入れて、0.5とか適当な数値を設定  

[![Image from Gyazo](https://i.gyazo.com/63067feb2862de4322b41977b3f51766.png)](https://gyazo.com/63067feb2862de4322b41977b3f51766)

# 参考
[Visual Effect Graph 入門](https://qiita.com/tan-y/items/cd6fc58674d6f0c54d0b)  
大筋この内容。  
  
[UnityでのScene Settingの作成の仕方](https://teratail.com/questions/233619)  
Bloomの設定はSceneSettingが無くなって、Volumeでやるようになったようだ。  

# ライセンス
[MIT license](https://en.wikipedia.org/wiki/MIT_License).  
まぁ、ライセンスとか言い出すようなもんか？  
ってレベルの簡単サンプルだけどw  
一応、書いときます。
