# Instagram Otomatik Paylaşım

Instagram'da otomatik paylaşım yapabilen modern web uygulaması.

## 🚀 Deployment Seçenekleri

### 1. Vercel (Önerilen - Ücretsiz)

1. [Vercel](https://vercel.com)'e gidin ve GitHub hesabınızla giriş yapın
2. "New Project" butonuna tıklayın
3. Bu repository'yi seçin
4. Otomatik olarak deploy edilecektir

```bash
# Vercel CLI ile
npm i -g vercel
vercel
```

### 2. Netlify

1. [Netlify](https://netlify.com)'e gidin
2. "New site from Git" seçin
3. Repository'yi bağlayın
4. Build command: `npm run build`
5. Publish directory: `.next`

### 3. Kendi Sunucunuzda (VPS/Dedicated)

#### PM2 ile:
```bash
# Sunucuda
npm install -g pm2
npm run build
pm2 start ecosystem.config.js
pm2 startup
pm2 save
```

#### Docker ile:
```bash
# Docker Compose
docker-compose up -d

# Sadece Docker
docker build -t instagram-app .
docker run -p 3000:3000 instagram-app
```

#### Manuel:
```bash
npm run build
npm start
```

## 🔧 Gereksinimler

- Node.js 18+
- npm veya yarn

## 📦 Kurulum

```bash
npm install
npm run dev
```

## 🌐 Production

```bash
npm run build
npm start
```

## 📝 Özellikler

- 📸 Instagram'a otomatik paylaşım
- 📅 Zamanlanmış paylaşımlar
- 🏷️ Hashtag önerileri
- 🔄 Proxy desteği
- 📱 Responsive tasarım
- ⚡ Modern UI/UX

## 🔒 Güvenlik

- Instagram API güvenliği
- Proxy rotasyonu
- Rate limiting
- Error handling

## 📞 Destek

Herhangi bir sorun için issue açabilirsiniz.
