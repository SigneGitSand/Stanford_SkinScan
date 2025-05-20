# Stanford_SkinScan
## Project description:
This project is a web-based tool that allows users to analyze skin lesion images and receive AI-generated medical insights. It combines a deep learning model for image classification (EfficientNet) with an LLM-enhanced knowledge base built from medical PDFs. Users can upload lesion photos and input symptoms; the app then classifies the lesion and provides a medically informed explanation using the most relevant text from trusted medical sources.
Disclaimer: This tool is for educational and informational purposes only. It does not replace professional medical advice.

## Installation guide: 
Install the following dependencies:
pip install streamlit gradio pillow pyngrok PyMuPDF sentence-transformers torchvision

A api key for OPENROUTER will also be needed to run the software. 


## Architecture Diagram

![image](https://github.com/user-attachments/assets/6883969c-0e4e-409e-bdc9-c288edc16c76)

### Sample Input/Output
**Input Example**
Image Input: Upload of a mole/skin lesion photo
Text Note: "My mole is hurting and is growing in a weird shape. It's been changing color over the past month."

**Output Example**
Classification Result:
Melanoma: 0.89

Medical Assessment:
Based on the image classification and your notes, this lesion appears concerning and could potentially be melanoma. 

The changing shape, color, and pain you've described are warning signs that should not be ignored. Melanoma is a serious form of skin cancer that requires prompt medical attention.

RECOMMENDATION: Please consult a dermatologist as soon as possible for proper diagnosis and treatment. Early detection significantly improves treatment outcomes for melanoma.

Reference Information:
Primary Reference: Melanoma is the most dangerous form of skin cancer. These cancerous growths develop when DNA damage to skin cells triggers mutations that lead the skin cells to multiply rapidly and form malignant tumors. The primary cause is intense, occasional UV exposure (frequently leading to sunburn), especially in those who are genetically predisposed...

Secondary Reference: Warning signs of melanoma include changes in an existing mole or the development of a new pigmented or unusual-looking growth. The ABCDE rule can help identify potential melanomas: Asymmetry, Border irregularity, Color variation, Diameter larger than 6mm, and Evolving size, shape, or color...
