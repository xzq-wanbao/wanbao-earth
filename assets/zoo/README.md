# 动物图标

- 来源：`素材库\动物`（原 `D:\兵种插画\宝物\纪元1800\透明底\动物`）
- 共 141 张 PNG：`zoo_001.png ... zoo_135.png` 由 `tools/build-zoo-assets.js` 复制，`zoo_136.png ... zoo_141.png`（狐狸/猎鹰/考拉/貘/霍加狓/白鲸）由 `tools/import_assets.py` 追加，并写入 `src/04c-animals.js` 图鉴数据。
- 稀有度按大洲配额：**每个大洲 2 金 + 5 紫**，其余蓝色（合计 12 金 / 30 紫 / 99 蓝），由 `build-zoo-assets.js` 的 `ANIMAL_RARITY_PLAN` 控制。
- 素材库里不少 `.png` 实际是 WebP，导入脚本会统一解码并保存为真正的 PNG。
- 图片仅用于本项目的帝国宝藏（动物园）功能；版权/使用范围请遵循素材原出处。
