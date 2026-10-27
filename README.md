# Wine Classification using Deep Learning

A Keras neural network that classifies wines into 3 classes using 13
chemical measurements (alcohol, flavanoids, proline, etc.).

## Model
- Input (13 features) -> Dense(8, ReLU) -> Dense(3, Softmax)
- Optimizer: Adam, Loss: Sparse Categorical Crossentropy
- StandardScaler (fit on training data only), 50 epochs, batch size 4

## Results
- Test accuracy: about 100% on 36 test samples
- Training and validation loss decrease together (no overfitting)

## Dataset
The Wine dataset from scikit-learn (178 real samples, 3 classes).
It is a clean, easy dataset, so high accuracy is common here and
does not reflect performance on harder real-world data.
