## ⚽ Offside Detection using Computer Vision
## 🎯 Problem:

In football matches, accurately determining offside in real-time is a significant challenge for referees. Some situations can remain unclear even after replays.

## 👨‍💻 Solution:

We developed a tool that uses computer vision to automatically detect offside by calculating the players' positions relative to the end line of the pitch and identifying the player closest to this line.

## 🧠 How Does the System Work?
We analyze the image using OpenCV algorithms, following these steps:

**Line Detection:** We use Canny edge detection and Hough Transform to identify the lines on the field, focusing on the penalty box line or the end line as a reference.

**Player Detection:** We rely on Haar Cascades to detect the players' positions.

**Finding the Nearest Player:** We calculate the vertical distance between each player and the reference line.

**Visualizing the Results:** We draw each player with a line to the nearest point on the reference line, sorting them by distance.

🔍 The player closest to the end line is considered the key factor in determining offside.

## 🛠️ Tools Used

Python

OpenCV

NumPy

Google Colab (for quick testing)

## 🖼️ Sample Output:


<p align="center"> <img src="output-image.png" alt="Sample Output" width="500"/> </p>
⚙️ How to Use


## Install the required dependencies:

bash
Copy
Edit
pip install -r requirements.txt
Run the code from the src/ folder:

bash
Copy
Edit
python src/detect_offside.py


## 🎨 UI/UX Design
You can browse the full design on Figma: Link to Figma

## 🤝 Team Members
Yousef Alabri – AI Developer

