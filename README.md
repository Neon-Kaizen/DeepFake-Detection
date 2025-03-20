# Deepfake Detection Script

This script performs deepfake detection on video files using a pre-trained model. It processes the video, detects faces, and provides predictions on whether the video is real or fake.

## Requirements

Before running the script, ensure you have the following dependencies installed:

- Python 3.x
- PyTorch
- OpenCV
- NumPy
- tqdm
- scikit-learn
- facenet-pytorch

You can install the required packages using pip:

```bash
pip install -r requirements.txt
```

## Usage

1. **Clone the repository** (if applicable) and navigate to the directory containing the script.

2. **Prepare your video files**. Ensure that the video files you want to analyze are accessible.

3. **Run the script**:

   ```bash
   python predict_celeb_df.py
   ```

4. **Input the video path** when prompted. The script will process the video and output the results.

## Functionality

- The script uses a pre-trained deepfake detection model to analyze the input video.
- It detects faces in the video frames and draws bounding boxes around them.
- The script outputs:
  - The prediction score (confidence level).
  - The predicted label (REAL or FAKE).
  - The ground truth based on the video path.
  - The total number of frames processed and faces detected.

## Notes

- Ensure that the model weights are available in the specified path (`weights/final_555_DeepFakeClassifier_tf_efficientnet_b7_ns_0_19`).
- The script is designed to run on a CUDA-enabled GPU for optimal performance. If you do not have a GPU, you may need to modify the script to run on the CPU.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

