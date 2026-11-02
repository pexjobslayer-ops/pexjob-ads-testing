# Pex JobSlayer — Ads Skills for Claude

ชุดสกิลสำหรับ Claude ช่วยวิเคราะห์ ทดสอบ และสเกลโฆษณา Meta (Facebook/Instagram)

| สกิล | ใช้ทำอะไร |
|---|---|
| [`meta-ads-testing-ai/`](meta-ads-testing-ai/SKILL.md) | **META ADS TESTING AI V3.0** — ระบบ Media Buyer อัตโนมัติ: ดึงข้อมูล → วิเคราะห์ → วินิจฉัย → ปรับปรุง → สเกล → รายงานรายวัน 09:00 น. |
| [`meta-ads-testing-autoscale/`](meta-ads-testing-autoscale/SKILL.md) | วิเคราะห์ผล วางแผนทดสอบ และแนะนำการสเกล Meta Ads |
| [`SKILL.md`](SKILL.md) (root) | Pex JobSlayer Ads Testing — A/B Testing แบบ 1-1-3 สำหรับ Facebook/Instagram และ TikTok |

## วิธีติดตั้งใน Claude (claude.ai / แอป Claude)

1. กดปุ่ม **Code → Download ZIP** ที่หน้านี้ แล้วแตกไฟล์
2. เลือกโฟลเดอร์สกิลที่ต้องการ (เช่น `meta-ads-testing-ai`) แล้วบีบอัดโฟลเดอร์นั้นเป็น ZIP
   (ใน ZIP ต้องมีโฟลเดอร์สกิล และข้างในมี `SKILL.md`)
3. ใน Claude ไปที่เมนู **Skills** → **Upload skill** → เลือกไฟล์ ZIP
4. เปิดสวิตช์สกิล แล้วลองพิมพ์ เช่น "วิเคราะห์แอดเมื่อวาน"

## วิธีติดตั้งใน Claude Code

```bash
git clone https://github.com/pexjobslayer-ops/pexjob-ads-testing
cp -r pexjob-ads-testing/meta-ads-testing-ai ~/.claude/skills/
```

## สิ่งที่ต้องมีก่อนใช้

- เชื่อมต่อ **Meta Ads** connector ใน Claude (เพื่อดึงข้อมูลบัญชีโฆษณาจริง)
- (ไม่บังคับ) เชื่อม **Gmail** หากต้องการรับรายงานทางอีเมล
- ครั้งแรกสกิลจะถามชื่อสินค้า ราคาขาย และต้นทุนสินค้า

## หมายเหตุ

- สกิลใช้ข้อมูลจริงจากบัญชีเท่านั้น ไม่แต่งตัวเลข ไม่คาดเดาออเดอร์
- สกิลจะ **ไม่ปิดแอดหรือเปลี่ยนงบจริงโดยไม่ได้รับอนุญาต**
- คำแนะนำเป็นแนวทางเพื่อประกอบการตัดสินใจ ไม่รับประกันผลลัพธ์ทางธุรกิจ
