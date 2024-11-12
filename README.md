# Multimodal Deep Learning Model for Persuasion Technique Detection

## Project Overview
This project presents an advanced deep learning model designed to detect persuasive techniques in internet memes, focusing on the multimodal integration of text and image data. The model is tailored to analyze how memes, which often blend visual and textual elements, convey persuasive messages that can influence public opinion and contribute to the spread of misinformation on social media.

### The system comprises two main components:

- **Multimodal Classification Model:** This model processes both the visual and textual elements of memes using architectures like DeBERTaV2 (for text) and ResNet50/EfficientNetB0 (for image analysis). By combining these features, the model can identify specific persuasive techniques, such as appeals to authority, fear-mongering, or humor, across a wide range of memes.

- **Sequence Tagging for Overlapping Techniques:** Memes often utilize multiple persuasive strategies simultaneously, which can be difficult to distinguish. This model extension uses a multi-label sequence tagging approach to identify overlapping persuasive techniques within the same meme, marking specific text spans associated with each technique.

The model leverages Focal Loss to handle class imbalance, making it particularly effective in detecting underrepresented techniques and improving its performance on nuanced classifications. It has been evaluated rigorously, with key performance metrics like F1 scores indicating strengths in general classification while identifying areas for improvement in detecting rare persuasive techniques.

## Use Cases
This model has broad applications across social media monitoring, content moderation, and research. Social media platforms can use it to flag memes that use manipulative persuasive techniques, helping identify misinformation and uphold community standards. Researchers in media studies, political science, and psychology can leverage the model to analyze trends in persuasive content, exploring how memes shape public opinion and cultural narratives. 

Additionally, the tool can aid marketers in understanding effective strategies for audience engagement and serve as an educational resource, helping users recognize manipulative tactics in digital content. Through these applications, the model supports safer digital spaces and a deeper understanding of persuasion in online media.

## Installation

### Prerequisites
This project requires Python and the packages listed in `requirements.txt`.

### Setup
1. Clone the repository:
   ```bash
   git clone https://github.com/param-kasana/Multimodal_Deep_Learning_Model_for_Persuasion_Technique_Detection.git
   cd Multimodal_Deep_Learning_Model_for_Persuasion_Technique_Detection
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
3. **Set Up the Environment**:
   - If using Google Colab, set the variable `colab_run` to `True`:

     ```python
     colab_run = True

     if colab_run:
         from google.colab import drive
         drive.mount('/content/drive')
         directory = '/content/drive/My Drive/DL_Assign_2/'
     else:
         directory = ''
     ```

## Project Structure
- **Multimodal DL Model.ipynb**: Notebook containing the model's implementation and explanations for each step.
- **Report.pdf**: Detailed report on the project, covering the model design, feature extraction, integration, evaluation, and future improvements.
- **requirements.txt**: Lists the necessary packages to run the code.
