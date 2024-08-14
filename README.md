# CPEZemi2024AITeam
2024年度のCPEゼミで作るAIで学習しながら走るクルマ
20240814　作成開始
 Pythonの環境を作る
  Miniforgeで専用のライブラリ環境を作成<https://qiita.com/ikutaro_hamada/items/c47e6e5dd2e0ea2ae517
   1. Miniforge Pronptを開く
   2. 環境を作成　>conda create --name hamasanzemi2024
   3. 環境を変更　>conda activate hamasanzemi2024
   4. ultralyticsライブラリをインストール >conda install ultralytics
   5. Pytorchライブラリをインストール　>conda install torch torchvision torchaudio
  hamatsutozemi2024 のPython環境にVSCodeの右下で変更
  YOLOを導入すべく、下を参考にしたが、import時にエラー発生
  https://qiita.com/Mikeinu/items/530bdb2ddeeedc32eb58
  OSError: [WinError 126] 指定されたモジュールが見つかりません。 Error loading "C:\Users\TSUTOMU\miniforge3\envs\hamasanzemi2024\Lib\site-packages\torch\lib\fbgemm.dll" or one of its dependencies. が解決せず。
  ☆結局実施したこと
  ① VisualC++のvc_redist.x64.exeをインストール
   　https://circleken.net/2020/11/post34/
  ② C:\Users\TSUTOMU>conda install torch==2.2.0 torchvision==0.17.0 torchaudio==2.2.0　バージョンを指定した
   　　https://qiita.com/UKI_datascience/items/2626dba5bba8f51fcb85
  ③ 'base'環境でしかNoErrorにならない。多分①がbaseでしか対応しないからではないか
　結局Miniforgeの個別環境ではできなかった。macbookも同じ。ただしmacbookは①②は不要
次はhttps://qiita.com/daifuku10/items/50cb5cd9740e07fde591　で動画で犬をトラッキングできるようにしたい

   
