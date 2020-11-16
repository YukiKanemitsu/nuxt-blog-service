# STORE

**This directory is not required, you can delete it if you don't want to use it.**

This directory contains your Vuex Store files.
Vuex Store option is implemented in the Nuxt.js framework.

Creating a file in this directory automatically activates the option in the framework.

More information about the usage of this directory in [the documentation](https://nuxtjs.org/guide/vuex-store).


# MEMO:

- payload
    ```ミューテーションはVuexのストアの状態を変更したいときに使うもので、分かりやすくいうとハンドラに近いものです。使い方と特徴がいくつかあるので以下にまとめます。```

    - ミューテーションはタイプとハンドラを持っています
    - ハンドラみたいなものなので直接使うことができません（公式ではハンドラに近い概念といっています）
    - タイプを指定してコミットすることでハンドラを使えます
    - ミューテーションのハンドラは第一引数にstateを渡して実際にstateの変更を行います
    - ミューテーションのハンドラは第二引数に追加の引数（`payload`といいます）を渡すこともできます※payloadはオブジェクトで渡します
    - コンポーネント側でタイプを指定してコミットします
    - 上に書いた第一引数と第二引数を無視して、第一引数にtypeプロパティを持つオブジェクトを渡してコミットすることもできます
    - ミューテーションハンドラでは非同期処理ができない


- dispatch


- スプレッド構文
    `...foo`の形で記述され、配列やオブジェクトの要素を文字通り展開する構文。
    `Array.prototype.concat()`相当のことが簡潔にかけます。

- シャローコピーとディープコピーについて
    https://top-men.hatenablog.com/entry/2018/10/03/213627

    スプレッド演算子はシャローコピー
    オブジェクト展開辞にディープコピーする方法は
    `JSON.stringify`と`JSON.parse`を使う方法
    があるが、undefinedや関数が定義されていると、プロパティがなくなってしまう。
    そう言ったケースでは、lodashと言うライブラリを使う。
    ES6のObject.assignはシャローコピー。


- preventDefault()
    https://qiita.com/tochiji/items/4e9e64cabc0a1cd7a1ae

- vuex
    https://reffect.co.jp/vue/understaind-vue-basic#Vuex
    https://qiita.com/nasum/items/d17c0a628e6c32616b85

- storeとform
    https://vuex.vuejs.org/ja/guide/forms.html
    https://qiita.com/sryuji/items/3d5f0136fb09ca32c7ad

- ライフサイクル
    https://vuex.vuejs.org/ja/guide/actions.html
    https://qiita.com/chan_kaku/items/7f3233053b0e209ef355