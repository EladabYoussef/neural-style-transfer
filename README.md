markdown
Copy
Edit
# 🖼️ Neural Style Transfer with TensorFlow

This project implements **Neural Style Transfer (NST)** from scratch using TensorFlow and VGG19. It blends the *content* of one image with the *style* of another, producing a new image that captures both the structural semantics and artistic texture.

In addition to the main NST process, this project also includes a simple pixel-wise **multiplication blending** comparison to illustrate the limitations of non-learned transformations versus learned feature extraction and optimization.

## 📌 Highlights

- Implemented entirely from scratch with TensorFlow (no high-level NST API)
- Uses pre-trained **VGG19** for feature extraction
- Supports custom **layer weightings** for controlling style intensity
- Visual and code-based **comparison with pixel-wise multiplication**
- Clean and modular code with training loop, cost functions, and plotting

---

## 🧠 Core Concepts

**Neural Style Transfer** works by optimizing a generated image so that its intermediate activations (from a CNN) match:

- **Style Features** of the style image (via Gram matrices)
- **Content Features** of the content image (via direct feature comparison)

**Pixel-wise Multiplication**, on the other hand, directly multiplies the RGB values of the content and style images. While it creates an interesting visual, it lacks spatial understanding and does not preserve structure.
