
# Dynamic AI: Fractal Universe Chocolate Wafer Model (FUCWM)

LM Studio - Fractall Ball chat currently live: 

[Watch the YouTube Live Video](https://www.youtube.com/live/LlnCpfqgqjU)

Dynamic AI is an experimental neural network model inspired by fractal structures in the universe and the human brain. It incorporates recursive nodes (FractalNodes) to dynamically grow and learn through Hebbian-like updates and pruning. The model also integrates a VAE (Variational Autoencoder) for encoding latent space representations. This repository contains the code for training, chatting, and interacting with the model via a Gradio interface.

## Features

- **Recursive Fractal Nodes**: Nodes can grow and create child nodes based on the complexity of their output, simulating the recursive, fractal-like nature of the brain and the universe.
- **Variational Autoencoder (VAE)**: Encodes latent representations of inputs.
- **Layer Normalization and Xavier Initialization**: Enhances training stability.
- **Dynamic Complexity-based Growth**: Nodes grow based on complexity thresholds and manage child connections.
- **Dynamic AI Chat**: Users can interact with the model to generate responses.
- **LM Studio Integration**: Chat with a local LM Studio instance in a collaborative conversational framework.
- **Gradio Interface**: A user-friendly interface to interact with the AI model, train it on Q&A pairs, and simulate conversations with LM Studio.

## What it is?

Think Fractal ball around big bang with chocolate wafer inspired super weights that add complexity to normal weights. 
The depth setting can make the ball complexities explode to Nan territory real fast and there was a real fight to keep the 
complexity setting at bay. It was a wild idea coded by Claude and o1 model. 
  
## Requirements
- Python 3.8+
- PyTorch
- Gradio
- LM Studio (optional, for integration with the `talk_with_lm_studio` feature)
- Etc
The requirements.txt was written by ChatGPT. I have not tested if it would work as it is.

## Problems?

Ask from Claude / ChatGPT. Paste them this and the code. They will understand what to do. 

## Installation

1. Clone this repository:

   ```bash
   git clone https://github.com/anttiluode/DaFUC.git
   cd dynamic-ai-fractal-wafer
   ```

2. Install dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. If you're planning to use LM Studio, ensure it's installed and running locally. Configure the `lm_studio_client` by setting your API key and URL in the code.

4. Run the application:

   ```bash
   python app.py
   ```

## Usage

### 1. Chat with Dynamic AI

You can use the Gradio interface to chat with the Dynamic AI model.

- **Message**: Enter your message and adjust the temperature for creativity.
- **Response**: The AI will generate a response based on its learned knowledge.

### 2. Train the Model on Q&A Pairs

You can train the model on a list of question-answer pairs using the Gradio interface.

- **Q&A Pairs File**: Upload a JSON file containing question-answer pairs.
- **Epochs**: Set the number of training epochs.
- **Training Output**: Monitor the progress of training, including loss metrics.

### 3. LM Studio Conversation

You can simulate a collaborative conversation between Dynamic AI and LM Studio:

- **Initial Message**: Set the initial message to start the conversation.
- **Duration**: Set the duration of the conversation.
- **Delay**: Set the delay between messages.

This is a good start. The question answer pairs seem to produce more random AI. 

### 4. Save/Load Model State

You can save and load the state of the model using the Gradio interface.

- **Save State**: Save the current model state to a file.
- **Load State**: Load a previously saved state to restore the model.

## Example

To chat with Dynamic AI using the command line interface:

```bash
python app.py
```

Then, access the Gradio interface from your browser. You can interact with the AI by typing messages, training it, or saving/loading its state.

### Training Data Format

The Q&A pairs should be provided in a JSON file in the following format:

```json
[
    {"question": "What is the capital of France?", "answer": "Paris"},
    {"question": "Who wrote '1984'?", "answer": "George Orwell"}
]
```

### Contribution

Feel free to contribute to this project by submitting pull requests or opening issues for improvements or bugs.

### Issues

The depth settings are extremely important: 

    dynamic_ai = DynamicAI(vocab_size=50000, embed_dim=256, latent_dim=256, output_dim=256, max_depth=7)

    As the deeper it gets, the deeper the "fractal ball" around point one "Think big bang" gets, the more 
    complex it gets. You hit NAN (out of reach) complexity very fast and the thing wont work. 

### License

This project is licensed under the MIT License.
