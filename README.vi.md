# CSM Beyond Features

[English](./README.md) | **Tiếng Việt**

> Một **mentor Customer Success Management (CSM)** thân thiện, chạy được trên Claude, Poe, ChatGPT hay Claude Code — đóng gói dưới dạng prompt di động, tái dùng ở đâu cũng được.

![type](https://img.shields.io/badge/type-prompt%20%2B%20skill-blue)
![use](https://img.shields.io/badge/works%20on-Claude%20%7C%20Poe%20%7C%20GPT%20%7C%20Claude%20Code-7C3AED)
![license](https://img.shields.io/badge/license-CC%20BY%204.0-yellow)

## Demo

https://github.com/user-attachments/assets/c099d8de-809a-40cc-90c5-b497ff95fa85

## Đây là gì

**CSM Beyond Features** là một persona mentor cho người học **Customer Success** — từ người mới hoàn toàn đến người đang cân nhắc theo nghề CSM. Thay vì đổ định nghĩa ra ngay, nó **hỏi 1–2 câu trước** để nắm level và mục tiêu của bạn, rồi giải thích đúng độ sâu kèm ví dụ thực tế.

Bao phủ: kiến thức nền CSM, vòng đời khách hàng, các metric (NRR, GRR, churn, health score, NPS…), quy trình (QBR/EBR, stakeholder mapping, playbook), các CS platform, và lộ trình nghề CSM.

Repo này **chỉ là phần instruction** (một system prompt) kèm một skill Claude dùng ngay — không có app phải cài, không thu thập dữ liệu. Bạn mang nó sang công cụ AI nào tùy thích.

## Nội dung repo

| File | Là gì |
|------|-------|
| [`SYSTEM_PROMPT.md`](./SYSTEM_PROMPT.md) | Instruction bản **tiếng Anh** — copy-paste vào bất kỳ công cụ AI nào |
| [`SYSTEM_PROMPT.vi.md`](./SYSTEM_PROMPT.vi.md) | Instruction gốc bản **tiếng Việt** |
| [`skill/csm-beyond-features/SKILL.md`](./skill/csm-beyond-features/SKILL.md) | Cùng persona, đóng gói thành **skill Claude Code / Claude Desktop** |
| [`examples/sample-conversations.md`](./examples/sample-conversations.md) | Hội thoại mẫu minh hoạ cách bot hành xử |

## Cách dùng

Chọn nền tảng bạn đang xài. Mọi cách dưới đây đều dùng nội dung file [`SYSTEM_PROMPT.md`](./SYSTEM_PROMPT.md) (hoặc `SYSTEM_PROMPT.vi.md` nếu bạn thích bản Việt).

### Cách 1 — Claude Project
1. Vào [claude.ai](https://claude.ai) → **Projects** → tạo project.
2. Mở **Set project instructions** (custom instructions).
3. Dán nội dung `SYSTEM_PROMPT.md` → lưu.
4. Chat ngay trong project đó.

### Cách 2 — Poe bot
1. Trên [Poe](https://poe.com) → **Create bot**.
2. Dán `SYSTEM_PROMPT.md` vào ô **prompt / instructions**.
3. Chọn base model, lưu, và (tuỳ chọn) để public để chia sẻ link.

### Cách 3 — Custom GPT (ChatGPT)
1. Trong ChatGPT → **Explore GPTs** → **Create**.
2. Ở **Configure → Instructions**, dán `SYSTEM_PROMPT.md`.
3. Lưu; chia sẻ link nếu muốn.

### Cách 4 — Skill Claude Code / Claude Desktop
```bash
# clone rồi copy skill vào thư mục skills của bạn
git clone https://github.com/nixthinh-bit/csm-beyond-features.git
mkdir -p ~/.claude/skills
cp -r csm-beyond-features/skill/csm-beyond-features ~/.claude/skills/
# restart Claude Code / Desktop, rồi cứ hỏi về Customer Success
```
Skill tự kích hoạt — Claude sẽ tự dùng khi bạn hỏi các chủ đề CSM.

> 🌐 **Song ngữ sẵn:** persona luôn trả lời theo ngôn ngữ của người dùng (Việt hoặc Anh), bất kể bạn nạp file prompt bản nào.

## Đóng góp

Hoan nghênh ý tưởng, ví dụ hay hơn, và bản dịch.
1. Mở [issue](https://github.com/nixthinh-bit/csm-beyond-features/issues) hoặc fork → PR.
2. Giữ nguyên cốt lõi persona (hỏi-trước, dạy-không-trích, cấu trúc súc tích).
3. Đừng thêm tên công ty, dữ liệu khách hàng, hay bất cứ gì không công khai.

## License

[CC BY 4.0](./LICENSE) © 2026 nixthinh-bit — dùng và chỉnh sửa tự do, kể cả mục đích thương mại, **nhưng phải ghi công** (vd *"Based on 'CSM Beyond Features' by nixthinh-bit"*). Không phải lời khuyên nghề nghiệp chính thức.
