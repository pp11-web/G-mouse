# G-Mouse

## Introduction

**G-Mouse** is a Python-based graphical mouse control application that uses hand gestures to control the mouse pointer via a webcam. It utilizes computer vision to track hand movements and simulate mouse actions like clicks and scrolling. This project aims to provide an intuitive and hands-free way to control the mouse, potentially improving accessibility for users with physical disabilities or offering an innovative control method for interactive environments.

## Features

- **Real-time hand tracking:** Detects and tracks hand movements to control the mouse.
- **Mouse control:** Simulates mouse clicks, pointer movements, and scrolling actions.
- **Gesture recognition:** Hand gestures control mouse functions like left/right clicks and dragging.
- **Cross-platform:** Works on Windows, macOS, and Linux.
- **Lightweight and easy to set up:** Requires only a webcam and basic Python libraries.

## How It Works

The G-Mouse application uses **OpenCV** for real-time hand tracking. By detecting the user's hand, it calculates the relative position of the hand to simulate mouse movements. The application uses the **PyAutoGUI** library to execute system-level mouse actions like clicks and drags based on the gestures detected by the camera.

### Key Steps:
1. The webcam captures video input.
2. The software processes the video feed and detects hand gestures.
3. Hand gestures are converted into mouse actions (movement, clicks, scrolling).

## Prerequisites

Before running the project, ensure you have:

- **Python 3.x**
- A working **webcam**
- The required Python libraries (OpenCV, PyAutoGUI)

## Installation

1. Clone the repository:

    ```bash
    git clone https://github.com/pp11-web/G-mouse.git
    ```

2. Navigate to the project directory:

    ```bash
    cd G-mouse
    ```

3. Install the dependencies:

    ```bash
    pip install -r requirements.txt
    ```

    This will install the necessary libraries like OpenCV and PyAutoGUI.

## Usage

Once you've installed the necessary dependencies, you can run the application by following these steps:

1. Run the application:

    ```bash
    python g_mouse.py
    ```

2. Control the mouse with your hand gestures:
   - Move your hand in front of the webcam to control the mouse pointer.
   - Perform clicking and scrolling using predefined hand gestures.
   
   *Note: You may customize the gestures and sensitivity by modifying the code.*

## Customization

You can tweak the following within the code:
- **Sensitivity:** Adjust how fast or slow the mouse moves based on hand movement.
- **Click gestures:** Modify the gestures used for left-click, right-click, and drag actions.
- **Processing rate:** Adjust the frame processing rate to optimize performance based on your system capabilities.

## Contributing

We welcome contributions to the project! To contribute:

1. **Fork** the repository.
2. Create a **new branch**:

    ```bash
    git checkout -b feature/your-feature
    ```

3. **Commit** your changes:

    ```bash
    git commit -m "Add a new feature"
    ```

4. **Push** the branch:

    ```bash
    git push origin feature/your-feature
    ```

5. Open a **Pull Request**.

## Future Enhancements

Potential future improvements:
- More advanced gesture recognition (e.g., multi-finger gestures).
- Voice control integration.
- Machine learning models to improve hand detection accuracy.

## License

This project is licensed under the **MIT License**. For more details, see the [LICENSE](LICENSE) file.

## Acknowledgements

Special thanks to the open-source community and the developers behind the tools and libraries (OpenCV, PyAutoGUI) that made this project possible.

