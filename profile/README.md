![Fortress of the Fallen](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/FotF.png)

## Overview
**Fortress of the Fallen** là một game **Online Action RPG** kết hợp yếu tố **Xây dựng** – **Nhập vai** – **Gacha**. Người chơi sẽ tồn tại trong một thế giới nổi trên không gian, nơi các hòn đảo vệ tinh bay xung quanh một Tinh Hà Trung Tâm.

Người chơi bắt đầu chỉ với một hòn đảo trống rỗng – như ngôi nhà riêng. Qua thời gian, họ sẽ:

- Xây dựng & quản lý đảo (quán ăn, nông trại, lò rèn, thư viện…).

- Tuyển dụng nhân vật thông qua cơ chế gacha tuyển dụng, yêu cầu tài nguyên để trả lương / duy trì.

- Thám hiểm Tinh Hà Trung Tâm: Leo 100 tầng tháp trên trời hoặc khám phá 18 tầng ngục dưới lòng đất.

- Sinh tử vĩnh hằng: Khi chết, số phận sẽ dựa vào Karma để quyết định bị đẩy xuống tầng ngục nào. Muốn hồi sinh, người chơi phải vượt qua thử thách trong ngục.
---

## Core Game Loop
- Xây dựng đảo cá nhân → Thu thập & tiêu hao tài nguyên để phát triển.

- Tuyển dụng đồng minh (qua gacha) → NPC / Anh hùng giúp vận hành module trên đảo.

- Leo tháp / Xuống ngục → Chiến đấu, loot tài nguyên, mở khóa kỹ năng & trang bị.

- Quản lý sinh tồn → Nếu chết, dựa vào Karma để xác định tầng ngục bị đẩy xuống.

- Vượt thử thách ngục → Thành công = hồi sinh. Thất bại = giảm chỉ số.

## Game Modes

| Chế độ        | Đặc điểm |
|---------------|----------|
| **Khám phá Tháp**  | Leo 100 tầng, mỗi tầng tăng độ khó, mở khóa boss và kho báu. |
| **Vượt ngục**  | Hình phạt khi để nhân vật chết. Vượt qua sẽ được hồi sinh. |
| **Xây dựng Đảo**  | Cá nhân hóa đảo vệ tinh của mình: công trình, NPC, phong cảnh. |
|**PVP Arena** | Đấu trường, người chơi có thể giao đấu ở khu vực này.|

---

## Game Play
- Action RPG Online: Chiến đấu hack-n-slash, tổ đội 1–4 người hoặc chơi solo.

- Đảo cá nhân hóa:

    - Khởi đầu: đảo trống chỉ có bạn.

    - Muốn vận hành nông trại, quán ăn, lò rèn, thư viện, học viện… → cần NPC.

    - NPC được tuyển qua gacha (Hero Recruit System).

- Hệ thống tử vong độc đáo:

    - Người chơi chết không "respawn ngay".

    - Dựa vào Karma → xác định tầng ngục bị đẩy xuống.

    - Muốn hồi sinh → phải vượt qua thử thách trong ngục.

- Gacha System:

    - Tuyển NPC (vận hành đảo).

    - Tuyển Hero (đồng minh chiến đấu).

    - Tỷ lệ hiếm phụ thuộc vào Luck và Influence.

## Character System
![Character System](https://github.com/fortress-of-the-fallen/FotF-GDD/blob/main/assets/stats-system.png)

- Level tối đa: **100**
- Hệ thống **chỉ số cơ bản và đặc biệt quyết định class**, không tăng cấp theo level.
- Trang bị có thể **tăng chỉ số để mở class mới** hoặc **kích hoạt kỹ năng độc quyền**.
- Các nhân vật **triệu hồi** cũng có class, skill riêng và tiến hóa riêng.

### A. Base Attributes (Chỉ số cơ bản)

| Attribute | Mô tả |
|----------|-------|
| STR (Strength)     | Sức mạnh cơ bắp, sát thương vật lý |
| DEX (Dexterity)    | Nhanh nhẹn, chính xác, tốc độ đánh |
| CON (Constitution) | Thể lực, máu, kháng sát thương |
| INT (Intelligence) | Trí tuệ, phép thuật, kháng phép |
| WIS (Wisdom)       | Niềm tin, khả năng sử dụng kỹ năng đặc biệt |
| CHA (Charisma)     | Mở khóa các kỹ năng đặc biệt |

### B. Derived Stats (Chỉ số phụ thuộc)

| **Stat**        | **Phụ thuộc vào**         | **Ý nghĩa**                            |
|----------------|---------------------------|----------------------------------------|
| HP             | CON, STR                  | Máu tối đa                              |
| MP             | WIS, INT                  | Mana tối đa                             |
| PATK / DATK    | STR, DEX, CON             | Tấn công / phòng thủ vật lý              |
| MATK / MDEF    | INT, WIS                  | Tấn công phép / kháng phép             |
| SPD            | DEX                       | Tốc độ hành động / đánh                |
| CRIT           | DEX                       | Tỷ lệ chí mạng                          |
| ACC            | DEX, INT                  | Độ chính xác khi tấn công              |
| EVA            | DEX, CON                  | Né tránh đòn đánh                      |

### C. Special Traits (Thuộc tính đặc biệt)

| Trait       | Mô tả |
|-------------|-------|
| Karma       | Đạo đức nhân vật (tốt, ác, trung lập) ảnh hưởng đến kỹ năng, mối quan hệ |
| Affinity    | Mối liên kết với phe phái / nguyên tố / NPC |
| Luck        | Tác động đến tỷ lệ rơi đồ, chí mạng, sự kiện ngẫu nhiên |
| Resistance  | Khả năng chống lại hiệu ứng bất lợi (poison, stun, curse...) |

---

## Race & Stat Cap System (Chủng tộc và giới hạn chỉ số)

Mỗi **chủng tộc** sẽ có:
- **Giới hạn chỉ số khác nhau**
- **Kháng / yếu với các nguyên tố**
- **Thế mạnh riêng biệt** trong lối chơi

### Ví dụ

| Race        | STR | DEX | CON | INT | WIS | CHA | Ghi chú |
|-------------|-----|-----|-----|-----|-----|-----|--------|
| Human       | 8   | 8   | 8   | 8   | 8   | 8   | Cân bằng |
| Elf         | 6   | 10  | 6   | 10  | 10  | 8   | Giỏi phép, tốc độ cao |
| Orc         | 12  | 6   | 10  | 4   | 4   | 4   | Cận chiến mạnh, kháng vật lý |
| Undead      | 6   | 6   | 12  | 8   | 6   | 4   | Không hồi máu, miễn độc |
| Dragonkin   | 10  | 10  | 10  | 10  | 10  | 6   | Rất mạnh nhưng tăng cấp chậm |

> Giới hạn có thể được tăng qua tiến hóa, tăng cấp, hoặc vật phẩm huyền thoại.

---

## Resource Management System

### Tài nguyên chính:
- **Gold**: Dùng để nâng cấp công trình, thuê lính, mua trang bị.
- **Mana Crystals**: Dùng để thi triển phép, nâng cấp công nghệ ma thuật.
- **Soul Shards**: Đơn vị hiếm, dùng để triệu hồi anh hùng, kỹ năng tối thượng.
- **Influence**: Chỉ số ảnh hưởng chính trị / uy tín nhân vật trong faction.

---

## Class System:
[`class-system.md`](./class-system.md): Chi tiết về hệ thống class, chỉ số unlock, trait ảnh hưởng, kết hợp với chủng tộc.

## NPC System (AI & Personality)
- Tuyển dụng NPC:

    - Người chơi gacha NPC để vận hành công trình (quán ăn, nông trại, lò rèn...).

    - NPC có chỉ số riêng + class riêng, không khác gì một nhân vật “mini-hero”.

- Tính cách (Personality):

    - Mỗi NPC sinh ra kèm tính cách AI độc lập (ví dụ: nghiêm túc, lười biếng, tham lam, hiền lành, trung thành...).

    - Tính cách ảnh hưởng đến hành vi làm việc (tăng năng suất, giảm chi phí, hoặc gây rắc rối).

- Quan hệ với người chơi:

    - Người chơi có thể tăng thiện cảm bằng cách cho quà, trò chuyện, hoàn thành nhiệm vụ cá nhân.

    - Khi thiện cảm cao, NPC sẽ mở thêm tính năng hoặc buff đặc biệt.

    - Khi thiện cảm thấp, NPC có thể bỏ việc, phản bội, hoặc tạo event bất ngờ.

- AI Behavior:

    - NPC hoạt động bán tự động theo vai trò (Blacksmith tự rèn đồ, Farmer tự gieo trồng, Healer tự hỗ trợ).

    - Có thể ra lệnh sơ đồ chiến thuật (AI Pattern), nhưng vẫn giữ sự ngẫu nhiên để tạo cảm giác “sống thật”.

## ERD
[`Link`](https://fortress-of-the-fallen.github.io/.github/erd/)
