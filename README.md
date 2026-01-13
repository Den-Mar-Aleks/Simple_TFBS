# 🔵 Simple_TFBS — Thin/Fat Body Slider LoRA
**Flux / ZIT compatible · Safe · Stylized body-geometry manipulation**

---

## 🔍 Overview
**Simple_TFBS** is an artistic geometry-based body-shape slider LoRA.  
It modifies **only stylized body volume** in the direction of **thinner ↔ fuller**, without affecting:

- face identity  
- ethnicity  
- age  
- personality traits  

All transformations remain within **safe, non-realistic, stylized anatomy**.

---

## ⚙️ How the Slider Works

Move the `network_multiplier` into negative or positive values:

| Multiplier | Effect |
|-----------:|--------|
| `-2 → -1`   | noticeably thinner body |
| `-1 → -0.5` | slight slimming |
| `0`         | neutral (no influence) |
| `+0.5 → +1` | slight volume increase |
| `+1 → +2`   | fuller body shape |

The model adjusts **only overall body silhouette**, keeping natural structure without distortions.

---

## 🧩 Example Usage (ComfyUI / AITS Toolkit)

```yaml
lora:
  name: "dmsnoa/jix/Simple_TFBS"
  multiplier: -1.5   # thin
```

### Recommended Base Prompt
```
person, solo, standing, full body, neutral pose,
arms relaxed, looking at camera,
plain background, soft lighting,
realistic anatomy, photorealistic
```

💡 No need to mention “thin/fat” in the text —  
the slider handles shape variation automatically.

---

## 🔐 Safety Notice
- This model performs **artistic stylized body-shape modification only**.  
- Not intended for medical, diagnostic, biometric, or real-person resemblance tasks.  
- Produces **non-realistic, non-identifiable** results.  
- Commercial/non-commercial use allowed under the license.

---

## 📦 Files Included
### `/low/`
- `tfbs_low.safetensors`
- `preview_low.png` / `preview_low.mp4`
- version notes (optional)

### `/mid/`
- `tfbs_mid.safetensors`
- `preview_mid.png` / `preview_mid.mp4`
- version notes (optional)

### `/ultra/`
- `tfbs_ultra.safetensors`
- `preview_ultra.png` / `preview_ultra.mp4`
- version notes (optional)

---

## 🧾 License
**CreativeML OpenRAIL-M**  
Users must follow safety restrictions and avoid misuse as described in the license.

---

## ✏️ Author
Created by **dmsnoa/jix**

⭐ If you found the model useful — consider starring the repository!