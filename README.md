# خطوات النشر على Vercel
1. Discord Developer Portal → New Application → OAuth2: انسخ Client ID و Client Secret.
   أضف Redirect: https://YOUR-SITE.vercel.app/api/callback
2. ارفع المجلد على GitHub، ثم Vercel → Import Project.
3. Vercel → Storage/Marketplace → أضف Upstash Redis واربطه بالمشروع.
4. Settings → Environment Variables:
   DISCORD_CLIENT_ID, DISCORD_CLIENT_SECRET,
   SESSION_SECRET (نص عشوائي طويل),
   SITE_URL = https://YOUR-SITE.vercel.app  (بدون / في الآخر),
   ADMIN_IDS = 1510646428559610068,1465120916794249287
5. Redeploy.
