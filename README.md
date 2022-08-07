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
	conv2d_5 (Conv2D)            (None, 198, 198, 32)      896       
	_________________________________________________________________
	activation_9 (Activation)    (None, 198, 198, 32)      0         
	_________________________________________________________________
	max_pooling2d_5 (MaxPooling2 (None, 99, 99, 32)        0         
	_________________________________________________________________
	conv2d_6 (Conv2D)            (None, 97, 97, 32)        9248      
	_________________________________________________________________
	activation_10 (Activation)   (None, 97, 97, 32)        0         
	_________________________________________________________________
	max_pooling2d_6 (MaxPooling2 (None, 48, 48, 32)        0         
	_________________________________________________________________
	flatten_3 (Flatten)          (None, 73728)             0         
	_________________________________________________________________
	dense_5 (Dense)              (None, 16)                1179664   
	_________________________________________________________________
	activation_11 (Activation)   (None, 16)                0         
	_________________________________________________________________
	dropout_3 (Dropout)          (None, 16)                0         
	_________________________________________________________________
	dense_6 (Dense)              (None, 1)                 17        
	_________________________________________________________________
	activation_12 (Activation)   (None, 1)                 0         
	=================================================================
	Total params: 1,189,825
	Trainable params: 1,189,825
	Non-trainable params: 0
	_________________________________________________________________






