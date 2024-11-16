# BLIP-2 Chat Notebook - 

This repository contains two Jupyter notebooks for experimenting with BLIP-2, an advanced image-to-text generation model. The notebooks are designed for different purposes, showcasing the model's capabilities in generating textual descriptions from images and handling various optimizations.

## Overview of the Notebooks

1. **Chat_with_BLIP_2.ipynb**
   - This notebook demonstrates the core functionality of BLIP-2 in generating text descriptions for given images. It is an interactive chat-style implementation where users can upload images and receive natural language responses about the image's content.
   - The notebook provides a friendly interface for understanding how the BLIP-2 model interprets visual input and converts it to human-like descriptive sentences. It is an excellent resource for those wanting to learn about image-captioning models.

2. **Chat_with_BLIP_2_[int8_bitsandbytes].ipynb**
   - This notebook takes the original BLIP-2 model and optimizes it using int8 quantization with the bitsandbytes library. The optimization reduces memory usage, making it possible to run the model on systems with limited hardware resources while retaining most of its accuracy.
   - This variant is especially useful for users who need a lightweight version of BLIP-2 for deployment on smaller devices or in scenarios with memory constraints.

## Key Features

- **Image-to-Text Generation**: Both notebooks allow users to input images and receive textual descriptions, using BLIP-2's sophisticated image-captioning capabilities.
- **Optimized Version**: The quantized notebook allows for more efficient usage of hardware resources, demonstrating the use of bitsandbytes for model compression.
- **Interactive Demo**: The chat-style interface gives users a hands-on experience with image understanding and caption generation.

## Requirements

- Python 3.8+
- Jupyter Notebook
- Dependencies listed in `requirements.txt` (if applicable)

### Installation Steps

1. **Clone the Repository**
   ```sh
   git clone <repository_url>
   cd <repository_directory>
   ```

2. **Install Dependencies**
   ```sh
   pip install -r requirements.txt
   ```

3. **Run the Notebook**
   ```sh
   jupyter notebook
   ```

   Open the respective notebook in Jupyter to start exploring.

## Usage

- Launch either of the Jupyter notebooks.
- Follow the instructions to load an image and see BLIP-2 generate a caption.
- For the optimized notebook, experience how BLIP-2 maintains performance while reducing hardware requirements.

## Notes

- For best results, ensure that images are clear and well-lit to help BLIP-2 provide more accurate descriptions.
- The optimized version may have slightly reduced accuracy compared to the full-precision model.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- Thanks to the developers of BLIP-2 and the bitsandbytes library for enabling efficient quantization of models.
- Special thanks to the open-source community for providing support and resources for model optimization.

