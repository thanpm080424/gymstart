# GymStart – Hướng Dẫn Deploy

## Cấu trúc project
```
gym-website/
├── index.html      ← Trang chính (AEO Schema, Semantic HTML)
├── style.css       ← Toàn bộ CSS
├── main.js         ← JavaScript
├── robots.txt      ← Cho phép AI crawlers
├── sitemap.xml     ← SEO sitemap
└── README.md       ← File này
```

## Deploy lên GitHub Pages (Miễn phí)

1. Tạo tài khoản GitHub tại https://github.com
2. Tạo repository mới, đặt tên (ví dụ: `gymstart`)
3. Upload toàn bộ file lên repository
4. Vào Settings → Pages → Source: `main` branch → `/root`
5. Đợi 2-3 phút → website live tại: `https://username.github.io/gymstart`

## Deploy lên Vercel (Nhanh hơn)

1. Tạo tài khoản tại https://vercel.com
2. Nhấn "New Project" → Import từ GitHub
3. Deploy tự động → nhận domain `.vercel.app`

## Sau khi deploy

1. Thay `https://your-website-url.com` bằng URL thật trong:
   - index.html (thẻ canonical + og:url + schema url)
   - sitemap.xml (tất cả thẻ <loc>)
   - robots.txt (dòng Sitemap:)

2. Kiểm tra AEO/AIEO:
   - Schema: https://validator.schema.org
   - Speed: https://pagespeed.web.dev
   - Console: https://search.google.com/search-console

## Kỹ thuật AEO/AIEO đã áp dụng

✅ FAQPage Schema Markup (JSON-LD)
✅ WebSite Schema Markup
✅ Semantic HTML5 (header, main, section, article, footer)
✅ Heading chuẩn phân cấp H1 → H2 → H3
✅ Meta description, canonical, OG tags
✅ robots.txt cho phép GPTBot, ClaudeBot, PerplexityBot
✅ Sitemap XML
✅ Nội dung FAQ trả lời ngắn gọn, rõ ràng
✅ Internal link giữa các section
