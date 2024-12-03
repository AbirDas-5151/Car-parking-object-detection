# Vehicle Counter Using YOLOv8 and SORT Tracker

This project is a **real-time vehicle counter** that detects and tracks vehicles in a video feed using the YOLOv8 object detection model and the SORT tracking algorithm. It provides an accurate count of vehicles crossing a defined line in the frame and is ideal for traffic monitoring systems.

---

## 🚀 **Features**
- **Real-Time Detection and Counting**: Detects and tracks vehicles (cars, trucks, buses, motorbikes) in real-time.
- **YOLOv8 for Object Detection**: Uses the YOLOv8 model for high-speed and accurate object detection.
- **SORT Tracker**: Utilizes the SORT (Simple Online and Realtime Tracking) algorithm for tracking objects across frames.
- **Customizable Counting Zone**: Define a specific line in the frame for counting vehicles.
- **Overlay Graphics**: Enhance visuals with overlay graphics and bounding boxes.

---

## 🛠️ **Technologies Used**
1. **Programming Language**: Python
2. **Libraries**:
   - OpenCV: For video processing and visualization.
   - NumPy: For numerical computations.
   - cvzone: For easy visualization of bounding boxes and text.
   - YOLOv8 (from the `ultralytics` library): For object detection.
   - SORT: For tracking detected vehicles across frames.

---

## 📋 **Setup Instructions**

### 1. Clone the Repository
```bash
git clone https://github.com/yourusername/vehicle-counter.git
cd vehicle-counter
```

### 2. Install Dependencies
Ensure you have Python 3.7+ installed, then run:
```bash
pip install ultralytics opencv-python numpy cvzone
```

### 3. Prepare Required Files
- **YOLO Weights**: Download YOLOv8 weights (e.g., `yolov8l.pt`) from the [Ultralytics YOLOv8 GitHub](https://github.com/ultralytics/ultralytics).
- **Mask and Graphics**: Add `mask.png` and `graphics.png` files for masking the region of interest and overlaying graphics.

Place these files in the project directory.

### 4. Run the Program
Run the vehicle counter:
```bash
python vehicle_counter.py
```

---

## 📂 **Project Files**
- `vehicle_counter.py`: Main script for vehicle counting.
- `mask.png`: Defines the region of interest for detection.
- `graphics.png`: Overlay graphics for visual enhancement.
- `Videos/cars.mp4`: Sample video for testing.

---

## ⚙️ **How It Works**
1. **Object Detection**: YOLOv8 detects vehicles in each frame.
2. **Tracking**: SORT tracks detected vehicles across frames.
3. **Counting**: Vehicles crossing a predefined line are counted, ensuring each vehicle is counted only once.
4. **Visualization**: Displays bounding boxes, vehicle IDs, and total count on the video feed.

---

## 🎯 **Customization**
- **Detection Classes**: Modify the detection logic to include or exclude specific classes (e.g., add `bicycle` or exclude `motorbike`).
- **Counting Line**: Change the `limits` variable to redefine the counting zone.
- **Confidence Threshold**: Adjust the confidence threshold to fine-tune detection accuracy.

---

## 📊 **Potential Applications**
- Traffic monitoring and analytics.
- Smart city and IoT systems.
- Vehicle flow analysis for highways, toll booths, or parking lots.

---

## 🤝 **Contributions**
Contributions are welcome! Here's how you can contribute:
1. Fork the repository.
2. Create a feature branch (`git checkout -b feature-name`).
3. Commit your changes (`git commit -m "Add feature"`).
4. Push to the branch (`git push origin feature-name`).
5. Open a pull request.

---

## 📜 **License**
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

---

## 📧 **Contact**
For any questions or feedback, feel free to contact me:
- **Email**: addyabir111@gmail.com
- **GitHub**: [AbirDas-5151](https://github.com/AbirDas-5151)

---

## 📝 **Acknowledgments**
- **Ultralytics YOLO**: For providing state-of-the-art object detection models.
- **SORT Algorithm**: For real-time object tracking.
- **OpenCV and cvzone**: For simplifying video processing and visualization.

Happy coding! 😊
