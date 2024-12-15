## 環境構築手順

### 1, node.js プロジェクトを初期化

```bash
mkdir ts_script
cd ts_script
npm init -y
```

### 2, TypeScript と ts-node をインストール

```bash
npm install typescript ts-node @types/node --save-dev
```

[\[typescript\]](https://www.npmjs.com/package/typescript)
[\[ts-node\]](https://www.npmjs.com/package/ts-node)
[\[@types/node\]](https://www.npmjs.com/package/@types/node)

### 3, Typescript 設定ファイルを作成

```bash
npx tsc --init
```

tsconfig.json に設定を追加

```json
{
  "compilerOptions": {
    "target": "ES2020", // 出力されるJavaScriptのバージョン
    "module": "CommonJS", // モジュールの形式
    "strict": true, // 厳格な型チェック
    "esModuleInterop": true, // ESモジュールとの互換性を有効化
    "skipLibCheck": true // ライブラリ型定義のチェックをスキップ
  }
}
```

## ファイルを実行

```bash
npx ts-node ファイル名
```
