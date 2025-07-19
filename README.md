# Building_Transformer
1) A custom-built encoder-decoder Transformer architecture.
2) Manually implemented multi-head self-attention and positional encoding.
3) Proper handling of masking (padding and look-ahead) for sequence tasks.
4) Training loop with loss calculation, optimizer state saving, and batch processing.
5) Label smoothing to improve generalization and avoid overconfidence.

# Architecture Overview
Encoder: Converts input tokens into rich vector representations using self-attention and feed-forward layers.
Decoder: Generates output tokens one step at a time, attending to both past outputs and encoder outputs.
Final Output: Transformed into word predictions over the target vocabulary.

# Training Highlights
Loss Function: CrossEntropyLoss with label smoothing and ignore_index for padding.
Optimizer: Adam with support for saving and resuming training.
Batching: Includes tokenization, padding, and dynamic masking.
Progress Monitoring: Uses tqdm to show epoch and loss updates.

# Project Structure
Whenever you are Training a Transformer
├── transformer/
│   ├── model.py          
│   ├── layers.py        
│   ├── utils.py           
│   ├── train.py          
│   ├── data_loader.py    
├── config.json            
├── README.md             

