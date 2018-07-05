# term3-CarND-Semantic-Segmentation

Microsoft Visual C++ 2015 Redistributable Update 3
https://www.microsoft.com/ja-JP/download/details.aspx?id=53587

conda update conda

python -m pip install --upgrade pip

pip install --ignore-installed --upgrade tensorflow 

conda create --name=IntroToTensorFlow python=3 anaconda

source activate IntroToTensorFlow

conda install -c conda-forge tensorflow
********************
conda env list

conda info -e コマンドで現存する環境を確認

conda env remove -n carnd-termXXX

conda install python=3.5  #downgrade

不要になったパッケージやキャッシュを削除
　不要な環境の削除ができたら、今度はパッケージやキャッシュを削除しましょう。 conda clean コマンドを利用すると、使われていないパッケージやキャッシュを削除することができます。 一番簡単には –all オプションを指定して、削除できるものは全て削除するのが良いかも知れません。

$ conda clean --all


TensorFlowのインストール
　前述の通り、TensorFlowのインストールはconda installではなくpip installが公式に推奨されている。これに従い、pip installコマンドを用いる。CPU版とGPU版でパッケージ名が異なるため、おのおのの環境に合わせて必要なパッケージをインストールする。GPU版は事前設定が必要であることは前述の通りだ。

Bash
(introtensorflow) $ pip --no-cache-dir install -I -U tensorflow

リスト10　TensorFlowをインストールするコマンド（CPU版）

Bash
(introtensorflow) $ pip --no-cache-dir install -I -U tensorflow-gpu
    
    リスト11　TensorFlowをインストールするコマンド（GPU版）
    
##############################################################################    
conda create --name=IntroToTensorFlow python=3.4 anaconda
