# Photo Personalike Poster

[English](#english) · [中文](#中文)

## 中文

一个 Codex 图片生成 Skill：将上传的人物、宠物、动物、物件、混合场景或风景照片转换成原创二维插画。

### 两种视觉模式与混合路由

- **主体 / 波普朋克二维海报**：适用于人物、多人、宠物、动物和物件。保留身份、数量、姿势、外形、服装或斑纹等关键特征；以猩红为主要冲击色、少量群青增加深度，通过倾斜断裂面板、撕纸边、粗黑分隔、网点和错位轮廓形成反叛、青春的登场动势。
- **风景 / 电影感二维场景**：适用于地点和环境。保留视角、天气、地标和空间关系，采用高饱和多色、分层光线与明确情绪焦点，不受主体模式限色约束。
- **主体 + 风景**：用户指定优先级时遵从用户；未指定时默认采用主体海报模式，并将三至五个地点特征保留为背景线索。若用户强调旅行地点或建筑，则使用风景模式，同时保持人物或宠物的数量、姿态和识别特征。

用户指定比例时优先遵从。未指定时，主体海报默认竖版 `4:5`；风景保持原图方向和近似比例，需要横向电影化裁切时使用 `16:9`。

### 风格借鉴与边界

风景只借鉴动画电影和游戏过场中常见的高饱和色彩、电影化光线、空间分层和情绪焦点；主体海报只借鉴反叛波普二维海报的拼贴、撕裂与高对比方法。Skill 不复刻任何游戏截图、角色、专有界面、文字、Logo、镜头框选、构图或具体作品的视觉签名。

### 致谢与非关联声明

本项目在主体海报的高对比图形语言上，参考了 Atlus《女神异闻录 5》的美术方向所体现的高层次设计方法。该参考不包括任何游戏截图、角色、UI、文字、Logo、构图或其他受保护素材。本项目为非官方原创项目，与 Atlus 及其关联公司不存在合作、赞助、认可或其他关联关系。

### 使用

在 Codex 中上传一张照片，然后请求：

```text
Use $photo-personalike-poster to transform this photo.
```

没有照片时，Skill 会先要求上传，不会凭空创建身份主体。最终图片保存到当前项目的 `images/photo-personalike-poster/`，只保留最新正式版本。

### 示例图片来源

- 风景原图由本人拍摄。
- 人物原图使用 OpenAI Image 2 生成。

示例仅用于展示二维化程度、色彩逻辑、主体层级、阴影与构图强度，不得复制其中的人物、地点、服装、姿势、道具、文字或具体构图。下方使用轻量预览图；点击图片可查看对应完整示例。

### 示例画廊 / Example gallery

每组按“原图 → 生成结果”展示。/ Each pair shows “source → generated result.”

| 示例 / Example | 原图 / Source | 生成结果 / Generated result |
| --- | --- | --- |
| 夜桥 / Night bridge | <a href="assets/examples/night-bridge-source.jpeg"><img src="assets/readme/night-bridge-source.jpg" alt="Night bridge source photo" width="300"></a> | <a href="assets/examples/night-bridge-landscape-cinematic.png"><img src="assets/readme/night-bridge-landscape-cinematic.jpg" alt="Night bridge illustrated result" width="300"></a> |
| 河畔夕景 / River sunset | <a href="assets/examples/river-sunset-source.jpeg"><img src="assets/readme/river-sunset-source.jpg" alt="River sunset source photo" width="300"></a> | <a href="assets/examples/river-sunset-landscape-cinematic.png"><img src="assets/readme/river-sunset-landscape-cinematic.jpg" alt="River sunset illustrated result" width="300"></a> |
| 寺院远眺 / Temple view | <a href="assets/examples/temple-view-source.jpg"><img src="assets/readme/temple-view-source.jpg" alt="Temple view source photo" width="300"></a> | <a href="assets/examples/temple-view-landscape-cinematic.png"><img src="assets/readme/temple-view-landscape-cinematic.jpg" alt="Temple view illustrated result" width="300"></a> |
| 鸟居通道 / Torii path | <a href="assets/examples/torii-path-source.jpg"><img src="assets/readme/torii-path-source.jpg" alt="Torii path source photo" width="300"></a> | <a href="assets/examples/torii-path-landscape-cinematic.png"><img src="assets/readme/torii-path-landscape-cinematic.jpg" alt="Torii path illustrated result" width="300"></a> |
| 夜间都市 / Night district | <a href="assets/examples/night-district-source.jpg"><img src="assets/readme/night-district-source.jpg" alt="Night district source photo" width="300"></a> | <a href="assets/examples/night-district-landscape-cinematic.png"><img src="assets/readme/night-district-landscape-cinematic.jpg" alt="Night district illustrated result" width="300"></a> |
| 坐姿人物 / Seated portrait | <a href="assets/examples/seated-portrait-source.png"><img src="assets/readme/seated-portrait-source.jpg" alt="Seated portrait source image" width="300"></a> | <a href="assets/examples/seated-portrait-subject-punk.png"><img src="assets/readme/seated-portrait-subject-punk.jpg" alt="Seated subject pop-punk result" width="300"></a> |
| 靠墙人物 / Wall portrait | <a href="assets/examples/wall-portrait-source.png"><img src="assets/readme/wall-portrait-source.jpg" alt="Wall portrait source image" width="300"></a> | <a href="assets/examples/wall-portrait-subject-punk.png"><img src="assets/readme/wall-portrait-subject-punk.jpg" alt="Wall subject pop-punk result" width="300"></a> |
| 卷发人物 / Wavy-hair portrait | <a href="assets/examples/wavy-hair-source.png"><img src="assets/readme/wavy-hair-source.jpg" alt="Wavy-hair portrait source image" width="300"></a> | <a href="assets/examples/wavy-hair-subject-punk.png"><img src="assets/readme/wavy-hair-subject-punk.jpg" alt="Wavy-hair subject pop-punk result" width="300"></a> |

### 内容结构

```text
photo-personalike-poster/
├── SKILL.md
├── agents/openai.yaml
├── references/
│   ├── photo-personalike-poster-prompt.zh-CN.md
│   └── photo-personalike-poster-prompt.en.md
├── assets/
│   ├── examples/
│   └── readme/
├── README.md
├── LICENSE
└── NOTICE
```

本项目使用 [Apache License 2.0](LICENSE)。第三方商标、游戏名称与相关知识产权归各自权利人所有。

## English

A Codex image-generation skill that turns an uploaded person, pet, animal, object, mixed subject-and-place, or landscape photo into an original 2D illustration.

### Two visual modes and mixed routing

- **Subject / Pop-punk 2D poster:** for people, groups, pets, animals, and objects. It preserves identity, count, pose, shape, clothing, markings, and other defining traits. Scarlet provides the main impact, restrained ultramarine adds depth, and fractured diagonal panels, torn edges, heavy black separators, halftone, and offset contours create rebellious youthful motion.
- **Landscape / Cinematic illustrated scene:** for places and environments. It preserves viewpoint, weather, landmarks, and spatial relationships while using saturated multicolor, layered light, and one emotional focus without the subject mode's palette restriction.
- **Subject + landscape:** follow an explicit user priority. Otherwise default to subject-poster treatment and preserve three to five defining place facts as background cues. If the user emphasizes a travel destination or architecture, use landscape mode while retaining the people or pets' count, pose, and identifying traits.

A user-specified aspect ratio takes priority. Otherwise subject posters default to vertical `4:5`; landscapes preserve source orientation and approximate ratio, using `16:9` when a new horizontal cinematic crop is needed.

### Inspiration and boundary

Landscapes borrow only broad qualities often found in animated films and game cutscenes: saturated color, cinematic light, spatial layering, and an emotional focus. Subject posters borrow only rebellious pop-art methods such as collage, tearing, and high-contrast composition. The Skill never recreates a game screenshot, character, proprietary interface, text, logo, camera crop, composition, or a particular work's visual signature.

### Acknowledgment and non-affiliation

The high-contrast graphic language of the subject posters draws high-level design inspiration from the art direction of Atlus's *Persona 5*. This reference excludes game screenshots, characters, UI, text, logos, compositions, and other protected material. This is an unofficial original project and is not affiliated with, sponsored by, endorsed by, or otherwise connected to Atlus or its affiliated companies.

### Usage

Upload a photo in Codex, then ask:

```text
Use $photo-personalike-poster to transform this photo.
```

Without an attached photo, the Skill asks for one instead of inventing an identity-bearing subject. Final images are saved to `images/photo-personalike-poster/` in the current project, keeping only the latest formal version.

### Example image sources

- Original landscape photos were taken by the repository author.
- Portrait source images were generated with OpenAI Image 2.

Examples demonstrate only the degree of 2D stylization, color logic, subject hierarchy, shadows, and composition strength. Do not copy their people, places, clothing, poses, props, text, or exact compositions. The gallery uses lightweight previews; click an image to open its full example.

### Contents

```text
photo-personalike-poster/
├── SKILL.md
├── agents/openai.yaml
├── references/
├── assets/examples/
├── assets/readme/
├── README.md
├── LICENSE
└── NOTICE
```

Licensed under the [Apache License 2.0](LICENSE). Third-party trademarks, game titles, and related intellectual property remain the property of their respective owners.
