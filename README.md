# npm install

```zsh
npm install --save-dev typescript ts-loader webpack webpack-cli webpack-dev-server
```

# 各パッケージの役割 (TypeScript Webpack)

|    パッケージ名    | 役割                                                          |
| :----------------: | :------------------------------------------------------------ |
|     typescript     | コンパイラ                                                    |
|     ts-loader      | Webpack と連動して TypeScript コンパイラを起動                |
|      webpack       | 複数のファイルを１つにまとめる                                |
|    webpack-cli     | コマンドラインで Webpack を使う                               |
| webpack-dev-server | Webpack のビルド<br>開発用 Web サーバの起動<br>ホットリロード |

# tsconfig の基本的な設定項目

| 設定項目名                       |   初期値   |                       意味                        |
| :------------------------------- | :--------: | :-----------------------------------------------: |
| target                           |   "es5"    |      コンパイル後の Javascript のバージョン       |
| module                           | "commonjs" |     どの方式でモジュール関連のコードを扱うか      |
| strict                           |    true    | TypeScript の基本的なチェックを全て true にするか |
| esModuleInterop                  |    true    |      import 文を使って読み込めるようにするか      |
| forceConsistentCasingInFileNames |    true    |           ファイル名の大小を区別するか            |
| allowJs                          |    true    |          JavaScript ファイルを許容するか          |
| jsx                              | "preserve" |        JSX ファイルをどうコンパイルするか         |
| lib                              |     []     |              使用する JS ライブラリ               |
| outDir                           |    "./"    |                ビルド結果の出力先                 |
| baseUrl                          |    "./"    |     import 文のベースパス (絶対パスを使える)      |

# 各パッケージの役割 (ESLint Pretter)

|           パッケージ名           | 役割                                                                       |
| :------------------------------: | :------------------------------------------------------------------------- |
|              eslint              | JavaScript のための静的検証ツール                                          |
|             prettier             | コードフォーマッター                                                       |
|      eslint-config-prettier      | ESLint と Prettier を併用する際に                                          |
| @typescript-eslint/eslint-plugin | ESLint で TypeScript のチェックを行うプラグイン                            |
|    @typescript-eslint/parser     | ESLint で TypeScript を解析できるようにする                                |
|              husky               | Git コマンドをフックに別のコマンドを呼び出せる                             |
|           lint-staged            | commit したファイル (staging にあるファイル)に lint を実行することができる |
