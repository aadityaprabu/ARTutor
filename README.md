# ARTutor

ARTutor or ART is a Unity-based Augmented Reality (AR) application designed to provide an **interactive learning environment** by combining **MediaPipe body tracking**, **Python-based data processing**, and **Unity AR Foundation** for real-time humanoid avatar animation.

---

## ✨ Features

- **Body Tracking with MediaPipe (Python)**

  - Accurate body pose estimation.
  - Keypoint data processing and chunked broadcasting.

- **Real-time Data Communication**

  - UDP sockets for transmitting body landmarks.
  - Efficient buffer queues and multithreading for smooth streaming.

- **Unity Integration**

  - C# receiver threads for packet reassembly.
  - Keypoint-to-avatar mapping for realistic humanoid animation.
  - AR Foundation + ARCore integration for real-world augmentation.

- **Immersive Learning Experience**
  - Learners can visualize and mimic performer movements.
  - Enhances traditional teaching with engaging AR environments.

---

## 🛠️ Tech Stack

- **Python** – MediaPipe body tracking, data preprocessing.
- **Sockets (UDP)** – Real-time communication between Python and Unity.
- **Unity (C#)** – AR application, packet processing, and avatar animation.
- **AR Foundation + ARCore** – AR deployment on mobile devices.

---

## 📂 Project Workflow

1. **Tracking** → MediaPipe captures body pose keypoints.
2. **Processing** → Python preprocesses and splits data into chunks.
3. **Broadcasting** → Data sent over UDP with delimiters.
4. **Receiving** → Unity C# receiver thread reconstructs the data.
5. **Mapping** → Keypoints mapped to a 3D character.
6. **Augmentation** → AR Foundation + ARCore display avatar in real-world AR.

---

## 📷 Demo & Documentation

- [📄 Full Documentation](Documentation/ARTutor-report.pdf)
- [▶️ Demo Playlist](https://youtube.com/playlist?list=PLCk1Y31wvMhXjcgWnek1wSJLmZKr1x8f1)

---

## 🚀 Getting Started

### Prerequisites

- **Python 3.7+**
- **MediaPipe**
- **Unity 2020+**
- **AR Foundation & ARCore XR Plugin**

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/aadityaprabu/ARTutor.git
   cd ARTutor
   ```

2. Install Python dependencies:

   ```bash
   pip install mediapipe opencv-python
   ```

3. Open the Unity project in the Unity Editor.

4. Connect the Python backend and Unity frontend using UDP sockets.

5. Deploy the Unity AR app to your mobile device.

---

## 📜 License

This project is licensed under the **MIT License**. See the [LICENSE](./LICENSE) file for details.

---

## 🤝 Contributing

Contributions, issues, and feature requests are welcome!  
Feel free to open an issue or submit a pull request.

---

## 👨‍💻 Author

**Aaditya Prabu**

- GitHub: [@aadityaprabu](https://github.com/aadityaprabu)
