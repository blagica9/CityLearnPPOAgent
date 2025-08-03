### 🔧 Environment Setup (Google Colab)

```python
# Install CityLearn
!pip install citylearn==2.3.0

# Replace gym with gymnasium
!pip uninstall -y gym
!pip install gymnasium==0.29.1

# Install Stable Baselines3
!pip install stable-baselines3[extra]==2.2.1

# Install PyTorch with CUDA 11.8
!pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu118

# Install PyTorch Geometric
!pip install torch-scatter -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
!pip install torch-sparse -f https://data.pyg.org/whl/torch-2.0.0+cu118.html
!pip install torch-geometric

# Fix versions
!pip install numpy==1.24.4 scipy==1.10.1
!pip install tensorboard==2.12.3
!pip install tensorflow==2.12.0

# Restart Colab runtime
import os
os.kill(os.getpid(), 9)
```
