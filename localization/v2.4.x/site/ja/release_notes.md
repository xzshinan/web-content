---
id: release_notes.md
summary: Milvusリリースノート
title: リリースノート
---
<h1 id="Release-Notes" class="common-anchor-header">リリースノート<button data-href="#Release-Notes" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h1><p>Milvusの新機能をご確認ください！このページでは、各リリースの新機能、改善点、既知の問題、バグ修正についてまとめています。v2.4.0以降の各バージョンのリリースノートはこのセクションにあります。定期的にこのページをご覧いただき、アップデート情報をご確認ください。</p>
<h2 id="v249" class="common-anchor-header">v2.4.9<button data-href="#v249" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日2024年8月20日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.9</td><td>2.4.5</td><td>2.4.3</td><td>2.4.4</td></tr>
</tbody>
</table>
<p>Milvus v2.4.9では、一部のコーナーケースで制限値(topk)未満の結果を返す可能性のある重大な問題に対処し、プラットフォームのパフォーマンスとユーザビリティを向上させるためのいくつかの重要な改善が含まれています。</p>
<h3 id="Critical-fixes" class="common-anchor-header">重大な修正</h3><ul>
<li>読み取り可能なスナップショットからl0セグメントを除外しました<a href="https://github.com/milvus-io/milvus/pull/35510">(#35510</a>)。</li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>プロキシにおけるスキーマヘルパーの重複作成を削除しました<a href="https://github.com/milvus-io/milvus/pull/35502">(#35502</a>)。</li>
<li>Ubuntu 20.04におけるMilvusのコンパイルをサポートしました<a href="https://github.com/milvus-io/milvus/pull/35457">(#35457</a>)。</li>
<li>ロックの使用を最適化し、クラスタリングバッファライタのダブルフラッシュを回避しました<a href="https://github.com/milvus-io/milvus/pull/35490">(#35490</a>)。</li>
<li>無効なログを削除しました<a href="https://github.com/milvus-io/milvus/pull/35473">(#35473</a>)。</li>
<li>クラスタリング圧縮のユーザーガイドを追加しました<a href="https://github.com/milvus-io/milvus/pull/35428">(#35428</a>)。</li>
<li>スキーマヘルパーに動的フィールドのサポートを追加しました<a href="https://github.com/milvus-io/milvus/pull/35469">(#35469</a>)。</li>
<li>生成されるYAMLにmsgchannelセクションを追加した<a href="https://github.com/milvus-io/milvus/pull/35466">(#35466</a>)。</li>
</ul>
<h2 id="v248" class="common-anchor-header">v2.4.8<button data-href="#v248" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日2024年8月14日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.8</td><td>2.4.5</td><td>2.4.3</td><td>2.4.4</td></tr>
</tbody>
</table>
<p>Milvus 2.4.8では、システムのパフォーマンスと安定性にいくつかの重要な改良が加えられました。最も注目すべき機能はクラスタリングコンパクションの実装であり、これは指定されたクラスタリングキーに基づいて大規模なコレクション内のデータを再分散し、スキャンされるデータ量を削減することにより、検索およびクエリの効率を向上させるメカニズムである。また、コンパクションはシャードDataNodeから切り離され、任意のDataNodeが独立してコンパクションを実行できるようになり、耐障害性、安定性、パフォーマンス、スケーラビリティが向上した。さらに、GoコンポーネントとC++コンポーネント間のインターフェイスは、非同期CGOコールを使用するようにリファクタリングされ、セッションのタイムアウトなどの問題に対処しました。アプリケーションの依存関係も更新され、既知のセキュリティ脆弱性に対処しました。さらに、このリリースには多数のパフォーマンスの最適化と重要なバグの修正も含まれています。</p>
<h3 id="Features" class="common-anchor-header">機能</h3><ul>
<li>クラスタリングコンパクションが実装され、指定されたクラスタリングキーに 基づいてデータを再分散できるようになり、クエリの効率が向上<a href="https://github.com/milvus-io/milvus/pull/34326">した (#34326</a>)、<a href="https://github.com/milvus-io/milvus/pull/34363">(#34363</a>)。</li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>CGOに非同期検索機能を実装。<a href="https://github.com/milvus-io/milvus/pull/34200">(#34200</a>)</li>
<li>コンパクション処理をShard DataNodeから分離し、システムのモジュール性を向上。<a href="https://github.com/milvus-io/milvus/pull/34157">(#34157</a>)</li>
<li>パフォーマンス向上のため、プロキシ/デリゲータ内のQueryNodeでクライアントプーリングのサポートを追加しました。<a href="https://github.com/milvus-io/milvus/pull/35195">(#35195</a>)</li>
<li>GinおよびRestfulV1ハンドラにおいて、JSONのマーシャリングおよびアンマーシャリング時のCPUオーバーヘッドを最小化するSonicを統合。<a href="https://github.com/milvus-io/milvus/pull/35018">(#35018</a>)</li>
<li>認証結果の取得を最適化するために、インメモリキャッシュを導入した。<a href="https://github.com/milvus-io/milvus/pull/35272">(#35272</a>)</li>
<li>autoindexのデフォルトのメトリックタイプを変更した。<a href="https://github.com/milvus-io/milvus/pull/34277">[#34277</a>,<a href="https://github.com/milvus-io/milvus/pull/34479">#34479</a>]</li>
<li>変数カラムの実行時のメモリフォーマットをリファクタリングし、メモリ使用量を削減しました。<a href="https://github.com/milvus-io/milvus/pull/34367">[#34367</a>,<a href="https://github.com/milvus-io/milvus/pull/35012">#35012</a>,<a href="https://github.com/milvus-io/milvus/pull/35041">#35041</a>]</li>
<li>コンパクション処理をリファクタリングし、永続的なデータ保存を可能にしました。<a href="https://github.com/milvus-io/milvus/pull/34268">(#34268</a>)</li>
<li>メモリマップドファイルが成長するセグメントをサポートし、メモリ管理を改善。<a href="https://github.com/milvus-io/milvus/pull/34110">(#34110</a>)</li>
<li>RESTful API のサポート、一貫性レベルのロギング、システムエラーとユーザーエラーの区別を追加し、アクセスログを改善しました。<a href="https://github.com/milvus-io/milvus/pull/34295">[#34295</a>,<a href="https://github.com/milvus-io/milvus/pull/34352">#34352</a>,<a href="https://github.com/milvus-io/milvus/pull/34396">#34396</a>]</li>
<li>Knowhereの新しいパラメータ<code translate="no">range_search_k</code> を利用して、範囲検索を高速化した。<a href="https://github.com/milvus-io/milvus/pull/34709">(#34709</a>)</li>
<li>ブロックブルームフィルタを適用し、フィルタの構築とクエリの速度を向上しました。<a href="https://github.com/milvus-io/milvus/pull/34377">[#34377</a>,<a href="https://github.com/milvus-io/milvus/pull/34922">#34922</a>]</li>
<li>メモリ使用量の改善：<ul>
<li>DataNodeのインサートバッファにあらかじめ領域を割り当てました。<a href="https://github.com/milvus-io/milvus/pull/34205">(#34205</a>)</li>
<li>Reduce処理用の<code translate="no">FieldData</code> 。<a href="https://github.com/milvus-io/milvus/pull/34254">(#34254</a>)</li>
<li>メモリリークを防ぐため、deleteコーデックのレコードを解放。<a href="https://github.com/milvus-io/milvus/pull/34506">(#34506</a>)</li>
<li>ファイル読み込み中のディスクファイルマネージャの同時実行レベルを制御。<a href="https://github.com/milvus-io/milvus/pull/35282">(#35282</a>)</li>
<li>Go実行時のガベージコレクションロジックを最適化し、タイムリーなメモリ解放を実現。<a href="https://github.com/milvus-io/milvus/pull/34950">(#34950</a>)</li>
<li>成長するセグメントに対する新しいシールポリシーを実装。<a href="https://github.com/milvus-io/milvus/pull/34779">(#34779</a>)</li>
</ul></li>
<li>DataCoord の強化：<ul>
<li>CPU 使用率を削減。<a href="https://github.com/milvus-io/milvus/pull/34231">[#34231</a>,<a href="https://github.com/milvus-io/milvus/pull/34309">#34309</a>]</li>
<li>ガベージコレクションの終了ロジックを高速化。<a href="https://github.com/milvus-io/milvus/pull/35051">(#35051</a>)</li>
<li>ワーカーノードのスケジューリングアルゴリズムを改善しました。<a href="https://github.com/milvus-io/milvus/pull/34382">(#34382</a>)</li>
<li>インポート操作に特化したセグメントサイズ制御アルゴリズムを強化。<a href="https://github.com/milvus-io/milvus/pull/35149">(#35149</a>)</li>
</ul></li>
<li>ロードバランシングアルゴリズムの改良：<ul>
<li>デリゲータのメモリ過負荷要因を低減しました。<a href="https://github.com/milvus-io/milvus/pull/35164">(#35164</a>)</li>
<li>デリゲータに固定メモリサイズを割り当て。<a href="https://github.com/milvus-io/milvus/pull/34600">(#34600</a>)</li>
<li>新しいクエリノードに対してセグメントとチャンネルを過剰に割り当てないようにした。<a href="https://github.com/milvus-io/milvus/pull/34245">(#34245</a>)</li>
<li>クエリコーディネータによるスケジューリングサイクルあたりのタスク数を削減し、スケジューリング頻度を増加させた。<a href="https://github.com/milvus-io/milvus/pull/34987">(#34987</a>)</li>
<li>データノードのチャネルバランシングアルゴリズムを強化しました<a href="https://github.com/milvus-io/milvus/pull/35033">(#35033</a>)。</li>
</ul></li>
<li>システムメトリクスの拡張：様々なコンポーネントにおいて、以下のような新しいメトリクスを追加しました：<ul>
<li>強制書き込み拒否状態。<a href="https://github.com/milvus-io/milvus/pull/34989">(#34989</a>)</li>
<li>キューの待ち時間。<a href="https://github.com/milvus-io/milvus/pull/34788">(#34788</a>)</li>
<li>ディスククォータ。<a href="https://github.com/milvus-io/milvus/pull/35306">(#35306</a>)</li>
<li>タスク実行時間。<a href="https://github.com/milvus-io/milvus/pull/35141">(#35141</a>)</li>
<li>ビンログサイズ。<a href="https://github.com/milvus-io/milvus/pull/35235">(#35235</a>)</li>
<li>挿入率。<a href="https://github.com/milvus-io/milvus/pull/35188">(#35188</a>)</li>
<li>メモリの高水位。<a href="https://github.com/milvus-io/milvus/pull/35188">(#35188</a>)</li>
<li>RESTful API のメトリクス。<a href="https://github.com/milvus-io/milvus/pull/35083">(#35083</a>)</li>
<li>検索待ち時間。<a href="https://github.com/milvus-io/milvus/pull/34783">(#34783</a>)</li>
</ul></li>
</ul>
<h3 id="Changes" class="common-anchor-header">変更点</h3><ul>
<li><p>オープンソースユーザーのために、このバージョンでは AutoIndex の<code translate="no">FloatVector</code> と<code translate="no">BinaryVector</code> のメトリックタイプをそれぞれ<code translate="no">Cosine</code> と<code translate="no">Hamming</code> に変更しました。</p></li>
<li><p><strong>サードパーティ依存バージョンの修正</strong>：</p>
<ul>
<li>このリリースでは、Milvusのソフトウェアサプライチェーンマネジメントを大幅に強化するため、特定のサードパーティ依存ライブラリの固定バージョンを導入しました。</li>
<li>プロジェクトを上流の変更から隔離することで、日々のビルドを潜在的な混乱から保護します。</li>
<li>このアップデートは、検証済みのC++サードパーティパッケージをJFrogクラウド上で独占的にホスティングし、Conan Recipe Revisions（RREV）を利用することで安定性を確保します。</li>
<li>このアプローチにより、ConanCenterのアップデートによる変更のブレークリスクが軽減される。</li>
<li>Ubuntu 22.04を使用している開発者は、これらの変更の恩恵をすぐに受けることができます。しかし、他のオペレーティング・システムの開発者は、互換性の問題を避けるために、<code translate="no">glibc</code> のバージョンをアップグレードする必要があるかもしれません。</li>
</ul></li>
</ul>
<h3 id="Critical-bug-fixes" class="common-anchor-header">重要なバグ修正</h3><ul>
<li>L0 コンパクション中にセグメントが省略され、削除データが失われる問題を修正しました。<a href="https://github.com/milvus-io/milvus/pull/33980">[#33980</a>,<a href="https://github.com/milvus-io/milvus/pull/34363">#34363</a>]</li>
<li>誤ったデータスコープ処理のために削除メッセージが転送されない問題を修正しました。<a href="https://github.com/milvus-io/milvus/pull/35313">(#35313</a>)</li>
<li><code translate="no">mmap</code> の不正な使用により発生していたSIGBUS例外を修正しました。<a href="https://github.com/milvus-io/milvus/pull/34455">[#34455</a>,<a href="https://github.com/milvus-io/milvus/pull/34530">#34530</a>].</li>
<li>不正な検索式によるクラッシュを修正しました。<a href="https://github.com/milvus-io/milvus/pull/35307">(#35307</a>)</li>
<li>ウォッチコンテキストのタイムアウト設定が正しくないためにDataNodeウォッチが失敗する問題を修正しました。<a href="https://github.com/milvus-io/milvus/pull/35017">(#35017</a>)</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>特定の依存関係をアップグレードすることで、セキュリティ脆弱性に対処した。<a href="https://github.com/milvus-io/milvus/pull/33927">[#33927</a>,<a href="https://github.com/milvus-io/milvus/pull/34693">#34693</a>]</li>
<li>長すぎる式による解析エラーを修正しました。<a href="https://github.com/milvus-io/milvus/pull/34957">(#34957</a>)</li>
<li>クエリプランの解析時に発生するメモリリークを解決しました。<a href="https://github.com/milvus-io/milvus/pull/34932">(#34932</a>)</li>
<li>動的なログレベルの変更が有効にならない問題を修正しました。<a href="https://github.com/milvus-io/milvus/pull/34777">(#34777</a>)</li>
<li>初期化されていないセグメントオフセットが原因で、成長しているデータに対する group by クエリが失敗する問題を解決しました。<a href="https://github.com/milvus-io/milvus/pull/34750">(#34750</a>)</li>
<li>Knowhere イテレータを使用する場合の検索パラメータの設定を修正した。<a href="https://github.com/milvus-io/milvus/pull/34732">(#34732</a>)</li>
<li>パーティションのロード状態をチェックするロジックを修正した。<a href="https://github.com/milvus-io/milvus/pull/34305">(#34305</a>)</li>
<li>特権キャッシュの更新が未処理のリクエストエラーにより失敗する問題を修正した。<a href="https://github.com/milvus-io/milvus/pull/34697">(#34697</a>)</li>
<li>QueryCoordの再起動後にロードされたコレクションの回復に失敗する問題を解決した。<a href="https://github.com/milvus-io/milvus/pull/35211">(#35211</a>)</li>
<li>不要なインデックスパラメータの検証を削除することで、ロードアイデンポテンスの問題を修正した。<a href="https://github.com/milvus-io/milvus/pull/35179">(#35179</a>)</li>
<li>DataCoord再起動後、<code translate="no">compressBinlog</code> が実行され、<code translate="no">reloadFromKV</code> がbinlogの<code translate="no">logID</code> を適切に満たすようにした。<a href="https://github.com/milvus-io/milvus/pull/34062">(#34062</a>)</li>
<li>DataCoordのガベージコレクション後にコレクションメタデータが削除されない問題を修正しました。<a href="https://github.com/milvus-io/milvus/pull/34884">(#34884</a>)</li>
<li>DataCoord 内の SegmentManager で、インポートによって生成されたフラッシュされたセグメントを削除することによるメモリリークを解決。<a href="https://github.com/milvus-io/milvus/pull/34651">(#34651</a>)</li>
<li>コンパクションが無効でコレクションがドロップされた場合のパニックの問題を修正。<a href="https://github.com/milvus-io/milvus/pull/34206">(#34206</a>)</li>
<li>メモリ使用量の推定アルゴリズムを強化することにより、DataNode のメモリ不足問題を修正した。<a href="https://github.com/milvus-io/milvus/pull/34203">(#34203</a>)</li>
<li>チャンクキャッシュにシングルフライトを実装することで、複数のベクトル検索要求がキャッシュミスにヒットした場合のバーストメモリ使用を防止。<a href="https://github.com/milvus-io/milvus/pull/34283">(#34283</a>)</li>
<li>コンフィギュレーションで CAS (Compare and Swap) 操作中の<code translate="no">ErrKeyNotFound</code> を捕捉。<a href="https://github.com/milvus-io/milvus/pull/34489">(#34489</a>)</li>
<li>CAS操作で誤ってフォーマットされた値を使用したために設定の更新に失敗する問題を修正した。<a href="https://github.com/milvus-io/milvus/pull/34373">(#34373</a>)</li>
</ul>
<h3 id="Miscellaneous" class="common-anchor-header">その他</h3><ul>
<li>OTLP HTTPエクスポータがサポートされ、観測および監視機能が強化されました。<a href="https://github.com/milvus-io/milvus/pull/35073">[#35073</a>,<a href="https://github.com/milvus-io/milvus/pull/35299">#35299</a>]</li>
<li>最大コレクション数やディスククォータ数を動的に変更できるようになりました。<a href="https://github.com/milvus-io/milvus/pull/34511">[#34511</a>,<a href="https://github.com/milvus-io/milvus/pull/34386">#34386</a>]</li>
<li>診断と監視を改善するために、DataNode内のL0コンパクションプロセスのトレース機能を追加しました。<a href="https://github.com/milvus-io/milvus/pull/33898">(#33898</a>)</li>
<li>コレクションごとのL0セグメントエントリ数のクォータ設定を導入。<a href="https://github.com/milvus-io/milvus/pull/34837">(#34837</a>)</li>
<li>インサート操作のレート制限メカニズムをアップサート操作にも適用するように拡張。<a href="https://github.com/milvus-io/milvus/pull/34616">(#34616</a>)</li>
<li>プロキシ CGO 呼び出し用の動的 CGO プールを実装し、リソースの使用量とパフォーマンスを最適化。<a href="https://github.com/milvus-io/milvus/pull/34842">(#34842</a>)</li>
<li>Ubuntu、Rocky、および Amazon オペレーティングシステムで DiskAnn コンパイルオプションを有効にし、これらのプラットフォームでの互換性とパフォーマンスを改善しました。<a href="https://github.com/milvus-io/milvus/pull/34244">(#34244</a>)</li>
<li>コナンをバージョン 1.64.1 にアップグレードし、最新機能との互換性を確保。<a href="https://github.com/milvus-io/milvus/pull/35216">(#35216</a>)</li>
<li>Knowhere をバージョン 2.3.7 に更新し、パフォーマンスの向上と新機能を追加。<a href="https://github.com/milvus-io/milvus/pull/34709">(#34709</a>)</li>
<li>特定のサードパーティパッケージのリビジョンを修正し、一貫したビルドを保証し、予期せぬ変更のリスクを低減した。<a href="https://github.com/milvus-io/milvus/pull/35316">(#35316</a>)</li>
</ul>
<h2 id="v246" class="common-anchor-header">v2.4.6<button data-href="#v246" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日: 2024年7月16日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.6</td><td>2.4.4</td><td>2.4.2</td><td>2.4.4</td></tr>
</tbody>
</table>
<p>Milvus v2.4.6は、パニック、メモリリーク、削除時のデータ損失などの重大な問題に対処したバグ修正リリースです。また、監視メトリクスの強化、Goバージョンの1.21へのアップグレード、RESTful count(*)クエリのユーザーエクスペリエンスの向上など、いくつかの最適化も行われています。</p>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>RESTful APIクエリの使い勝手を向上しました<a href="https://github.com/milvus-io/milvus/pull/34444">(#34444</a>)。</li>
<li>Goのバージョンを1.20から1.21に更新しました<a href="https://github.com/milvus-io/milvus/pull/33940">(#33940</a>)。</li>
<li>ヒストグラム・メトリック・バケットを最適化し、バケットの粒度をより細かくしました<a href="https://github.com/milvus-io/milvus/pull/34592">(#34592</a>)。</li>
<li>Pulsar依存バージョンを2.8.2から2.9.5にアップグレード。Milvus 2.4.6以降、Pulsarを2.9.5にアップグレードすることを推奨します。</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>GetReplicas APIがnilステータスを返す問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/34019">(#34019</a>)。</li>
<li>クエリが削除されたレコードを返す問題を修正した<a href="https://github.com/milvus-io/milvus/pull/34502">(#34502</a>)。</li>
<li>IndexNode が不正な寿命制御によって停止中にスタックする問題を解決した<a href="https://github.com/milvus-io/milvus/pull/34559">(#34559</a>)。</li>
<li>ワーカーがオフラインの場合に、主キーオラクルオブジェクトのメモリリークを修正した<a href="https://github.com/milvus-io/milvus/pull/34020">(#34020</a>)。</li>
<li>ChannelManagerImplV2が正しいNodeに通知されるように修正し、ループクロージャにおけるパラメータ取得の問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/34004">(#34004</a>)。</li>
<li>ImportTask segmentsInfoにおける読み書きのデータ競合を、ディープコピーを実装することで修正しました<a href="https://github.com/milvus-io/milvus/pull/34126">(#34126</a>)。</li>
<li>legacyVersionWithoutRPCWatch」設定オプションのバージョン情報を修正し、ローリングアップグレード時のエラーを防止しました<a href="https://github.com/milvus-io/milvus/pull/34185">(#34185</a>)。</li>
<li>ロードされるパーティション数のメトリックを修正しました<a href="https://github.com/milvus-io/milvus/pull/34195">(#34195</a>)。</li>
<li>segcoreのトレース設定時に<code translate="no">otlpSecure</code> の設定を渡すようにした<a href="https://github.com/milvus-io/milvus/pull/34210">(#34210</a>)。</li>
<li>DataCoordのプロパティが誤って上書きされる問題を修正した<a href="https://github.com/milvus-io/milvus/pull/34240">(#34240</a>)。</li>
<li>新しく作成された2つのメッセージストリームが誤ってマージされることによるデータ損失の問題を解決した<a href="https://github.com/milvus-io/milvus/pull/34563">(#34563</a>)。</li>
<li>msgstreamが無効なpchannelを消費しようとすることによるパニックを修正しました<a href="https://github.com/milvus-io/milvus/pull/34230">(#34230</a>)。</li>
<li>インポートによって孤児ファイルが生成される場合がある問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/34071">(#34071</a>)。</li>
<li>セグメント内で主キーが重複していた場合に、クエリ結果が不完全になる問題を修正した<a href="https://github.com/milvus-io/milvus/pull/34302">(#34302</a>)。</li>
<li>L0コンパクションで、封印されたセグメントが欠落する問題を解決した<a href="https://github.com/milvus-io/milvus/pull/34566">(#34566</a>)。</li>
<li>ガベージコレクション後に生成されるchannel-cpメタにダーティデータが含まれる問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/34609">(#34609</a>)。</li>
<li>RootCoordの再起動後にdatabase_numが0になるメトリクスを修正しました<a href="https://github.com/milvus-io/milvus/pull/34010">(#34010</a>)。</li>
<li>DataCoordのSegmentManagerにおいて、インポートによって生成されたフラッシュされたセグメントを削除することによるメモリリークを修正しました<a href="https://github.com/milvus-io/milvus/pull/34652">(#34652</a>)。</li>
<li>DataCoordの再起動後にcompressBinlogがbinlogのlogIDを埋めるようにし、KVからの適切なリロードを保証するようにした<a href="https://github.com/milvus-io/milvus/pull/34064">(#34064</a>)。</li>
</ul>
<h2 id="v245" class="common-anchor-header">v2.4.5<button data-href="#v245" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日：2024年6月18日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.5</td><td>2.4.4</td><td>2.4.1</td><td>2.4.3</td></tr>
</tbody>
</table>
<p>Milvus 2.4.5のリリースでは、パフォーマンス、安定性、および機能性を向上させるために、いくつかの改善とバグ修正が導入されています。Milvus 2.4.5では、スパース、float16、bfloat16ベクトル検索が自動インデックス作成機能により簡素化され、Bloomフィルター最適化機能により検索、削除、コンパクションが高速化され、読み込み時間の短縮とL0セグメントのインポート対応によりデータ管理に取り組んでいます。また、効率的な高次元スパースデータ検索のためのスパースHNSWインデックスを導入し、スパースフロートベクトルをサポートするRESTful APIを強化し、重要なバグを修正して安定性を向上させました。</p>
<h3 id="New-Features" class="common-anchor-header">新機能</h3><ul>
<li>describe/alterデータベースAPIにrbacサポートを追加しました<a href="https://github.com/milvus-io/milvus/pull/33804">(#33804</a>)。</li>
<li>スパースベクトル用のHNSWインデックスの構築をサポート<a href="https://github.com/milvus-io/milvus/pull/33653">しました(#33653</a>,<a href="https://github.com/milvus-io/milvus/pull/33662">#33662</a>)。</li>
<li>バイナリベクトルのディスクインデックスの構築をサポートしました<a href="https://github.com/milvus-io/milvus/pull/33575">(#33575</a>)。</li>
<li>RESTful v2でスパースベクタタイプをサポートしました<a href="https://github.com/milvus-io/milvus/pull/33555">(#33555</a>)<a href="https://github.com/milvus-io/milvus/pull/33555">。</a></li>
<li>コンポーネントを停止するための/management/stop RESTful APIを追加しました<a href="https://github.com/milvus-io/milvus/pull/33799">(#33799</a>)。</li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>maxPartitionNumのデフォルト値を1024に設定<a href="https://github.com/milvus-io/milvus/pull/33950">(#33950</a>)</li>
<li>接続不可エラー時に接続を強制的にリセットできるようにした<a href="https://github.com/milvus-io/milvus/pull/33910">(#33910</a>)</li>
<li>コレクションレベルのフラッシュレートリミッターを有効にした<a href="https://github.com/milvus-io/milvus/pull/33864">(#33864</a>)</li>
<li>セグメント予測を高速化するために、ブルームフィルタの適用を並列に実行するようにした<a href="https://github.com/milvus-io/milvus/pull/33793">(#33793</a>)</li>
<li>json.Unmarshalを高速化するため、削除ログのunmarshalにfastjson libを使用<a href="https://github.com/milvus-io/milvus/pull/33802">(#33802</a>)</li>
<li>BatchPkExistを使用して、ブルームフィルタのfunc呼び出しコストを削減しました<a href="https://github.com/milvus-io/milvus/pull/33752">(#33752</a>)。</li>
<li>小さなコレクションの読み込みを高速化<a href="https://github.com/milvus-io/milvus/pull/33746">(#33746</a>)</li>
<li>L0セグメントへの削除データのインポートをサポート(<a href="https://github.com/milvus-io/milvus/pull/33712">#33712</a>)。</li>
<li>同じタスクが何度も実行されないように、タイムアウトされるマークコンパクションのタスクをスキップ<a href="https://github.com/milvus-io/milvus/pull/33833">(#33833</a>)</li>
<li>numpyの一括挿入において、float16およびbfloat16ベクトルをBinaryVectorと同じものとして扱うようにしました(<a href="https://github.com/milvus-io/milvus/pull/33788">#33788</a>)。</li>
<li>seekメソッドにincludeCurrentMsgフラグを追加しました<a href="https://github.com/milvus-io/milvus/pull/33743">(#33743</a>)。</li>
<li>mergeInterval、targetBufSize、maxTolerantLagof msgdispatcherを設定に追加しました<a href="https://github.com/milvus-io/milvus/pull/33680">(#33680</a>)。</li>
<li>スパースベクトルのGetVectorByIDを改善しました<a href="https://github.com/milvus-io/milvus/pull/33652">(#33652</a>)<a href="https://github.com/milvus-io/milvus/pull/33652">。</a></li>
<li>不要なコピーと関数呼び出しのコストを削減するためにStringPrimarykeyを削除しました(<a href="https://github.com/milvus-io/milvus/pull/33649">#33649</a>)。</li>
<li>バイナリ/スパースデータ型の自動インデックスマッピングを追加しました<a href="https://github.com/milvus-io/milvus/pull/33625">(#33625</a>)<a href="https://github.com/milvus-io/milvus/pull/33625">。</a></li>
<li>一部のキャッシュを最適化し、メモリ使用量を削減した<a href="https://github.com/milvus-io/milvus/pull/33560">(#33560</a>)</li>
<li>インポート/プレインポートタスクの実行インターフェイスを抽象化(<a href="https://github.com/milvus-io/milvus/pull/33607">#33607</a>)</li>
<li>バッファ挿入時にタイムスタンプにマップpkを使用することで、bfの発生を抑制<a href="https://github.com/milvus-io/milvus/pull/33582">(#33582</a>)</li>
<li>インポートの冗長なメタ操作を回避(<a href="https://github.com/milvus-io/milvus/pull/33519">#33519</a>)</li>
<li>ディスククォータ情報のロギングを改善し、UseDefaultConsistencyフラグを追加し、不要なログを削除した<a href="https://github.com/milvus-io/milvus/pull/33597">(#33597</a>,<a href="https://github.com/milvus-io/milvus/pull/33644">#33644</a>,<a href="https://github.com/milvus-io/milvus/pull/33670">#33670</a>)。</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>queryHookがベクトル型を認識できないバグを修正しました<a href="https://github.com/milvus-io/milvus/pull/33911">(#33911</a>)。</li>
<li>反復変数partitionIDをキャプチャして使用しないようにした<a href="https://github.com/milvus-io/milvus/pull/33970">(#33970</a>)。</li>
<li>バイナリベクタやスパースベクタでMilvusがAutoIndexを作成できない場合がある不具合を修正しました<a href="https://github.com/milvus-io/milvus/pull/33867">(#33867</a>)。</li>
<li>indexnodeが全てのベクトルの無効なインデックスパラメータに対してインデックス作成を再試行する場合があるバグを修正しました(#<a href="https://github.com/milvus-io/milvus/pull/33878">33878</a>)。</li>
<li>ロードとリリースが同時に発生した場合にサーバがクラッシュすることがあるバグを修正しました<a href="https://github.com/milvus-io/milvus/pull/33699">(#33699</a>)。</li>
<li>設定値のキャッシュの一貫性を改善しました<a href="https://github.com/milvus-io/milvus/pull/33797">(#33797</a>)。</li>
<li>削除時にデータが失われる可能性がある問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33821">(#33821</a>)。</li>
<li>コレクションを削除した後に、DroppedAtフィールド(削除のタイムスタンプ)が設定されるようにした<a href="https://github.com/milvus-io/milvus/pull/33767">(#33767</a>)。</li>
<li>Milvusがバイナリベクタのデータサイズを正しく扱えない問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33751">(#33751</a>)。</li>
<li>機密性の高いKafkaの認証情報がプレーンテキストでログに記録されないようにした<a href="https://github.com/milvus-io/milvus/pull/33694">(#33694</a>,<a href="https://github.com/milvus-io/milvus/pull/33747">#33747</a>)。</li>
<li>Milvus が複数のベクトルフィールドを持つデータを正しくインポートできるようにした<a href="https://github.com/milvus-io/milvus/pull/33724">(#33724</a>)。</li>
<li>インポートジョブが存在するかどうかを開始前にチェックすることで、インポートの信頼性を向上させた。<a href="https://github.com/milvus-io/milvus/pull/33673">(#33673</a>)</li>
<li>スパースHNSWインデックス(内部機能)の取り扱いを改善しました<a href="https://github.com/milvus-io/milvus/pull/33714">(#33714</a>)。</li>
<li>メモリリークを回避するためにベクタメモリをクリーンアップ<a href="https://github.com/milvus-io/milvus/pull/33708">(#33708</a>)。</li>
<li>状態ロックの問題を修正することにより、よりスムーズな非同期ウォームアップを保証<a href="https://github.com/milvus-io/milvus/pull/33687">(#33687</a>)。</li>
<li>クエリイテレータで結果が欠落するバグを修正。<a href="https://github.com/milvus-io/milvus/pull/33506">(#33506</a>)</li>
<li>インポートセグメントサイズが不均等になる場合があったバグを修正 (<a href="https://github.com/milvus-io/milvus/pull/33634">#33634</a>)。</li>
<li>bf16、fp16、バイナリベクタ型の不正なデータサイズの取り扱いを修正<a href="https://github.com/milvus-io/milvus/pull/33488">(#33488</a>)</li>
<li>L0 コンパクタに関する潜在的な問題を修正し、安定性を向上<a href="https://github.com/milvus-io/milvus/pull/33564">(#33564</a>)。</li>
<li>動的な設定の更新がキャッシュに正しく反映されるようにした。<a href="https://github.com/milvus-io/milvus/pull/33590">(#33590</a>)</li>
<li>RootCoordQuotaStates メトリックの精度を改善しました(<a href="https://github.com/milvus-io/milvus/pull/33601">#33601</a>)。</li>
<li>ロードされたエンティティの数を正確に報告するようにしました<a href="https://github.com/milvus-io/milvus/pull/33522">(#33522</a>)。</li>
<li>例外ログにおいて、より完全な情報を提供するようにした。 <a href="https://github.com/milvus-io/milvus/pull/33396">(#33396</a>)</li>
<li>不要なグループチェッカを削除し、クエリパイプラインを最適化した<a href="https://github.com/milvus-io/milvus/pull/33485">(#33485</a>)</li>
<li>インデックスノードのディスク容量をより正確に確認するために、ローカルストレージのパスを使用するようにしました。<a href="https://github.com/milvus-io/milvus/pull/33505">(#33505</a>)</li>
<li>hasMoreResultのヒット数が制限値より大きい場合にfalseを返すことがあった問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33642">(#33642</a>)<a href="https://github.com/milvus-io/milvus/pull/33642">。</a></li>
<li>デリゲータの bf のロードを遅延させ、worker のメモリ不足時に bf が何度もロードされないようにした<a href="https://github.com/milvus-io/milvus/pull/33650">(#33650</a>)- queryHook がベクトル型を認識できないバグを修正した<a href="https://github.com/milvus-io/milvus/pull/33911">(#33911</a>)- queryHook がベクトル型を認識できないバグを修正した<a href="https://github.com/milvus-io/milvus/pull/33911">(#33911</a>)- queryHook がベクトル型を認識できないバグを修正した<a href="https://github.com/milvus-io/milvus/pull/33911">(#33911</a>)</li>
<li>イテレーション変数 partitionID をキャプチャして使用しないようにした<a href="https://github.com/milvus-io/milvus/pull/33970">(#33970</a>)</li>
<li>バイナリベクタやスパースベクタでMilvusがAutoIndexを作成できない場合があるバグを修正<a href="https://github.com/milvus-io/milvus/pull/33867">(#33867</a>)</li>
<li>indexnodeが全てのベクトルの無効なインデックスパラメータに対してインデックス作成を再試行する場合があるバグを修正しました(#<a href="https://github.com/milvus-io/milvus/pull/33878">33878</a>)。</li>
<li>ロードとリリースが同時に発生した場合にサーバがクラッシュすることがあるバグを修正しました<a href="https://github.com/milvus-io/milvus/pull/33699">(#33699</a>)。</li>
<li>設定値のキャッシュの一貫性を改善しました<a href="https://github.com/milvus-io/milvus/pull/33797">(#33797</a>)。</li>
<li>削除時にデータが失われる可能性がある問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33821">(#33821</a>)。</li>
<li>コレクションを削除した後に、DroppedAtフィールド(削除のタイムスタンプ)が設定されるようにした<a href="https://github.com/milvus-io/milvus/pull/33767">(#33767</a>)。</li>
<li>Milvusがバイナリベクタのデータサイズを正しく扱えない問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33751">(#33751</a>)。</li>
<li>機密性の高いKafkaの認証情報がプレーンテキストでログに記録されないようにした<a href="https://github.com/milvus-io/milvus/pull/33694">(#33694</a>,<a href="https://github.com/milvus-io/milvus/pull/33747">#33747</a>)。</li>
<li>Milvus が複数のベクトルフィールドを持つデータを正しくインポートできるようにした<a href="https://github.com/milvus-io/milvus/pull/33724">(#33724</a>)。</li>
<li>インポートジョブが存在するかどうかを開始前にチェックすることで、インポートの信頼性を向上させた。<a href="https://github.com/milvus-io/milvus/pull/33673">(#33673</a>)</li>
<li>スパースHNSWインデックス(内部機能)の取り扱いを改善しました<a href="https://github.com/milvus-io/milvus/pull/33714">(#33714</a>)。</li>
<li>メモリリークを回避するためにベクタメモリをクリーンアップ<a href="https://github.com/milvus-io/milvus/pull/33708">(#33708</a>)。</li>
<li>状態ロックの問題を修正することにより、よりスムーズな非同期ウォームアップを保証<a href="https://github.com/milvus-io/milvus/pull/33687">(#33687</a>)。</li>
<li>クエリイテレータで結果が欠落するバグを修正。<a href="https://github.com/milvus-io/milvus/pull/33506">(#33506</a>)</li>
<li>インポートセグメントサイズが不均等になる場合があったバグを修正 (<a href="https://github.com/milvus-io/milvus/pull/33634">#33634</a>)。</li>
<li>bf16、fp16、バイナリベクタ型の不正なデータサイズの取り扱いを修正<a href="https://github.com/milvus-io/milvus/pull/33488">(#33488</a>)</li>
<li>L0 コンパクタに関する潜在的な問題を修正し、安定性を向上<a href="https://github.com/milvus-io/milvus/pull/33564">(#33564</a>)。</li>
<li>動的な設定の更新がキャッシュに正しく反映されるようにした。<a href="https://github.com/milvus-io/milvus/pull/33590">(#33590</a>)</li>
<li>RootCoordQuotaStates メトリックの精度を改善しました(<a href="https://github.com/milvus-io/milvus/pull/33601">#33601</a>)。</li>
<li>ロードされたエンティティの数を正確に報告するようにしました<a href="https://github.com/milvus-io/milvus/pull/33522">(#33522</a>)。</li>
<li>例外ログにおいて、より完全な情報を提供するようにした。 <a href="https://github.com/milvus-io/milvus/pull/33396">(#33396</a>)</li>
<li>不要なグループチェッカを削除し、クエリパイプラインを最適化した<a href="https://github.com/milvus-io/milvus/pull/33485">(#33485</a>)</li>
<li>インデックスノードのディスク容量をより正確に確認するために、ローカルストレージのパスを使用するようにしました。<a href="https://github.com/milvus-io/milvus/pull/33505">(#33505</a>)</li>
<li>hasMoreResultのヒット数が制限値より大きい場合にfalseを返すことがあった問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33642">(#33642</a>)<a href="https://github.com/milvus-io/milvus/pull/33642">。</a></li>
<li>デリゲータの bf のロードを遅延させ、worker のメモリ不足時に bf が何度もロードされないようにした<a href="https://github.com/milvus-io/milvus/pull/33650">(#33650</a>)。</li>
</ul>
<h2 id="v244" class="common-anchor-header">v2.4.4<button data-href="#v244" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日: 2024年5月31日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDK バージョン</th><th>Java SDK バージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.4</td><td>2.4.3</td><td>2.4.1</td><td>2.4.2</td></tr>
</tbody>
</table>
<p>Milvus v2.4.4では、パフォーマンスと安定性の向上を目的としたいくつかの重要なバグ修正と改善が含まれています。特に、<strong>バルクインサートの統計ログが不正にガベージコレクションさ</strong>れ、データの整合性に影響を及ぼす可能性が<strong>あるという重大な問題を解決</strong>しました。<strong>これらの修正の恩恵を受けるために、すべてのv2.4ユーザーがこのバージョンにアップグレードすることを強くお勧めします。</strong></p>
<p><strong>バルク・インサートを使用している場合は、データの整合性を保つために、できるだけ早い機会にv2.4.4にアップグレードしてください。</strong></p>
<h3 id="Critical-bug-fixes" class="common-anchor-header">重大なバグ修正</h3><ul>
<li>統計ログのIDを埋め、その正しさを検証した<a href="https://github.com/milvus-io/milvus/pull/33478">(#33478</a>)</li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>ARM SVE用のビットセットをアップグレードした<a href="https://github.com/milvus-io/milvus/pull/33440">(#33440</a>)</li>
<li>GCC-13でのMilvusコンパイルを有効にした<a href="https://github.com/milvus-io/milvus/pull/33441">(#33441</a>)</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>すべての権限が付与されている場合に空のコレクションを表示するようにした<a href="https://github.com/milvus-io/milvus/pull/33454">(#33454</a>)。</li>
<li>CMakeがx86_64だけでなく現在のプラットフォーム用にダウンロードとインストールを行うようにした<a href="https://github.com/milvus-io/milvus/pull/33439">(#33439</a>)<a href="https://github.com/milvus-io/milvus/pull/33439">。</a></li>
</ul>
<h2 id="v243" class="common-anchor-header">v2.4.3<button data-href="#v243" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日: 2024年5月29日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.3</td><td>2.4.3</td><td>2.4.1</td><td>2.4.2</td></tr>
</tbody>
</table>
<p>Milvusバージョン2.4.3では、パフォーマンスと信頼性を向上させるために、多くの機能、改善、バグ修正が行われました。特筆すべき機能強化としては、スパースフロートベクトル一括挿入のサポートや、最適化されたブルームフィルタアクセラレーションなどが挙げられる。改善点は、動的な設定更新からメモリ使用量の最適化まで、さまざまな分野に及んだ。バグ修正では、パニックシナリオのような重要な問題に対処し、よりスムーズなシステム運用を確保しました。このリリースは、機能強化、パフォーマンスの最適化、そして堅牢なユーザーエクスペリエンスの提供に対するMilvusの継続的なコミットメントを強調するものです。</p>
<h3 id="Features" class="common-anchor-header">特徴</h3><ul>
<li>binlog/json/parquetのスパースフロートベクトル一括挿入をサポートしました<a href="https://github.com/milvus-io/milvus/pull/32649">。</a></li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>RPCに基づくDatacoord/nodeウォッチチャネルを実装しました<a href="https://github.com/milvus-io/milvus/pull/32036">(#32036</a>)</li>
<li>ブルームフィルタを最適化し、削除フィルタリングを高速化した<a href="https://github.com/milvus-io/milvus/pull/32642">(#32642</a> <a href="https://github.com/milvus-io/milvus/pull/33329">、#33329</a> <a href="https://github.com/milvus-io/milvus/pull/33284">、#33284</a>)</li>
<li>スカラーインデックスに生データがない場合、mmap経由で生データをロードするようにした<a href="https://github.com/milvus-io/milvus/pull/33317">(#33317</a>)。</li>
<li>milvusの設定をmilvus.yamlに同期した<a href="https://github.com/milvus-io/milvus/pull/33322">(#33322</a>,<a href="https://github.com/milvus-io/milvus/pull/32920">#32920</a>,<a href="https://github.com/milvus-io/milvus/pull/32857">#32857</a>,<a href="https://github.com/milvus-io/milvus/pull/32946">#32946</a>)。</li>
<li>knowhereのバージョンを更新しました<a href="https://github.com/milvus-io/milvus/pull/33310">(#33310</a> <a href="https://github.com/milvus-io/milvus/pull/32931">、#32931</a> <a href="https://github.com/milvus-io/milvus/pull/33043">、#33043</a>)。</li>
<li>QueryCoordでバランサポリシーの動的更新を可能にしました<a href="https://github.com/milvus-io/milvus/pull/33272">(#33272</a>)。</li>
<li>ロガーの割り当てを最小化するため、書き込みバッファに事前に作成したロガーを使用するようにした<a href="https://github.com/milvus-io/milvus/pull/33304">(#33304</a>)</li>
<li>パラメータチェックを改善した<a href="https://github.com/milvus-io/milvus/pull/32777">(#32777</a>,<a href="https://github.com/milvus-io/milvus/pull/33271">#33271</a>,<a href="https://github.com/milvus-io/milvus/pull/33218">#33218</a>)。</li>
<li>チェックポイントの不正なメッセージIDを無視するパラメータを追加しました<a href="https://github.com/milvus-io/milvus/pull/33249">(#33249</a>)。</li>
<li>プラグインの初期化失敗処理を制御する設定を追加<a href="https://github.com/milvus-io/milvus/pull/32680">(#32680</a>)</li>
<li>knowhere用のスコア計算一貫性設定を追加した<a href="https://github.com/milvus-io/milvus/pull/32997">(#32997</a>)</li>
<li>パブリックロールパーミッションの初期化を制御する設定オプションを導入した<a href="https://github.com/milvus-io/milvus/pull/33174">(#33174</a>)</li>
<li>フィールド読み込み時のメモリ使用量を最適化した<a href="https://github.com/milvus-io/milvus/pull/33196">(#33196</a>)</li>
<li>チャネルマネージャv2の実装を改良した<a href="https://github.com/milvus-io/milvus/pull/33172">(#33172</a>,<a href="https://github.com/milvus-io/milvus/pull/33121">#33121</a>,<a href="https://github.com/milvus-io/milvus/pull/33014">#33014</a>)</li>
<li>binlogのメモリ上のデータサイズを追跡する機能を追加<a href="https://github.com/milvus-io/milvus/pull/33025">(#33025</a>)</li>
<li>セグメントインデックスファイルのサイズに関するメトリクスを追加<a href="https://github.com/milvus-io/milvus/pull/32979">(#32979</a>,<a href="https://github.com/milvus-io/milvus/pull/33305">#33305</a>)</li>
<li>DeleteをDeletePartialMatchに置き換え、メトリクスを削除した<a href="https://github.com/milvus-io/milvus/pull/33029">(#33029</a>)</li>
<li>セグメントタイプに応じた関連データサイズを取得<a href="https://github.com/milvus-io/milvus/pull/33017">(#33017</a>)</li>
<li>メタストアのチャンネルノード情報を整理<a href="https://github.com/milvus-io/milvus/pull/32988">(#32988</a>)</li>
<li>データノードブローカからルートコードを削除<a href="https://github.com/milvus-io/milvus/pull/32818">(#32818</a>)</li>
<li>バッチアップロードを可能にした<a href="https://github.com/milvus-io/milvus/pull/32788">(#32788</a>)</li>
<li>パーティションキー使用時のデフォルトのパーティション番号を16に変更した<a href="https://github.com/milvus-io/milvus/pull/32950">(#32950</a>)</li>
<li>非常に大きなtop-kクエリの削減性能を改善した<a href="https://github.com/milvus-io/milvus/pull/32871">(#32871</a>)</li>
<li>書き込みとコンパクションを高速化するためにTestLocations機能を利用しました<a href="https://github.com/milvus-io/milvus/pull/32948">(#32948</a>)。</li>
<li>プランパーサプールを最適化し、不要な再利用を回避しました<a href="https://github.com/milvus-io/milvus/pull/32869">(#32869</a>)。</li>
<li>ロード速度を改善しました<a href="https://github.com/milvus-io/milvus/pull/32898">(#32898</a>)。</li>
<li>restv2でコレクションのデフォルト一貫性レベルを使用するようにした<a href="https://github.com/milvus-io/milvus/pull/32956">(#32956</a>)</li>
<li>rest APIにコスト応答を追加しました<a href="https://github.com/milvus-io/milvus/pull/32620">(#32620</a>)。</li>
<li>チャネル排他バランスポリシーを有効にした<a href="https://github.com/milvus-io/milvus/pull/32911">(#32911</a>)。</li>
<li>プロキシで describedatabase API を公開<a href="https://github.com/milvus-io/milvus/pull/32732">(#32732</a>)</li>
<li>コレクションでRGを取得する際にcoll2replicaマッピングを利用するようにした<a href="https://github.com/milvus-io/milvus/pull/32892">(#32892</a>)</li>
<li>検索とクエリのトレースを追加<a href="https://github.com/milvus-io/milvus/pull/32734">(#32734</a>)</li>
<li>opentelemetry トレースの動的設定をサポート<a href="https://github.com/milvus-io/milvus/pull/32169">(#32169</a>)</li>
<li>leaderviewを更新する際、チャンネル結果の繰り返しを回避<a href="https://github.com/milvus-io/milvus/pull/32887">(#32887</a>)</li>
<li>寄木細工のベクトルオフセットの取り扱いを最適化<a href="https://github.com/milvus-io/milvus/pull/32822">(#32822</a>)</li>
<li>コレクションでのデータコードセグメントのフィルタリングを改善<a href="https://github.com/milvus-io/milvus/pull/32831">(#32831</a>)</li>
<li>ログのレベルと頻度を調整<a href="https://github.com/milvus-io/milvus/pull/33042">(#33042</a> <a href="https://github.com/milvus-io/milvus/pull/32838">、#32838</a> <a href="https://github.com/milvus-io/milvus/pull/33337">、#33337</a>)</li>
<li>バランス停止後にバランスを停止できるようにした<a href="https://github.com/milvus-io/milvus/pull/32812">(#32812</a>)。</li>
<li>リーダーの位置が変更された場合に、シャードリーダーのキャッシュを更新した<a href="https://github.com/milvus-io/milvus/pull/32470">(#32470</a>)。</li>
<li>非推奨のAPIおよびフィールドを削除した<a href="https://github.com/milvus-io/milvus/pull/32808">(#32808</a>,<a href="https://github.com/milvus-io/milvus/pull/32704">#32704</a>)。</li>
<li>文字列の比較をint型に変換するmetautil.channelを追加<a href="https://github.com/milvus-io/milvus/pull/32749">(#32749</a>)</li>
<li>querynodeが新しいコレクションを発見した場合に、ペイロードライターのエラーメッセージとログにタイプ情報を追加しました<a href="https://github.com/milvus-io/milvus/pull/32522">(#32522</a>)。</li>
<li>パーティションキーでコレクションを作成する場合に、パーティション番号をチェックするようにした<a href="https://github.com/milvus-io/milvus/pull/32670">(#32670</a>)。</li>
<li>ウォッチに失敗した場合、レガシーl0セグメントを削除した<a href="https://github.com/milvus-io/milvus/pull/32725">(#32725</a>)</li>
<li>リクエストの出力タイプを改善した<a href="https://github.com/milvus-io/milvus/pull/33319">(#33319</a>)</li>
<li>型を取得する前に配列フィールドデータがnilであるかチェックするようにした<a href="https://github.com/milvus-io/milvus/pull/33311">(#33311</a>)</li>
<li>ノードのDelete/AddNode操作が失敗した場合にエラーを返すようにした<a href="https://github.com/milvus-io/milvus/pull/33258">(#33258</a>)。</li>
<li>データノードのサーバIDを更新できるようにしました<a href="https://github.com/milvus-io/milvus/pull/31597">(#31597</a>)。</li>
<li>コレクションリリースでquerynodeメトリクスのクリーンアップを統一した<a href="https://github.com/milvus-io/milvus/pull/32805">(#32805</a>)</li>
<li>スカラー自動インデックスの設定が不正なバージョンだった問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/32795">(#32795</a>)。</li>
<li>インデックスの作成/変更時のインデックスパラメータチェックを改良しました<a href="https://github.com/milvus-io/milvus/pull/32712">(#32712</a>)。</li>
<li>冗長なレプリカリカバリを削除した<a href="https://github.com/milvus-io/milvus/pull/32985">(#32985</a>)</li>
<li>チャネルメタテーブルで200kセグメント以上の書き込みを可能にした<a href="https://github.com/milvus-io/milvus/pull/33300">(#33300</a>)</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>レートリミットインタセプタにおいて、データベースが存在しない場合にパニックを起こす問題を修正した<a href="https://github.com/milvus-io/milvus/pull/33308">(#33308</a>)。</li>
<li>quotacenter メトリクスの収集で、不正なパラメータが原因で失敗する問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33399">(#33399</a>)<a href="https://github.com/milvus-io/milvus/pull/33399">。</a></li>
<li>processactivestandbyがエラーを返した場合のパニックを修正しました<a href="https://github.com/milvus-io/milvus/pull/33372">(#33372</a>)。</li>
<li>restful v2でnq &gt; 1の場合に検索結果が切り捨てられる問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/33363">(#33363</a>)。</li>
<li>restful v2のロール操作にデータベース名フィールドを追加した<a href="https://github.com/milvus-io/milvus/pull/33291">(#33291</a>)</li>
<li>グローバルレート制限が動作しない問題を修正<a href="https://github.com/milvus-io/milvus/pull/33336">(#33336</a>)</li>
<li>インデックス構築の失敗によるパニックを修正した<a href="https://github.com/milvus-io/milvus/pull/33314">(#33314</a>)</li>
<li>segcoreにおけるスパースベクタの検証を追加し、合法性を確保した<a href="https://github.com/milvus-io/milvus/pull/33312">(#33312</a>)</li>
<li>タスク完了後にsyncmgrからタスクを削除するようにした<a href="https://github.com/milvus-io/milvus/pull/33303">(#33303</a>)</li>
<li>データインポート時のパーティションキーフィルタリングの失敗を修正した<a href="https://github.com/milvus-io/milvus/pull/33277">(#33277</a>)</li>
<li>noop exporterを使用した場合にtraceIDを生成できない問題を修正<a href="https://github.com/milvus-io/milvus/pull/33208">(#33208</a>)</li>
<li>クエリ結果の取得を改善した<a href="https://github.com/milvus-io/milvus/pull/33179">(#33179</a>)</li>
<li>チェックポイントラグメトリクスの漏えいを防ぐため、チャネルのチェックポイントを削除するようにした<a href="https://github.com/milvus-io/milvus/pull/33201">(#33201</a>)</li>
<li>進行停止中にクエリノードがスタックする問題を修正<a href="https://github.com/milvus-io/milvus/pull/33154">(#33154</a>)</li>
<li>フラッシュレスポンスに欠落していたセグメントを修正<a href="https://github.com/milvus-io/milvus/pull/33061">(#33061</a>)</li>
<li>サブミット操作がべき等であるようにした<a href="https://github.com/milvus-io/milvus/pull/33053">(#33053</a>)</li>
<li>ストリーミングリーダでバッチごとに新しいスライスを割り当てた<a href="https://github.com/milvus-io/milvus/pull/33360">(#33360</a>)</li>
<li>QueryCoord再起動後にリソースグループからオフラインノードを削除しました<a href="https://github.com/milvus-io/milvus/pull/33233">(#33233</a>)<a href="https://github.com/milvus-io/milvus/pull/33233">。</a></li>
<li>completedCompactorのl0コンパクタを削除しました<a href="https://github.com/milvus-io/milvus/pull/33216">(#33216</a>)。</li>
<li>リミッター初期化時にクォータ値をリセットするようにした<a href="https://github.com/milvus-io/milvus/pull/33152">(#33152</a>)</li>
<li>etcdの制限を超過する問題を修正した<a href="https://github.com/milvus-io/milvus/pull/33041">(#33041</a>)</li>
<li>フィールド数が多すぎることによるetcdトランザクションの上限超過を解決した<a href="https://github.com/milvus-io/milvus/pull/33040">(#33040</a>)</li>
<li>GetNumRowsOfPartitionにおけるRLockの再入力を削除した<a href="https://github.com/milvus-io/milvus/pull/33045">(#33045</a>)。</li>
<li>LeaderCacheObserverをSyncAllの前に起動するようにした<a href="https://github.com/milvus-io/milvus/pull/33035">(#33035</a>)。</li>
<li>解放されたスタンバイチャネルのバランシングを有効にした<a href="https://github.com/milvus-io/milvus/pull/32986">(#32986</a>)</li>
<li>サーバ初期化の前にアクセスロガーを初期化するようにした<a href="https://github.com/milvus-io/milvus/pull/32976">(#32976</a>)</li>
<li>コンパクタが空のセグメントをクリアできるようにした<a href="https://github.com/milvus-io/milvus/pull/32821">(#32821</a>)</li>
<li>l0 コンパクションでデルタログエントリ番号と時間範囲を埋めるようにした<a href="https://github.com/milvus-io/milvus/pull/33004">(#33004</a>)。</li>
<li>シャードリーダのキャッシュデータの競合によるプロキシのクラッシュを修正<a href="https://github.com/milvus-io/milvus/pull/32971">(#32971</a>)</li>
<li>ロードインデックスメトリックの時間単位を修正しました<a href="https://github.com/milvus-io/milvus/pull/32935">(#32935</a>)。</li>
<li>停止中のクエリノードのセグメントを正常に解放できない問題を修正<a href="https://github.com/milvus-io/milvus/pull/32929">(#32929</a>)</li>
<li>インデックスリソースの見積もりを修正しました<a href="https://github.com/milvus-io/milvus/pull/32842">(#32842</a>)。</li>
<li>チャネルチェックポイントをデルタ位置に設定するようにした<a href="https://github.com/milvus-io/milvus/pull/32878">(#32878</a>)。</li>
<li>syncmgrがfutureを返す前にキーをロックするようにした<a href="https://github.com/milvus-io/milvus/pull/32865">(#32865</a>)。</li>
<li>転置インデックスが1セグメントしか持たないようにした<a href="https://github.com/milvus-io/milvus/pull/32858">(#32858</a>)。</li>
<li>コンパクショントリガーが2つの同じセグメントを選択する問題を修正<a href="https://github.com/milvus-io/milvus/pull/32800">(#32800</a>)</li>
<li>binlogインポートでパーティション名を指定できない問題を修正した<a href="https://github.com/milvus-io/milvus/pull/32730">(#32730</a>,<a href="https://github.com/milvus-io/milvus/pull/33027">#33027</a>)。</li>
<li>寄木細工のインポートで動的カラムをオプションにした<a href="https://github.com/milvus-io/milvus/pull/32738">(#32738</a>)</li>
<li>データ挿入時に自動IDチェックをスキップするようにした<a href="https://github.com/milvus-io/milvus/pull/32775">(#32775</a>)</li>
<li>挿入フィールドデータの行数をスキーマで検証するようにした<a href="https://github.com/milvus-io/milvus/pull/32770">(#32770</a>)</li>
<li>CTraceContextのIDにWrapperとKeepaliveを追加した<a href="https://github.com/milvus-io/milvus/pull/32746">(#32746</a>)</li>
<li>datacoordメタオブジェクトでデータベース名が見つからない問題を修正<a href="https://github.com/milvus-io/milvus/pull/33412">(#33412</a>)</li>
<li>ドロップされたパーティションのドロップされたセグメントを同期するようにした<a href="https://github.com/milvus-io/milvus/pull/33332">(#33332</a>)</li>
<li>不適切なパラメータによるquotaCenterのメトリクス収集の失敗を修正した<a href="https://github.com/milvus-io/milvus/pull/33399">(#33399</a>)</li>
</ul>
<h2 id="v241" class="common-anchor-header">v2.4.1<button data-href="#v241" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日: 2024年5月6日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Java SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.1</td><td>2.4.1</td><td>2.4.0</td><td>2.4.2</td></tr>
</tbody>
</table>
<p>Milvusバージョン2.4.1では、ソフトウェアのパフォーマンス、可観測性、安定性を向上させるために、数多くの改善とバグフィックスが行われました。これらの改善には、宣言的リソースグループAPI、Float16/BFloat16ベクトルデータ型をサポートするバルクインサート機能の強化、オブジェクトストレージのリスト操作を削減する改良されたガベージコレクション（GC）メカニズム、およびパフォーマンスの最適化に関するその他の変更が含まれます。さらに、コンパイルエラー、改行文字でのファジーマッチの失敗、RESTfulインターフェースの不正なパラメータデータ型、動的フィールドが有効な場合にnumpyファイル上でBulkInsertがエラーを発生させるなどのバグ修正も行われました。</p>
<h3 id="Breaking-changes" class="common-anchor-header">変更点</h3><ul>
<li>空のフィルター式での削除のサポートを終了しました。<a href="https://github.com/milvus-io/milvus/pull/32472">(#32472</a>)</li>
</ul>
<h3 id="Features" class="common-anchor-header">機能</h3><ul>
<li>バルクインサートにおいて、Float16/BFloat16ベクトルデータ型をサポートしました<a href="https://github.com/milvus-io/milvus/pull/32157">(#32157</a>)。</li>
<li>スパースフロートベクトルを改良し、ブルートフォースイテレータ検索と範囲検索をサポート<a href="https://github.com/milvus-io/milvus/pull/32635">(#32635</a>)</li>
</ul>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>宣言型リソースグループAPIを追加しました<a href="https://github.com/milvus-io/milvus/pull/31930">(#31930</a>,<a href="https://github.com/milvus-io/milvus/pull/32297">#32297</a>,<a href="https://github.com/milvus-io/milvus/pull/32536">#32536</a>,<a href="https://github.com/milvus-io/milvus/pull/32666">#32666</a>)。</li>
<li>QueryCoordのコレクションオブザーバをタスクドリブンに書き直した<a href="https://github.com/milvus-io/milvus/pull/32441">(#32441</a>)</li>
<li>DataNodeのSyncManagerで使用されるデータ構造をリファクタリングし、メモリ使用量を減らし、エラーを防止しました<a href="https://github.com/milvus-io/milvus/pull/32673">(#32673</a>)。</li>
<li>ガベージコレクションの実装を見直し、オブジェクトストレージに関連するリスト操作を最小限にしました<a href="https://github.com/milvus-io/milvus/pull/31740">(#31740</a>)</li>
<li>コレクション数が多い場合のCPU使用量を削減<a href="https://github.com/milvus-io/milvus/pull/32245">(#32245</a>)</li>
<li>milvus.yamlファイルの関連する設定項目をコードによって自動的に生成することで、 milvus.yamlの管理を強化した<a href="https://github.com/milvus-io/milvus/pull/31832">(#31832</a>,<a href="https://github.com/milvus-io/milvus/pull/32357">#32357</a>)</li>
<li>ローカル削減を行った後にデータを取得することで、Queryのパフォーマンスを向上した<a href="https://github.com/milvus-io/milvus/pull/32346">(#32346</a>)</li>
<li>etcdクライアント作成時にWithBlockオプションを追加した<a href="https://github.com/milvus-io/milvus/pull/32641">(#32641</a>)</li>
<li>クライアントが提供する場合、クライアントが指定するclient_request_idをTraceIDとして使用するようにした<a href="https://github.com/milvus-io/milvus/pull/32264">(#32264</a>)</li>
<li>削除および一括挿入操作のメトリクスにdbラベルを追加した<a href="https://github.com/milvus-io/milvus/pull/32611">(#32611</a>)</li>
<li>AutoIDおよびPartitionKey列の設定による検証をスキップするロジックを追加した<a href="https://github.com/milvus-io/milvus/pull/32592">(#32592</a>)</li>
<li>認証に関するエラーを改善した<a href="https://github.com/milvus-io/milvus/pull/32253">(#32253</a>)</li>
<li>DataCoordのAllocSegmentIDに関するエラーログを整理した<a href="https://github.com/milvus-io/milvus/pull/32351">(#32351</a>,<a href="https://github.com/milvus-io/milvus/pull/32335">#32335</a>)</li>
<li>重複するメトリクスの削除<a href="https://github.com/milvus-io/milvus/pull/32380">(#32380</a>,<a href="https://github.com/milvus-io/milvus/pull/32308">#32308</a>)、および未使用のメトリクスの整理<a href="https://github.com/milvus-io/milvus/pull/32404">(#32404</a>,<a href="https://github.com/milvus-io/milvus/pull/32515">#32515</a>)。</li>
<li>partitionKey機能の有効化を強制するかどうかを制御する設定オプションを追加<a href="https://github.com/milvus-io/milvus/pull/32433">(#32433</a>)</li>
<li>1回のリクエストで挿入できる最大データ量を制御する設定オプションを追加しました<a href="https://github.com/milvus-io/milvus/pull/32433">(#32433</a>)。</li>
<li>セグメントレベルでのapplyDelete操作を並列化し、DelegatorによるDeleteメッセージの処理を高速化した<a href="https://github.com/milvus-io/milvus/pull/32291">(#32291</a>)</li>
<li>インデックス<a href="https://github.com/milvus-io/milvus/pull/32232">(#32232</a>,<a href="https://github.com/milvus-io/milvus/pull/32505">#32505</a>,<a href="https://github.com/milvus-io/milvus/pull/32533">#32533</a>,<a href="https://github.com/milvus-io/milvus/pull/32595">#32595</a>)とキャッシュの追加<a href="https://github.com/milvus-io/milvus/pull/32580">(#32580</a>)により、 QueryCoordで頻繁に行われるフィルタリング処理を高速化した<a href="https://github.com/milvus-io/milvus/pull/32232">(#32232</a>,<a href="https://github.com/milvus-io/milvus/pull/32505">#32505</a>,<a href="https://github.com/milvus-io/milvus/pull/32533">#32533, #</a> <a href="https://github.com/milvus-io/milvus/pull/32595">32595</a>)。</li>
<li>DataCoordの一般的な操作を高速化するために、データ構造を書き直し<a href="https://github.com/milvus-io/milvus/pull/32273">(#32273</a>)、コードをリファクタリング<a href="https://github.com/milvus-io/milvus/pull/32389">(#32389</a>)。</li>
<li>conanからopenblasを削除した<a href="https://github.com/milvus-io/milvus/pull/32002">(#32002</a>)。</li>
</ul>
<h3 id="Bug-fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>rockylinux8におけるmilvusのビルドを修正しました<a href="https://github.com/milvus-io/milvus/pull/32619">(#32619</a>)<a href="https://github.com/milvus-io/milvus/pull/32619">。</a></li>
<li>ARM上でのSVEのコンパイルエラーを修正<a href="https://github.com/milvus-io/milvus/pull/32463">(#32463</a>,<a href="https://github.com/milvus-io/milvus/pull/32270">#32270</a>)。</li>
<li>ARMベースのGPUイメージにおけるクラッシュ問題を修正<a href="https://github.com/milvus-io/milvus/pull/31980">(#31980</a>)</li>
<li>正規表現クエリが改行を含むテキストを扱えない問題を修正<a href="https://github.com/milvus-io/milvus/pull/32569">(#32569</a>)</li>
<li>GetShardLeadersが空のノードリストを返すことにより検索結果が空になる問題を修正<a href="https://github.com/milvus-io/milvus/pull/32685">(#32685</a>)</li>
<li>BulkInsertがnumpyファイルの動的フィールドに遭遇した場合にエラーを発生する問題を修正しました<a href="https://github.com/milvus-io/milvus/pull/32596">(#32596</a>)<a href="https://github.com/milvus-io/milvus/pull/32596">。</a></li>
<li>RESTFulV2インターフェイスに関するバグを修正。リクエストの数値パラメータが文字列型ではなく数値入力を受け付けるようにする重要な修正も含まれる<a href="https://github.com/milvus-io/milvus/pull/32485">(#32485</a>,<a href="https://github.com/milvus-io/milvus/pull/32355">#32355</a>)。</li>
<li>レートリミッターのwatching configイベントを削除したことによる、 プロキシのメモリリークを修正<a href="https://github.com/milvus-io/milvus/pull/32313">(#32313</a>)</li>
<li>パーティション名(partitionName)が指定されていない場合に、レートリミッターがパーティションが見つからないと不正に報告する問題を修正した<a href="https://github.com/milvus-io/milvus/pull/32647">(#32647</a>)</li>
<li>エラータイプにコレクションが回復状態にある場合とロードされていない場合の検出を追加。<a href="https://github.com/milvus-io/milvus/pull/32447">(#32447</a>)</li>
<li>負のクエリ可能なnumエンティティメトリックを修正した<a href="https://github.com/milvus-io/milvus/pull/32361">(#32361</a>)</li>
</ul>
<h2 id="v240" class="common-anchor-header">v2.4.0<button data-href="#v240" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日: 2024年4月17日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th><th>Node.js SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.0</td><td>2.4.0</td><td>2.4.0</td></tr>
</tbody>
</table>
<p>2.4.0-rc.1リリースの強固な基盤の上に、既存の機能を維持しつつ、ユーザーから報告された重大なバグへの対応に重点を置きました。さらに、Milvus 2.4.0では、システム性能の向上、様々なメトリクスの導入による観測性の向上、コードベースの簡素化を目的とした様々な最適化を導入しています。</p>
<h3 id="Improvements" class="common-anchor-header">改良点</h3><ul>
<li>MinIO TLS接続のサポート<a href="https://github.com/milvus-io/milvus/pull/31396">(#31396</a>,<a href="https://github.com/milvus-io/milvus/pull/31618">#31618</a>)</li>
<li>スカラーフィールドのAutoIndex対応<a href="https://github.com/milvus-io/milvus/pull/31593">(#31593</a>)</li>
<li>ハイブリッド検索リファクタリングにより、通常の検索と一貫した実行パスを実現<a href="https://github.com/milvus-io/milvus/pull/31742">(#31742</a> <a href="https://github.com/milvus-io/milvus/pull/32178">、#32178</a>)</li>
<li>bitsetおよびbitset_viewリファクタリングによるフィルタリングの高速化<a href="https://github.com/milvus-io/milvus/pull/31592">(#31592</a>,<a href="https://github.com/milvus-io/milvus/pull/31754">#31754</a>,<a href="https://github.com/milvus-io/milvus/pull/32139">#32139</a>)。</li>
<li>インポートタスクがデータインデックスの完了を待つようになりました<a href="https://github.com/milvus-io/milvus/pull/31733">(#31733</a>)。</li>
<li>インポートの互換性の強化<a href="https://github.com/milvus-io/milvus/pull/32121">(#32121</a>)、タスクのスケジューリング<a href="https://github.com/milvus-io/milvus/pull/31475">(#31475</a>)、インポートファイルのサイズと数の制限<a href="https://github.com/milvus-io/milvus/pull/31542">(#31542)</a></li>
<li>型チェックのインターフェイスの標準化<a href="https://github.com/milvus-io/milvus/pull/31945">(#31945</a>,<a href="https://github.com/milvus-io/milvus/pull/31857">#31857</a>)、非推奨のコードやメトリクスの削除<a href="https://github.com/milvus-io/milvus/pull/32079">(#32079</a>,<a href="https://github.com/milvus-io/milvus/pull/32134">#32134</a>,<a href="https://github.com/milvus-io/milvus/pull/31535">#31535</a>,<a href="https://github.com/milvus-io/milvus/pull/32211">#32211</a>,<a href="https://github.com/milvus-io/milvus/pull/31935">#31935</a>)、定数名の正規化<a href="https://github.com/milvus-io/milvus/pull/31515">(#31515</a>)などのコードの簡素化。</li>
<li>QueryCoordのカレントターゲットチャンネルチェックポイントの遅延に対する新しいメトリクスを追加しました<a href="https://github.com/milvus-io/milvus/pull/31420">(#31420</a>)。</li>
<li>共通メトリクスにdbラベルを追加した<a href="https://github.com/milvus-io/milvus/pull/32024">(#32024</a>)</li>
<li>削除済み、インデックス付き、およびロードされたエンティティのカウントに関する新しいメトリクスに、collectionNameやdbNameなどのラベルが追加されました<a href="https://github.com/milvus-io/milvus/pull/31861">(#31861</a>)。</li>
<li>ベクトル型が不一致の場合のエラー処理を改善しました<a href="https://github.com/milvus-io/milvus/pull/31766">(#31766</a>)<a href="https://github.com/milvus-io/milvus/pull/31766">。</a></li>
<li>インデックスが構築できない場合にクラッシュせずにエラーを投げるようにした<a href="https://github.com/milvus-io/milvus/pull/31845">(#31845</a>)</li>
<li>データベースの削除時にデータベースのメタキャッシュを無効にするようにした<a href="https://github.com/milvus-io/milvus/pull/32092">(#32092</a>)</li>
<li>チャンネル配信<a href="https://github.com/milvus-io/milvus/pull/31814">(#31814</a>)およびリーダービュー管理<a href="https://github.com/milvus-io/milvus/pull/32127">(#32127</a>)のインターフェイスをリファクタリング。</li>
<li>チャンネルディストリビューションマネージャインターフェイスのリファクタリング<a href="https://github.com/milvus-io/milvus/pull/31814">(#31814</a>)とリーダービューマネージャインターフェイスのリファクタリング<a href="https://github.com/milvus-io/milvus/pull/32127">(#32127</a>)</li>
<li>バッチ処理<a href="https://github.com/milvus-io/milvus/pull/31632">(#31632</a>)、マッピング情報の追加<a href="https://github.com/milvus-io/milvus/pull/32234">(#32234</a>,<a href="https://github.com/milvus-io/milvus/pull/32249">#32249</a>)、ロックの使用回避<a href="https://github.com/milvus-io/milvus/pull/31787">(#31787</a>)により、頻繁に呼び出される操作を高速化。</li>
</ul>
<h3 id="Breaking-Changes" class="common-anchor-header">変更点</h3><ul>
<li>バイナリベクトルでのグルーピング検索の廃止<a href="https://github.com/milvus-io/milvus/pull/31735">(#31735</a>)</li>
<li>ハイブリッド検索でのグループ化検索の廃止<a href="https://github.com/milvus-io/milvus/pull/31812">(#31812</a>)</li>
<li>バイナリベクトルにおけるHNSWインデックスの廃止<a href="https://github.com/milvus-io/milvus/pull/31883">(#31883</a>)</li>
</ul>
<h3 id="Bug-Fixes" class="common-anchor-header">バグ修正</h3><ul>
<li>クラッシュ防止のため、クエリと挿入時のデータ型と値のチェックを強化<a href="https://github.com/milvus-io/milvus/pull/31478">(#31478</a> <a href="https://github.com/milvus-io/milvus/pull/31653">、#31653</a> <a href="https://github.com/milvus-io/milvus/pull/31698">、#31698</a> <a href="https://github.com/milvus-io/milvus/pull/31842">、#31842</a> <a href="https://github.com/milvus-io/milvus/pull/32042">、#32042</a> <a href="https://github.com/milvus-io/milvus/pull/32251">、#32251</a> <a href="https://github.com/milvus-io/milvus/pull/32204">、#32204</a>)</li>
<li>RESTful APIのバグ修正<a href="https://github.com/milvus-io/milvus/pull/32160">(#32160</a>)</li>
<li>転置インデックスのリソース使用量の予測を改善した<a href="https://github.com/milvus-io/milvus/pull/31641">(#31641</a>)。</li>
<li>認証が有効な場合のetcdとの接続問題の解決<a href="https://github.com/milvus-io/milvus/pull/31668">(#31668</a>)</li>
<li>natsサーバのセキュリティ更新<a href="https://github.com/milvus-io/milvus/pull/32023">(#32023</a>)</li>
<li>転置インデックスファイルを/tmpではなくQueryNodeのローカルストレージパスに格納するようにした<a href="https://github.com/milvus-io/milvus/pull/32210">(#32210</a>)</li>
<li>collectionInfoにおけるdatacoordのメモリリークに対処<a href="https://github.com/milvus-io/milvus/pull/32243">(#32243</a>)</li>
<li>システムパニックを引き起こす可能性のあるfp16/bf16関連のバグを修正しました<a href="https://github.com/milvus-io/milvus/pull/31677">(#31677</a>,<a href="https://github.com/milvus-io/milvus/pull/31841">#31841</a>,<a href="https://github.com/milvus-io/milvus/pull/32196">#32196</a>)。</li>
<li>グループ化検索が不十分な結果を返す問題を解決<a href="https://github.com/milvus-io/milvus/pull/32151">(#32151</a>)</li>
<li>Reduceステップにおけるオフセットをより効果的に扱い、"reduceStopForBest "が有効な場合に適切な結果が得られるように、イテレータを用いた検索を調整した<a href="https://github.com/milvus-io/milvus/pull/32088">(#32088</a>)</li>
</ul>
<h2 id="v240-rc1" class="common-anchor-header">v2.4.0-rc.1<button data-href="#v240-rc1" class="anchor-icon" translate="no">
      <svg translate="no"
        aria-hidden="true"
        focusable="false"
        height="20"
        version="1.1"
        viewBox="0 0 16 16"
        width="16"
      >
        <path
          fill="#0092E4"
          fill-rule="evenodd"
          d="M4 9h1v1H4c-1.5 0-3-1.69-3-3.5S2.55 3 4 3h4c1.45 0 3 1.69 3 3.5 0 1.41-.91 2.72-2 3.25V8.59c.58-.45 1-1.27 1-2.09C10 5.22 8.98 4 8 4H4c-.98 0-2 1.22-2 2.5S3 9 4 9zm9-3h-1v1h1c1 0 2 1.22 2 2.5S13.98 12 13 12H9c-.98 0-2-1.22-2-2.5 0-.83.42-1.64 1-2.09V6.25c-1.09.53-2 1.84-2 3.25C6 11.31 7.55 13 9 13h4c1.45 0 3-1.69 3-3.5S14.5 6 13 6z"
        ></path>
      </svg>
    </button></h2><p>リリース日：2024年3月20日</p>
<table>
<thead>
<tr><th>Milvusバージョン</th><th>Python SDKバージョン</th></tr>
</thead>
<tbody>
<tr><td>2.4.0-rc.1</td><td>2.4.0</td></tr>
</tbody>
</table>
<p>このリリースでは、いくつかのシナリオベースの機能が導入されています：</p>
<ul>
<li><p><strong>新しいGPUインデックス - CAGRA</strong>: NVIDIAの貢献により、この新しいGPUインデックスは、特にバッチ検索において10倍のパフォーマンス向上を提供します。詳細は<a href="/docs/ja/gpu_index.md">GPUインデックスを</a>ご参照ください。</p></li>
<li><p><strong>マルチベクトルと</strong> <strong>ハイブリッド検索</strong>：この機能により、複数のモデルからのベクトル埋め込みを保存し、ハイブリッド検索を行うことができます。詳細は「<a href="/docs/ja/multi-vector-search.md">ハイブリッド検索</a>」を参照。</p></li>
<li><p><strong>スパース・ベクトル</strong>：キーワードの解釈と分析に最適なスパース・ベクターが、コレクションでの処理に対応しました。詳細については、<a href="/docs/ja/sparse_vector.md">スパース・ベクトルを</a>参照してください。</p></li>
<li><p><strong>グループ化検索</strong>：カテゴリカルな集約は、RAG（Retrieval-Augmented Generation）アプリケーションのドキュメントレベルのリコールを強化します。詳細については、「<a href="https://milvus.io/docs/single-vector-search.md#Grouping-search">グループ化検索</a>」を参照してください。</p></li>
<li><p><strong>転置インデックスと</strong> <strong>ファジィ・マッチング</strong>：これらの機能は、スカラー・フィールドのキーワード検索を向上させます。詳細については、「<a href="/docs/ja/index-scalar-fields.md">スカラー・フィールドのインデックスと</a> <a href="/docs/ja/single-vector-search.md#filtered-search">フィルター検索</a>」を参照してください。</p></li>
</ul>
<h3 id="New-Features" class="common-anchor-header">新機能</h3><h4 id="GPU-Index---CAGRA" class="common-anchor-header">GPUインデックス - CAGRA</h4><p>NVIDIAチームのCAGRAへの貴重な貢献に対し、心より感謝申し上げます。CAGRAは、オンラインで使用できる最先端の（SoTA）GPUベースのグラフインデックスです。</p>
<p>これまでのGPUインデックスとは異なり、CAGRAは従来CPUインデックスが得意としてきた小バッチクエリにおいても圧倒的な優位性を示しています。さらに、GPUインデックスがすでに得意とする大規模バッチクエリとインデックス構築速度におけるCAGRAの性能は、まさに比類ないものです。</p>
<p>サンプルコードは<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/example_gpu_cagra.py">example_gpu_cagra.py</a> にあります。</p>
<h4 id="Sparse-Vector-Beta" class="common-anchor-header">スパースベクトル (ベータ)</h4><p>このリリースでは、スパースベクトルと呼ばれる新しいタイプのベクトル場を導入します。スパースベクトルは密なベクトルとは異なり、ゼロでない次元はほんの一握りで、次元数が数倍高くなります。この特徴は、項ベースの性質により解釈しやすく、特定の領域においてより効果的である。SPLADEv2/BGE-M3のような学習済みのスパースモデルは、一般的な第一段階のランキングタスクに非常に有用であることが証明されている。Milvusのこの新機能の主なユースケースは、SPLADEv2/BGE-M3のようなニューラルモデルやBM25アルゴリズムのような統計モデルによって生成されたスパースベクトルに対する効率的な近似意味的最近傍探索を可能にすることです。Milvusは現在、スパースベクトルの効率的で高性能な格納、インデックス付け、検索（MIPS、最大内積探索）をサポートしています。</p>
<p>サンプルコードは<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/hello_sparse.py">hello_sparse.pyに</a>あります。</p>
<h4 id="Multi-Embedding---Hybrid-Search" class="common-anchor-header">マルチ埋め込みとハイブリッド検索</h4><p>マルチベクタのサポートは、マルチモデルデータ処理や密なベクトルと疎なベクトルの混在を必要とするアプリケーションの基礎となります。マルチベクタサポートにより、以下のことが可能になります：</p>
<ul>
<li>複数のモデルから非構造化テキスト、画像、音声サンプルに対して生成されたベクトル埋め込みを保存。</li>
<li>各エンティティの複数のベクトルを含むANN検索の実行。</li>
<li>異なる埋め込みモデルに重みを割り当てることで、検索ストラテジーをカスタマイズ。</li>
<li>様々な埋め込みモデルを試して、最適なモデルの組み合わせを見つける。</li>
</ul>
<p>マルチ・ベクトル・サポートにより、FLOAT_VECTOR や SPARSE_FLOAT_VECTOR などの異なる型の複数のベクトル・フィールドをコレクションに格納し、インデックスを付け、リランキング戦略を適用することができる。現在、2つのリランキング戦略が利用可能である：<strong>Reciprocal Rank Fusion (RRF)</strong>と<strong>Average Weighted Scoring</strong>である。どちらの戦略も、異なるベクトルフィールドからの検索結果を統一された結果セットに結合する。最初の戦略は、異なるベクトルフィールドの検索結果に一貫して現れるエンティティを優先し、もう一方の戦略は、各ベクトルフィールドの検索結果に重みを割り当てて、最終的な結果セットにおける重要度を決定する。</p>
<p>コード例は<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/hybrid_search.py">hybrid_search.pyに</a>あります。</p>
<h4 id="Inverted-Index-and-Fuzzy-Match" class="common-anchor-header">転置インデックスとファジィマッチ</h4><p>Milvusの以前のリリースでは、スカラーフィールドのインデックス作成にメモリベースのバイナリ検索インデックスとMarisa Trieインデックスが使用されていました。しかし、これらの方法はメモリを大量に消費しました。Milvusの最新リリースでは、すべての数値および文字列データ型に適用可能なTantivyベースの転置インデックスが採用されました。この新しいインデックスはスカラークエリーの性能を劇的に向上させ、文字列中のキーワードのクエリーを10分の1に削減した。さらに、この転置インデックスは、データ圧縮と内部インデックス構造のMMap（Memory-Mapped Storage）メカニズムにおける追加の最適化により、より少ないメモリを消費します。</p>
<p>このリリースでは、接頭辞、接尾辞、接尾辞を使用したスカラーフィルタリングにおけるファジーマッチもサポートしています。</p>
<p>コードの例は<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/inverted_index_example.py">inverted_index_example.py</a>と<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/fuzzy_match.py">fuzzy_match.py</a> にあります。</p>
<h4 id="Grouping-Search" class="common-anchor-header">検索のグループ化</h4><p>特定のスカラーフィールドの値で検索結果を集約できるようになりました。これはRAGアプリケーションがドキュメントレベルのリコールを実装するのに役立ちます。各文書は様々なパッセージに分割されます。各パッセージは1つのベクトル埋め込みによって表現され、1つの文書に属する。散らばったパッセージではなく、最も関連性の高いドキュメントを見つけるために、search()操作にgroup_by_field引数を含めることで、ドキュメントIDによって結果をグループ化することができます。</p>
<p>コード例は<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/example_group_by.py">example_group_by.py</a> にあります。</p>
<h4 id="Float16-and-BFloat--Vector-DataType" class="common-anchor-header">Float16 と BFloat- Vector データ型</h4><p>機械学習やニューラルネットワークでは、Float16やBFloatのような半精度データ型がよく使用されます。これらのデータ型はクエリの効率を改善し、メモリ使用量を削減できますが、精度の低下というトレードオフが伴います。今回のリリースで、Milvusはベクトルフィールドでこれらのデータ型をサポートするようになりました。</p>
<p>サンプルコードは<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/float16_example.py">float16_example.py</a>と<a href="https://github.com/milvus-io/pymilvus/blob/2.4/examples/bfloat16_example.py">bfloat16_example.py</a> にあります。</p>
<h3 id="Upgraded-Architecture" class="common-anchor-header">アップグレードされたアーキテクチャ</h3><h4 id="L0-Segment" class="common-anchor-header">L0 セグメント</h4><p>このリリースには、削除されたデータを記録するために設計された L0 セグメントという新しいセグメントが含まれています。このセグメントでは、保存された削除レコードを定期的にコンパクト化し、封印されたセグメントに分割することで、小さな削除に必要なデータフラッシュの回数を減らし、小さなストレージフットプリントを残します。このメカニズムにより、Milvusはデータ圧縮とデータフラッシュを完全に分離し、削除およびアップサート操作のパフォーマンスを向上させます。</p>
<h4 id="Refactored-BulkInsert" class="common-anchor-header">リファクタリングされた一括挿入</h4><p>本リリースでは、改良された一括挿入ロジックも導入されています。これにより、1回の一括挿入リクエストで複数のファイルをインポートできるようになります。リファクタリングされたバージョンでは、一括挿入のパフォーマンスと安定性の両方が大幅に改善されました。また、レート制限の微調整やユーザーフレンドリーなエラーメッセージなど、ユーザーエクスペリエンスも向上しています。さらに、MilvusのRESTful APIを通じてバルクインサートのエンドポイントに簡単にアクセスすることができます。</p>
<h4 id="Memory-mapped-Storage" class="common-anchor-header">メモリマップストレージ</h4><p>Milvusはメモリマップドストレージ(MMap)を使用してメモリ使用量を最適化しています。このメカニズムでは、ファイルコンテンツを直接メモリにロードする代わりに、ファイルコンテンツをメモリにマッピングします。このアプローチは、パフォーマンスの低下というトレードオフを伴います。  2つのCPUと8GBのRAMを持つホスト上のHNSWインデックス付きコレクションでMMapを有効にすると、10%未満の性能低下で、4倍のデータをロードできます。</p>
<p>さらに、このリリースでは、Milvusを再起動することなく、MMapを動的かつきめ細かく制御することができます。</p>
<p>詳細については、<a href="/docs/ja/mmap.md">MMap Storage</a> を参照してください。</p>
<h3 id="Others" class="common-anchor-header">その他</h3><h4 id="Milvus-CDC" class="common-anchor-header">Milvus-CDC</h4><p>Milvus-CDCは、Milvusインスタンス間で増分データをキャプチャおよび同期するための使いやすいコンパニオンツールであり、増分バックアップおよびディザスタリカバリを容易に行うことができます。本リリースでは、Milvus-CDCの安定性が向上し、変更データキャプチャ(CDC)機能が一般的に利用できるようになりました。</p>
<p>Milvus-CDCの詳細については、<a href="https://github.com/zilliztech/milvus-cdc">GitHubリポジトリ</a>および<a href="/docs/ja/milvus-cdc-overview.md">Milvus-CDC Overviewを</a>ご参照ください。</p>
<h4 id="Refined-MilvusClient-Interfaces" class="common-anchor-header">MilvusClientインターフェースの改良</h4><p>MilvusClientはORMモジュールに代わる使いやすいクライアントです。サーバとのインタラクションを単純化するために、純粋に機能的なアプローチを採用しています。コネクションプールを維持する代わりに、各MilvusClientはサーバとのgRPC接続を確立します。 MilvusClientモジュールはORMモジュールのほとんどの機能を実装しています。 MilvusClientモジュールの詳細については、<a href="https://github.com/milvus-io/pymilvus">pymilvus</a>および<a href="/api-reference/pymilvus/v2.4.x/About.md">リファレンスドキュメントを</a>参照してください。</p>
