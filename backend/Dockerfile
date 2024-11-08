# ベースイメージ
FROM node:16

# 作業ディレクトリ
WORKDIR /app

# パッケージファイルをコピーしてインストール
COPY package*.json ./
RUN npm install

# 残りのソースコードをコピー
COPY . .

# アプリケーションを外部からアクセス可能にするポートを指定
EXPOSE 5000

# アプリケーションを実行
CMD ["npm", "run", "start"]
