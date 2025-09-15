# RNN-Based 3D Animation Prediction in Blender 🎥✨

This project demonstrates how to use a **Recurrent Neural Network (RNN with LSTMs)** to predict **future animation frames** and extend 3D character motion in **Blender**. Instead of static motion capture, the character continues moving in a realistic way — generated purely by AI.  

---

## 🔑 Key Steps in the Workflow
- Exported bone keyframes from Blender Python API → JSON  
- Preprocessed and normalized skeleton data (positions + quaternions)  
- Trained an **RNN (LSTMs)** to learn motion dynamics  
- Predicted future frames beyond the original sequence  
- Re-imported predictions into Blender using Python API to extend animations seamlessly  

---

## 💡 Next Steps
- Using **Transformers** for long-range motion prediction  
- Driving animations directly from **real-time video or camera feeds** (Pose Estimation → Blender armature)  
- Combining this with **generative pipelines** for character/scene creation  

---

## 📂 Project Structure
```
├── animation_data.json            # Exported Blender animation data
├── prepare_data.py                # Preprocessing & normalization
├── rnn_model.py                   # RNN model training
├── predict_future_frames.py       # Predict future frames
├── predicted_future_frames.json   # Generated predictions
```

---

## 🚀 Getting Started

1. **Prepare data**
   ```bash
   python prepare_data.py
   ```

2. **Train the model**
   ```bash
   python rnn_model.py
   ```

3. **Predict future frames**
   ```bash
   python predict_future_frames.py
   ```

4. **Import into Blender**
   - Use the provided Blender Python API script to load predictions and extend animations.

---

## 🌟 Results
AI-driven animation continues beyond the original motion capture sequence, generating new movement dynamically inside Blender.  

---

## 🤝 Collaboration
I’d love to connect with others exploring **Generative AI for Animation** — feel free to fork, experiment, and share improvements!  

#AI #MachineLearning #Blender3D #Animation #DeepLearning #GenerativeAI #RNN  
