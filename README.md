# DRS - Decision Review System in Cricket 🏏

Welcome to the DRS (Decision Review System) repository! 🎉 This project implements a graphical user interface (GUI) for reviewing cricket decisions using video playback. Built with Python's Tkinter and OpenCV libraries, this system allows users to play, rewind, and fast-forward video clips of cricket incidents, and display decisions like "Out" or "Not Out". 🎥

## Features 🌟

   - **Video Playback:** Play, rewind, and fast-forward cricket video clips. 🎬
   - **Decision Display:** Show pending decisions and final outcomes (Out/Not Out). 🚦
   - **User-Friendly Interface:** Intuitive buttons and layout for easy navigation. 🎨
   - **Threading Support:** Smooth interaction with the GUI during video playback. 🧵

## Requirements 🔧
   - Python 3.x
   - OpenCV
   - Pillow
   - imutils

## Installation 🧑‍💻

   To get started with the DRS system, follow these steps:

1. **Clone the Repository:** 🌳

   ```bash
   git clone git@github.com:Bitwise-AR/DRS_System_In_Cricket.git
   cd DRS_System_In_Cricket

2. **Install Required Libraries:** 📚

   Ensure you have Python installed (preferably Python 3.6 or higher). Install the required libraries using pip:
    ```bash
      pip install opencv-python Pillow imutils

4. **Prepare Video and Images:** 🖼️
   Make sure you have the video file (runout.mp4) and the required images in an images directory as follows:
    ```text
      images/
      ├── background.jpg
      ├── decision-pending-cricket.png
      ├── icc.png
      ├── out.png
      ├── not_out.png
      └── welcome.jpg
    ```

## Usage 🪜

  Replace the file `clip.mp4` 📽️ with the clip of the runout you want to analyze and boom💥! You are good to go...
  
  To run the DRS application, execute the following command in your terminal: 💻
  ```bash
    python main.py
  ```

  This will launch the GUI, where you can control the video playback and make decisions. 🎮

## Controls ⚙️

  - **Rewind (Fast/Slow):** Use the buttons to rewind the video at different speeds. ⏪
  - **Forward (Fast/Slow):** Use the buttons to move forward in the video. ⏩
  - **Give Out/Not Out:** Click these buttons to display the respective decision. ☝️🙅

## Modules and Libraries Used 🧿

   This project utilizes the following Python libraries:
      - **Tkinter:** For creating the GUI.
      - **OpenCV (cv2):** For video processing and image handling.
      - **Pillow (PIL):** For image manipulation and display.
      - **Imutils:** For additional image processing functions.
      - **Threading:** For managing concurrent execution during video playback.

## Code Overview 👀
  The main components of the code include:
  - **Video Playback:** Managed by the `play_video` function, which controls the current frame of the video. 🎥
  - **Decision Handling:** The `give_out` and `give_not_out` functions trigger the display of decision images after a brief delay. 🕰️
  - **GUI Layout:** Built using Tkinter, with buttons styled for a consistent look and feel. 🎨

## Key Functions 🔦
  - **`resize_with_aspect_ratio(image, width=None, height=None, inter=cv2.INTER_AREA)`:** Resizes an image while maintaining its aspect ratio. The function takes parameters for width and height, and it adjusts the dimensions accordingly to preserve the aspect ratio. 📏
  - **`play_video(play_speed)`:** Plays the video at a specified speed. ⏸️
  - **`show_pending(decision)`:** Displays the decision pending image, then shows the sponsor image, and finally the decision outcome. 🏆
  - **`give_out() and give_not_out()`:** Handle the decision-making process and update the GUI accordingly. 👨‍⚖️

## Contributing 🤝
  Contributions are what make the open-source community such an amazing place to learn, inspire, and create. Any contributions you make are greatly appreciated.

   If you have a suggestion that would make this project better, please fork the repository and create a pull request. You can also simply open an issue with the tag    "enhancement".

   - **Fork the Project**
   - **Create your Feature Branch (`git checkout -b feature/AmazingFeature`)**
   - **Commit your Changes (`git commit -m 'Add some AmazingFeature'`)**
   - **Push to the Branch (`git push origin feature/AmazingFeature`)**
   - **Open a Pull Request**

## License 📜
  This project is open-source and available under the [MIT License](LICENSE)
