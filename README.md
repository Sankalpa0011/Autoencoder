# Denoising Autoencoder for Image Noise Removal

This project implements a denoising autoencoder using Keras to remove noise from images. The autoencoder is trained on the MNIST dataset with added random noise and is capable of reconstructing clean images from noisy inputs.

## Project Structure

.
├── autoencoders_noise_removal_weights.weights.h5
├── autoencoders_noise_removal.h5
├── autoencoders_noise_removal.keras
├── Denoising Autoencoder Data Preprocessing.ipynb
├── Denoising Autoencoder Model Training.ipynb
├── Denoising Autoencoder Testing.ipynb
├── image1.jpg
├── image2.jpg
└── .ipynb_checkpoints/



### Key Files
- **`Denoising Autoencoder Data Preprocessing.ipynb`**: Prepares the MNIST dataset, adds random noise, and saves the noisy and clean datasets.
- **`Denoising Autoencoder Model Training.ipynb`**: Defines the autoencoder architecture, trains the model, and saves the trained weights and model.
- **`Denoising Autoencoder Testing.ipynb`**: Loads the trained model, evaluates it on noisy test data, and generates predictions.

## How It Works

1. **Data Preprocessing**:
   - The MNIST dataset is normalized and reshaped.
   - Random Gaussian noise is added to create noisy versions of the images.
   - The noisy and clean datasets are saved as `.npy` files.

2. **Model Architecture**:
   - The autoencoder consists of convolutional layers for encoding and decoding.
   - The encoder compresses the input into a latent representation, and the decoder reconstructs the clean image.

3. **Training**:
   - The model is trained using the noisy images as input and the clean images as output.
   - The loss function used is binary cross-entropy, and the optimizer is Adam.

4. **Testing**:
   - The trained model is used to predict clean images from noisy test data.
   - Results are visualized and saved for comparison.

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/denoising-autoencoder.git
   cd denoising-autoencoder


2. Install the required Python packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Ensure you have the MNIST dataset available (it will be downloaded automatically by Keras).

## Usage

### Data Preprocessing
Run the notebook:
jupyter notebook "Denoising Autoencoder Data Preprocessing.ipynb"


### Model Training
Run the notebook:
jupyter notebook "Denoising Autoencoder Model Training.ipynb"


### Testing
Run the notebook:
jupyter notebook "Denoising Autoencoder Testing.ipynb"



## Results

The autoencoder successfully removes noise from the images. 

## Requirements

- Python 3.7+
- TensorFlow/Keras
- NumPy
- Matplotlib
- Jupyter Notebook

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Acknowledgments

- The MNIST dataset is provided by Yann LeCun and collaborators.
- The project is inspired by the use of autoencoders for noise removal in images.


