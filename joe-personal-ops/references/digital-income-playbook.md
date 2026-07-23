# Digital Income Playbook — เป้า 50,000+ บาท/เดือน

โครงสร้างรายได้ 3 ชั้น: **Etsy (สินค้า) → Gumroad (ความรู้) → Affiliate (ต่อยอด traffic)**
กติกาเหล็ก: ชั้นถัดไปเปิดได้ต่อเมื่อชั้นก่อนหน้า live แล้ว — ห้ามกระโดดไป affiliate ก่อน listing ขึ้น

---

## ชั้น 1 — Etsy: Goldeneraprintsart (Art Deco Printable Art)

**สถานะ:** shop เปิดแล้ว, 0 listings, 18 Midjourney prompt formulas (6 หมวด) พร้อม, TASKS.md sprint 14 วันวางแล้ว

**Sprint หลัก (ทำตามลำดับ ไม่สลับ):**
1. **วันที่ 1–3:** generate + คัดภาพจาก 18 formulas → ได้อย่างน้อย 10 design แรก (1 design = หลายขนาด ratio: 2:3, 3:4, 4:5, ISO, 11x14)
2. **วันที่ 4–6:** เตรียมไฟล์ (n8n ช่วย resize อัตโนมัติได้), mockup, เขียน title/tags/description — ผ่าน `humanize-content` preset Etsy ทุกตัว
3. **วันที่ 7–10:** ขึ้น listing จริง 10 ตัวแรก (งาน manual — Etsy ไม่มีทางลัด) เป้าขั้นต่ำ 2 listings/วัน
4. **วันที่ 11–14:** Pinterest auto-posting ผ่าน n8n + เก็บ baseline metric

**Listing quality bar ขั้นต่ำ:** 13 tags เต็ม, title มี keyword หน้า 40 ตัวอักษรแรก, 6+ ภาพ (mockup ห้องจริงอย่างน้อย 3), ระบุขนาดไฟล์ครบใน description, ราคา launch $4–6 แล้วค่อยขยับ

**KPI ladder:**
| Milestone | เป้า | ความหมาย |
|-----------|------|-----------|
| Listings live | 10 → 25 → 50 | 50 = จุดที่ Etsy search เริ่มเห็นร้าน |
| ยอดขายแรก | ภายใน 30 วันหลัง 10 listings | ถ้าไม่มา → รื้อ SEO ก่อนเพิ่ม listing |
| รายเดือน | $50 → $200 → $500 → $1,400 (≈50K บาทเมื่อรวมทุกชั้น) | |

---

## ชั้น 2 — Gumroad: "Art Deco Etsy Seller Masterkit" ($19)

**สถานะ:** product page draft แล้ว — เงื่อนไข launch: Etsy มีอย่างน้อย 10 listings live ก่อน (ขายวิธีทำต้องมีของจริงให้ดู)
- Masterkit = prompt formulas + workflow + template ที่ Joe ใช้จริง — อัปเดตจากประสบการณ์ sprint ชั้น 1 ก่อนปล่อย
- Copy ทั้งหมดผ่าน `humanize-content` preset Gumroad
- Cross-promote: ท้าย listing Etsy ไม่ใส่ลิงก์ (ผิด TOS) แต่ใช้ TikTok/Pinterest bio เป็นสะพาน
- เป้า: 5–10 ชิ้น/เดือน = $95–190

## ชั้น 3 — Affiliate (เปิดหลัง Etsy+Gumroad live)

ลำดับสมัครตามที่ vet ไว้:
1. **eRank** — 30% recurring 12 เดือน (เนื้อหาผูกกับ workflow Etsy ที่ Joe ใช้จริง → น่าเชื่อ)
2. **Creative Fabrica** — 25%/order หรือ 20% recurring, cookie 90 วัน
3. **Kittl** — 20% recurring 12 เดือน

รูปแบบ content: "เครื่องมือที่ผมใช้เปิดร้าน Etsy จากศูนย์" — TikTok faceless + บทความ ใช้ trilingual advantage (จีน: Xiaohongshu ตลาดแยก)

---

## n8n Automation Scope (ตามที่ map ไว้)

| งาน | Automate ได้ | หมายเหตุ |
|-----|---------------|----------|
| Resize ภาพหลาย ratio | ✅ | ทำก่อน — คืนเวลาเยอะสุด |
| SEO tags ผ่าน API | ✅ | generate draft ให้ Joe คัด |
| Pinterest auto-post | ✅ | ตั้ง schedule รายวัน |
| ขึ้น Etsy listing | ❌ manual | บล็อกเวลาเช้า 30 นาที/วันช่วง sprint |

VPS: Contabo (vmi3205475) — n8n + OpenClaw รันอยู่แล้ว, alert เข้า Telegram

## Monthly Money Check (ทุกสิ้นเดือน)

รายได้จริง Etsy + Gumroad + Affiliate (บาท) vs เป้า 50K → ถ้า 3 เดือนติดต่ำกว่า 20% ของเป้า ให้ทบทวนกลยุทธ์ทั้งระบบ ไม่ใช่เพิ่มความขยันอย่างเดียว
