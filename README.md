# Autarkia - 分散型サブスクリプション管理システム

## 概要
Autarkiaは、Web3技術を活用したNFTベースのサブスクリプション管理プラットフォーム。  
クリエイターは独自のNFTサブスクプランを提供し、ユーザーはNFTを所有することで限定コンテンツへのアクセス権を得る。  
従来の中央集権型サービス（Netflix、Patreonなど）と異なり、支払い・認証・コンテンツ配信を分散型の仕組みで管理し、  
クリエイターへ100%の収益を直接還元する。

## 特徴
- **NFTサブスク**: クリエイターが発行するNFTを購入することで、限定コンテンツへのアクセス権を取得。
- **分散型決済**: スマートコントラクトを活用し、定期的な支払いを自動化。
- **コンテンツ保護**: IPFS / Filecoinを利用した分散ストレージにより、中央管理なしで安全にデータを保存。
- **ウォレット認証**: Web3ウォレット（MetaMask、WalletConnectなど）を通じたシームレスなログイン。
- **コミュニティガバナンス**: NFT所有者による投票機能で、コンテンツの方向性を決定。

## 技術スタック
- **フロントエンド**: Next.js, TypeScript, TailwindCSS, Wagmi
- **バックエンド**: Spring Boot, Web3j, PostgreSQL, Redis
- **ブロックチェーン**: Solidity, Hardhat, Ethereum/Polygon
- **ストレージ**: IPFS, Filecoin
- **認証**: JWT, OAuth2, Web3ウォレット

## インストール & セットアップ
```bash
git clone https://github.com/your-repo/autarkia.git
cd autarkia
npm install
npm run dev
```

## ライセンス
このプロジェクトはMITライセンスのもとで提供されます。

## ディレクトリ構成
```
/autarkia
├── /frontend          # フロントエンド（Next.js）
│   ├── /components   # 再利用可能なUIコンポーネント
│   ├── /pages        # Next.jsのルーティング（ページごとのディレクトリ）
│   │   ├── index.tsx        # トップページ
│   │   ├── dashboard.tsx    # ユーザーダッシュボード
│   │   ├── content.tsx      # サブスクコンテンツページ
│   │   ├── creator.tsx      # クリエイター向けページ
│   │   ├── login.tsx        # ウォレット接続ページ
│   ├── /styles       # TailwindCSSのカスタムスタイル
│   ├── /utils        # ウォレット認証・NFT取得のユーティリティ関数
│   ├── /hooks        # カスタムReact Hooks（ウォレット接続など）
│   ├── /context      # グローバル状態管理（React Context API）
│   ├── package.json  # 依存関係
│   ├── tsconfig.json # TypeScript設定
│   ├── next.config.js # Next.js設定
│   └── README.md     # フロントエンドのドキュメント
│
├── /backend          # バックエンド（Spring Boot）
│   ├── /src/main/java/com/autarkia  # Javaソースコード
│   ├── /src/main/resources          # 設定ファイル
│   ├── application.yml              # Spring Boot設定
│   ├── Dockerfile                   # Dockerコンテナ設定
│   ├── build.gradle                 # Gradleビルド設定
│   └── README.md                     # バックエンドのドキュメント
│
├── /contracts        # スマートコントラクト（Solidity）
│   ├── /src         # Solidityスマートコントラクト
│   ├── /scripts     # Hardhatデプロイスクリプト
│   ├── hardhat.config.js  # Hardhat設定
│   ├── package.json       # 依存関係
│   └── README.md          # コントラクトのドキュメント
│
├── /docs             # プロジェクトドキュメント
│   ├── architecture.md  # システム設計資料
│   ├── api.md          # API仕様
│   ├── smart-contract.md  # スマートコントラクト仕様
│   └── README.md       # ドキュメント全体の説明
│
└── README.md         # プロジェクト全体のREADME
```
