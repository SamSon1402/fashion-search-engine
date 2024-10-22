# Fashion Search Engine 🔍👗

![202410111238](https://github.com/user-attachments/assets/cf64e89a-a54b-48cc-a7aa-fcd9a614dc50)


A Streamlit-based web application that uses deep learning to find similar fashion items based on uploaded images. The app leverages pre-trained models (VGG16, ResNet50, and Xception) to extract features from images and perform similarity searches across a fashion product database.

## 🌟 Features

- Upload and process fashion images in real-time
- Choose between three powerful deep learning models:
  - VGG16
  - ResNet50
  - Xception
- View top 10 similar fashion items with product details
- Interactive user interface with progress tracking
- Efficient caching system for faster subsequent searches

## 🛠️ Prerequisites

- Python 3.7+
- TensorFlow 2.x
- Streamlit
- Pandas
- NumPy
- Pillow (PIL)

## 📦 Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/fashion-search-engine.git
cd fashion-search-engine
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

## 📁 Project Structure

The project requires the following structure:
```
fashion-search-engine/
├── app.py
├── current_farfetch_listings.csv
├── model-img/
│   └── model/
│       └── [image files]
├── requirements.txt
└── README.md
```

## 🚀 Usage

1. Start the Streamlit app:
```bash
streamlit run app.py
```

2. Access the web interface through your browser (typically at `http://localhost:8501`)

3. Upload a fashion image using the file uploader

4. Select a model for feature extraction

5. View similar fashion items with their details:
   - Brand name
   - Price
   - Product description

## 💾 Data Requirements

The application expects:
- A CSV file named `current_farfetch_listings.csv` containing product information
- A directory structure with fashion images stored in `model-img/model/`

The CSV file should include the following columns:
- `images.model`
- `brand.name`
- `priceInfo.formattedFinalPrice`
- `shortDescription`

## 🔄 Model Information

### VGG16
- Input image size: 224x224
- Feature extraction layer: 'block5_pool'

### ResNet50
- Input image size: 224x224
- Feature extraction layer: 'conv5_block3_out'

### Xception
- Input image size: 299x299
- Feature extraction layer: 'block14_sepconv2_act'

## ⚡ Performance

- Dataset loading and processing time is displayed in the app
- Features are cached for improved performance
- Progress bar indicates dataset loading status

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 📧 Contact

Your Name - [https://www.linkedin.com/in/sameer-m-b73376167/)

Project Link: [https://github.com/yourusername/fashion-search-engine](https://github.com/SamSon1402/fashion-search-engine)
