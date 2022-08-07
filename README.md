# Charts_CNN_Based_MultiClassification

Python Jupyter Notebook with **2 layer Convolutional Neural Network** image classifier implemented in **Keras** 🖼️. It's **[Google Colab](https://colab.research.google.com/)** ready.

## Usage

Structure your data as follows:

	data/
		training/
			class_a/
				class_a01.jpg
				class_a02.jpg
				...
			class_b/
				class_b01.jpg
				class_b02.jpg
				...
		validation/
			class_a/
				class_a01.jpg
				class_a02.jpg
				...
			class_b/
				class_b01.jpg
				class_b02.jpg
				...

## Performance

**Dataset:** [Chart_Classification]

**Description:** Multi-class classification. 5 classes distinguish - 
    
**dot_line**  **horizontal_bar** **vertical_bar** **dot_line** **pie**

**Training:**  800 images per class

**Validation:** 40 images per class

### model

_________________________________________________________________
Layer (type)                 Output Shape              Param #   
=================================================================
conv2d_4 (Conv2D)            (None, 128, 128, 32)      896       
_________________________________________________________________
max_pooling2d_4 (MaxPooling2 (None, 64, 64, 32)        0         
_________________________________________________________________
dropout_2 (Dropout)          (None, 64, 64, 32)        0         
_________________________________________________________________
conv2d_5 (Conv2D)            (None, 64, 64, 32)        9248      
_________________________________________________________________
max_pooling2d_5 (MaxPooling2 (None, 21, 21, 32)        0         
_________________________________________________________________
flatten_2 (Flatten)          (None, 14112)             0         
_________________________________________________________________
dense_4 (Dense)              (None, 128)               1806464   
_________________________________________________________________
dense_5 (Dense)              (None, 5)                 645       
=================================================================
Total params: 1,817,253
Trainable params: 1,817,253
Non-trainable params: 0
_________________________________________________________________





