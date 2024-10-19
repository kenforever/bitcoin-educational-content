---
name: BIP39 パスフレーズ
description: パスフレーズの仕組みを理解する
---
![cover](assets/cover.webp)

## BIP39 パスフレーズとは何ですか？

HDウォレットは通常、12または24の単語からなるニーモニックフレーズから生成されます。このフレーズは非常に重要で、ハードウェアウォレットなどの物理的な媒体が失われた場合に、ウォレットのすべてのキーを復元することを可能にします。しかし、このフレーズが侵害されると、攻撃者がすべてのビットコインを盗む可能性があるため、単一の障害点を構成します。

![PASSPHRASE BIP39](assets/notext/01.webp)

ここでパスフレーズが登場します。これは、キー導出プロセスでニーモニックフレーズに追加される任意のパスワードで、自由に選択でき、ウォレットのセキュリティを強化します。

![PASSPHRASE BIP39](assets/notext/02.webp)

パスフレーズをハードウェアウォレットのPINコードや、コンピューター上のウォレットへのアクセスを解除するために使用されるパスワードと混同しないでください。これらの要素とは異なり、パスフレーズはウォレットのキーの導出において役割を果たします。**これは、パスフレーズなしではビットコインを回復することができないことを意味します。**

パスフレーズはニーモニックフレーズと連携して機能し、キーが生成されるシードを変更します。したがって、誰かがあなたの12または24語のフレーズを入手しても、パスフレーズがなければ資金にアクセスすることはできません。**パスフレーズを使用することは、異なるキーを持つ新しいウォレットを基本的に作成することを意味します。パスフレーズを（わずかに）変更すると、異なるウォレットが生成されます。**

## なぜパスフレーズを使用すべきですか？

パスフレーズは任意であり、ユーザーが選択した任意の文字の組み合わせであることができます。したがって、パスフレーズを使用することにはいくつかの利点があります。まず、ニーモニックフレーズの侵害に関連するすべてのリスクを、資金にアクセスするための第二の要素を要求することで減らします（盗難、自宅へのアクセスなど）。

次に、物理的な制約による資金の盗難、例えば悪名高い「*5ドルのレンチ攻撃*」に対処するために、デコイウォレットを戦略的に作成するために使用できます。このシナリオでは、パスフレーズを使用しないウォレットに少量のビットコインを含めることが考えられており、潜在的な攻撃者を満足させるのに十分な量ですが、隠されたウォレットを持っています。この後者は同じニーモニックフレーズを使用していますが、追加のパスフレーズで保護されています。

最後に、HDウォレットのシード生成のランダム性を制御したい場合に、パスフレーズを使用することが興味深いです。

## 良いパスフレーズを選ぶ方法は？
パスフレーズが効果的であるためには、十分に長くランダムでなければなりません。強力なパスワードと同様に、できるだけ長くランダムなパスフレーズを選択し、文字、数字、記号のバリエーションを使用して、どんなブルートフォース攻撃も不可能にすることをお勧めします。

このパスフレーズを適切に保存することも重要です。ニーモニックフレーズと同じ方法で。**これを失うと、ビットコインへのアクセスを失うことを意味します。**頭の中だけで覚えることは、損失のリスクを不合理に高めるため、強くお勧めしません。理想的なのは、ニーモニックフレーズとは別の物理的な媒体（紙や金属）に書き留めることです。このバックアップは、ニーモニックフレーズが保管されている場所とは異なる場所に明らかに保管する必要があります。これにより、両方が同時に侵害されることを防ぎます。

## チュートリアル

Ledgerデバイス（Stax、Flex、またはNano）にパスフレーズを設定する方法については、このチュートリアルを参照してください：

https://planb.network/tutorials/wallet/passphrase-ledger