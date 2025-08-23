# Hệ Thống Class - Fortress of the Fallen

## Cơ chế mở khóa

- **Không dựa vào level**, mà dựa vào:
  - **Chỉ số** (Strength, Intelligence, Dexterity, Vitality, Charisma, Wisdom)
  - **Traits**: Karma (Thiện/Ác), Affinity (Light/Dark), Luck, Resistance
  - **Chủng tộc** (Human, Undead, Beastkin, Elemental...)
  - **Trang bị đặc biệt hoặc sách kỹ năng**
- Một nhân vật có thể **unlock nhiều class** nhưng chỉ **kích hoạt 1 class chính** tại một thời điểm.

---

## Cây Class Cơ Bản (Basic Paths)

| Gốc Chính  | Class Gốc            | Điều kiện                                 |
|-----------|----------------------|-------------------------------------------|
| Vật lý     | Warrior              | Strength ≥ 20                              |
| Vật lý     | Archer               | Dexterity ≥ 20                             |
| Phép thuật | Mage                 | Intelligence ≥ 20                          |
| Phép thuật | Healer               | Wisdom ≥ 20                                |
| Hỗn hợp    | Rogue                | Dexterity ≥ 15 + Strength ≥ 10             |
| Hỗn hợp    | Tactician            | Intelligence ≥ 15 + Charisma ≥ 15          |

---

## Class Trung Cấp 

| Class                 | Điều kiện mở khóa |
|-----------------------|------------------|
| Knight                | Warrior + Vitality ≥ 30            |
| Paladin               | Warrior + Karma ≥ 60 + Affinity = Light |
| Dark Knight           | Warrior + Karma ≤ -60 + Affinity = Dark |
| Sniper                | Archer + Dexterity ≥ 40            |
| Assassin              | Rogue + Dexterity ≥ 25 + Luck ≥ 20 |
| Battle Mage           | Mage + Strength ≥ 15               |
| Necromancer           | Mage + Affinity = Dark + Intelligence ≥ 35 |
| Sage                  | Healer + Wisdom ≥ 40               |
| War Priest            | Healer + Strength ≥ 20 + Karma ≥ 40 |
| Commander             | Tactician + Charisma ≥ 30 + Wisdom ≥ 20 |

---

## Class Cao Cấp 

| Class                 | Điều kiện mở khóa |
|-----------------------|------------------|
| Hero                  | Knight + Karma ≥ 80 + Charisma ≥ 40 |
| Deathlord             | Dark Knight + Necromancer + Resistance ≥ 40 |
| Shadow Reaper         | Assassin + Karma ≤ -80 + Luck ≥ 40 |
| Arcane Lord           | Battle Mage + Intelligence ≥ 50     |
| Grand Sage            | Sage + Wisdom ≥ 60 + Resistance ≥ 30 |
| Beastmaster           | Any base + Charisma ≥ 30 + chủng tộc Beastkin |
| Warlord               | Commander + Strength ≥ 35 + Vitality ≥ 30 |
| Druid                 | Mage + Affinity = Light + Luck ≥ 30 |
| Hexblade              | Rogue + Mage + Curse Weapon         |

---

## 🧬 Class Độc Quyền theo Chủng Tộc

| Chủng tộc   | Class đặc biệt      | Điều kiện |
|-------------|---------------------|-----------|
| Undead      | Lich                | Necromancer + Undead + Karma ≤ -50 |
| Beastkin    | Feral Warden        | Strength ≥ 30 + Beastkin           |
| Elemental   | Stormcaller         | Intelligence ≥ 35 + Resistance ≥ 25 |
| Dragonkin   | Dragoon             | Vitality ≥ 40 + Charisma ≥ 30 + Dragonkin |
| Human       | Enlightened         | Wisdom ≥ 60 + Luck ≥ 40 + Human    |
| Demon       | Abyss Knight        | Strength ≥ 40 + Karma ≤ -80 + Demon |

---

## Trait và Ảnh Hưởng

| Trait       | Ảnh hưởng đến |
|-------------|----------------|
| Karma       | Thiện / Ác ảnh hưởng class thiên hướng Light/Dark |
| Affinity    | Quyết định hướng kỹ năng (Holy, Dark, Elemental) |
| Luck        | Tăng khả năng học kỹ năng hiếm / tránh né / crit |
| Resistance  | Giảm hiệu ứng bất lợi, mở class phép cao cấp |

---

## Trang bị mở khóa class

| Tên trang bị           | Mở khóa class |
|------------------------|---------------|
| **Cursed Blade**       | Hexblade      |
| **Book of Eternal Night** | Necromancer / Lich |
| **Crown of Light**     | Paladin / Sage |
| **Demonic Pact Ring**  | Abyss Knight |
| **Ancient Beast Horn** | Feral Warden |

---

## Ghi chú

- Một nhân vật có thể giữ nhiều class đã mở khóa, và **chuyển đổi giữa các class đã mở khi không trong trận**.
- Việc chọn đúng chỉ số và trait phù hợp giúp bạn **phát triển nhân vật theo hướng mong muốn**, tạo nên đội hình đa dạng.
- NPC có class riêng → ảnh hưởng đến cách họ vận hành công trình (Ví dụ: Blacksmith = Warrior class, Librarian = Mage class, Farmer = Druid…).
