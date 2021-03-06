# 東北きりたん歌唱データベースのラベルデータ
東北きりたん歌唱データベース（きりたん歌唱DB）の最新ラベルデータを共有するためのリポジトリです．データベースの本体は[こちら](https://zunko.jp/kiridev/login.php)からダウンロードできます．midi_label，mono_labelに加えてMusicXMLも公開しました．

## 学会発表や論文投稿において文献の引用が必要な場合
以下の論文を引用してください．  
[1] I. Ogawa and M. Morise: Tohoku Kiritan singing database: A singing database for statistical parametric singing synthesis using Japanese pop songs, Acoustical Science and Technology, vol. 42, no. 3, pp. 140-145, May 2021.

## 本リポジトリで配布するデータとGitHubで公開する動機
本データベースのラベルにはmidi_labelとmono_labelとがあり，それぞれ譜面データと音素境界のデータとなります．MIDIについてはMelodyneで自動採譜した後に手動で調整したものを配布していますが，楽曲によっては採譜そのものが困難な場合や，キーが曖昧でずれてしまっている場合があります．これら以外にも，実際に利用してみて判明する問題もあると考えられることから，ご利用者の皆様の修正案をここで議論できればと思い，ラベルデータのみGitHubで管理することにしました．

ラベルデータは本リポジトリで修正できますが，歌唱ファイルを修正する前処理はここで処理できません．修正のアイディアをissueで投げて頂ければ，本readmeに反映するように致します．明確なミスの場合はすぐ差し換えますが，微妙な差についてはissue内で差し換え・掲載するべきか議論する形にさせてください．以下の例のように情報は逐次更新していき，修正にご協力頂いた皆様のお名前はできるだけクレジットさせて頂く予定です．なお，本データベースはあくまでも改正著作権法30条の4に定められた範囲での利用に限定されていますので，本リポジトリやそれ以外の場所においても範囲を逸脱した使途にならないようにお気をつけください．

## 現時点で判明しているラベルの問題点
- 08: 前半部分の採譜が極めて困難なため，MIDIそのものが存在しない

## その他データベースについて品質を上げるための工夫
- 08: 歌声そのものについて，推定されたF0がMIDIとずれているため学習前にF0をMIDIに寄せたほうが良い

## 修正履歴
- 2020/04/05: 06.labのミス（617行目の/sh/）を修正
- 2020/01/06: 44の276行目/m/が抜けていたので追加
- 2020/01/06: 39の143行目/u/が抜けていたので追加
- 2020/01/06: 38の217行目/i/が抜けていたので追加
- 2020/01/06: 20の326, 334行目/t/->/ts/
- 2020/01/06: 16の390行目/a/が抜けていたので追加
- 2020/01/06: 15の318行目/sh/->/s/
- 2019/11/25: 06の後半部分のMIDIラベルが無かったので追加
- 2019/11/22: MIDIラベルの13と14が逆だったので入れ替え

## ご協力頂いた皆様
@Auxilyrica 様，Hiroshiba 様，dhgrs 様，匿名希望様，ご協力ありがとうございます．
