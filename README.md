# ASL Alphabet Classification with Machine Learning

## Problem Definition

Effective communication is essential in today's interconnected world. For individuals who are deaf or hard of hearing, American Sign Language (ASL) provides a powerful means of expressing emotions and ideas. However, interpreting ASL gestures through machine learning remains a challenging task.

This project aims to build a machine learning model capable of classifying ASL hand signs for the English alphabet (A–Z). By translating hand gestures into recognized letters, the model serves as a step toward improving accessibility and bridging communication gaps for ASL users.

The task is formulated as a multiclass, single-label classification problem:

- **Multiclass**: Each image represents one of 26 letters (A–Z).
- **Single-label**: Each image corresponds to only one letter, with no ambiguity or overlap.

## Dataset

The dataset used is the [ASL Alphabet Dataset](https://www.kaggle.com/datasets/grassknoted/asl-alphabet) from Kaggle, which contains:

- 78,000 color images (3,000 per class)
- Resolution: 200x200 pixels
- 26 classes corresponding to the ASL letters A–Z

Due to hardware constraints, this project uses a subset of 100 images per class.

### Preprocessing Considerations

To improve training efficiency and reduce complexity:

- **Image resizing** was applied to lower computational cost and training time.
- **Color-to-grayscale conversion** was performed to focus the model on shape and structure rather than color information.

These steps help minimize overfitting and ensure the model concentrates on the essential visual features of each sign.

## Project Goal

To develop a robust model that can:

- Accurately classify ASL hand signs representing letters A–Z
- Serve as a foundational tool for future applications in ASL recognition and communication accessibility
