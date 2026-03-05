=# 🫀 PranaAI: MedCardio (GAP-Optimized)

### ⚡ The "GAP" Innovation
Unlike standard models that use heavy `Flatten` layers, MedCardio uses **Global Average Pooling (GAP)**.

**Why it's Rare:**
- **Zero Parameter Weights:** GAP has no weights to train, making the model file tiny.
- **Anti-Overfitting:** It enforces a stronger link between feature maps and the diagnosis.
- **Legacy Ready:** Runs perfectly on **8GB RAM** i5 systems.

### 🛠️ Code Implementation
```python
# The GAP Optimization Protocol
model.add(layers.GlobalAveragePooling1D())
