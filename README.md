# lab_analysis

in vivoカルシウムイメージングデータを対象とした、
1細胞レベル神経活動解析の実装例をまとめたポートフォリオです。  
（研究守秘義務に基づき、許可されたコードおよび再構成した解析例のみ公開）

本リポジトリでは、実験データの前処理（動き補正）から  
細胞抽出（CaImAn）、刺激応答の時系列解析、統計評価、空間mappingまで、  
一連の解析パイプラインをPythonで一貫して実装しています。

## 主な特徴
・in vivo神経活動データの1細胞レベル解析  
・前処理〜抽出〜統計までの再現性を意識した解析設計  
・実験データ特性を踏まえた解析フローの統合実装  

## 内容
・caiman_analysis  
CaImAnを用いたカルシウムイメージング解析例  
（動き補正、細胞抽出、ΔF/F算出、時系列信号解析）

・odor_response_mapping  
匂い刺激応答におけるプルキンエ細胞の時空間応答マッピング  
（刺激依存的ROI応答の時系列解析＋空間heatmap）

<p align="center">
  <img src="odor_response_mapping/ROI_position_heatmap.png" width="600">
</p>

・cluster_visualization  
Open CVを用いた、小脳プルキンエ細胞活動のクラスタリング解析例  
（時空間解析とクラスター解析の統合）

## 使用技術
Python / CaImAn / NumPy / pandas / matplotlib  
1細胞神経活動データに対する前処理〜抽出〜統計解析までの一連の解析フローを実装
