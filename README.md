MapEnv
====

GarminGPS向け日本地図の作成に必要なツール類が"git clone"するだけで揃います。

## Description

これはmkgmapを使ってOpenStreetMapからオリジナル地図を作成するためのツール/スクリプト/設定ファイルのパッケージです。基本的に必要となるツール類が含まれており、このプロジェクトをダウンロードしていくつかのシェルスクリプトを実行するだけでGPSで利用可能な地図が作成出来ます。
（ただし、2017/09/11現時点では作成範囲を日本に限定しています）

本パッケージは以下の環境で動作確認しています。

 - OS:Ubuntu 16.04
 - Memory:8GByte（4GByte以上は欲しいです）
 - HDD:100GByte

本パッケージで地図を生成するにあたり、大容量のデータを扱うことになるためメモリとHDDは大きいほど良いです。特に基盤地図情報のデジタル標高モデルを使用して等高線を引く場合は、さらにHDD容量が必要となります。


## Requirement

本パッケージは以下のツール/モジュールを必要とします。

- Java8(OpenJDK)
- python2.7
- perl
- gdal 2.2以降
- python module(numpy, gdal, matplotlib, beautifulsoup, lxml)
- kakasi
- wget
- sed
- Bash


## Usage

T.D.B


## Install

1.必要なパッケージ類をインストールします(ubuntuの場合)。

> $ sudo apt-get install osmosis osmium-tool gdal-bin python python-pip python-numpy python-gdal python-matplotlib python-beautifulsoup python-lxml kakasi kakasi-dic

2.本パッケージをgit cloneします。

> $ git clone --recursive https://github.com/suke-blog/MapEnv.git



## LICENCE

* fgddemImporter - GPL3 (https://github.com/minorua/fgddemImporter)
* mkgmap - GPL2 (http://www.mkgmap.org.uk/)
* splitter - GPL3 (http://www.mkgmap.org.uk/)
* ogr2osm - MIT license (https://github.com/pnorman/ogr2osm)
* phyghtmap - GPL2 (http://katze.tfiu.de/projects/phyghtmap/)
* SKK-JISYO.station, SKK-JISHO.geo - GPL2 (http://openlab.ring.gr.jp/skk/wiki/wiki.cgi?page=SKK%BC%AD%BD%F1)

