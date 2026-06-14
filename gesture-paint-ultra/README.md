# Gesture Paint Ultra 🎨✋

A real-time hand gesture drawing application powered by MediaPipe Hands and Computer Vision. Draw, erase, and switch colors using simple hand gestures directly from your webcam—no mouse, stylus, or touch screen required.

## 🚀 Features

* ✋ Real-time hand tracking using MediaPipe
* 🎨 Air drawing with pinch gesture
* 🧹 Erase using a closed fist gesture
* ⚫⚪ Toggle between black and white colors using a V-sign gesture
* 📏 Adjustable brush size
* 📈 Live FPS monitoring
* 📱 Responsive fullscreen canvas
* 🌐 Runs entirely in the browser
* 🔒 No backend or data collection

## 🖥️ Live Demo

Try the application here:

🔗 [**https://devesh-gawai.github.io/web-practice-project/gesture-paint-ultra/index.html**](https://devesh-gawai.github.io/web-practice-project/gesture-paint-ultra/index.html)

Enable webcam access and start drawing in the air using hand gestures.

## 🎯 Controls

| Gesture                      | Action                   |
| ---------------------------- | ------------------------ |
| Pinch (Thumb + Index Finger) | Draw                     |
| Closed Fist                  | Erase                    |
| V Sign ✌️                    | Toggle Black/White Color |
| Brush Size Slider            | Adjust Stroke Width      |
| Clear Drawing Button         | Clear Canvas             |

## 🛠️ Technologies Used

* HTML5
* CSS3
* JavaScript (Vanilla JS)
* Media Pipe Hands
* Canvas API
* Webcam API (getUserMedia)

## 📂 Project Structure

```text
gesture-paint-ultra/
│
├── index.html
├── README.md
└── assets/
```

## 🚀 Installation

### Clone Repository

```bash
git clone https://github.com/Devesh-Gawai/web-practice-project.git
```

### Open Project

Navigate to the project folder and open:

```text
gesture-paint-ultra/index.html
```

Or run a local server:

```bash
python -m http.server 8000
```

Then visit:

```text
http://localhost:8000
```

## 🌍 GitHub Pages Deployment

This project is already deployed and accessible at:

```text
https://devesh-gawai.github.io/web-practice-project/gesture-paint-ultra/index.html
```

To deploy your own version:

1. Fork or clone the repository.
2. Push your changes to GitHub.
3. Go to Repository Settings → Pages.
4. Select:

   * Deploy from a branch
   * Branch: main
   * Folder: /root
5. Save changes and wait for deployment.

## ⚡ Performance Optimizations

* Single-hand tracking
* Reduced model complexity
* Landmark smoothing
* Efficient canvas rendering
* Optimized 30 FPS webcam stream

## 🔮 Future Improvements

* Multiple brush colors
* Save drawing as image
* Undo/Redo support
* Gesture-based color palette
* Multi-hand interaction
* Mobile gesture optimization
* PWA support

## 🤝 Contributing

Contributions, issues, and feature requests are welcome. Feel free to fork the repository and submit a pull request.

## 👨‍💻 Author

Developed by **Devesh Gawai** using MediaPipe Hands and modern web technologies for real-time gesture-based drawing experiences.
