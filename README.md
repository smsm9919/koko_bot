
# Balanced Pack (Render)
- 10x leverage + 60% capital per trade (enforced at runtime).
- Balanced entries + strong anti-reverse protections.
- Verbose logs: indicators snapshot, reasons, trade details, cumulative PnL.
- Keep-alive ping every 60s.

**Start command**
```
gunicorn -w 1 -b 0.0.0.0:$PORT runner:app
```
**Env vars**
- `BOT_MODULE` (اسم ملف البوت بدون .py) — مثال: `bot`
- `BINGX_API_KEY`, `BINGX_API_SECRET` (+ `PUBLIC_URL` اختياري)
