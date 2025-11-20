<h1>😷 Face Mask Detection System</h1>

<h2>🩵 Project Overview</h2>
<p>The <strong>Face Mask Detection System</strong> is a real-time AI application that detects whether a person is <strong>wearing a face mask or not</strong>.  
It uses <strong>OpenCV</strong> for face detection and <strong>MobileNetV2 (TensorFlow)</strong> for mask classification.</p>

<blockquote>
 <em>Example:</em><br>
If a person appears in front of the webcam, the system will classify them as <strong>"Mask"</strong> or <strong>"No Mask"</strong> and highlight their face with bounding boxes.
</blockquote>

<h2> Key Features</h2>
<ul>
  <li>* Real-time face mask detection using webcam</li>
  <li>* Detects multiple faces simultaneously</li>
  <li>* High accuracy using MobileNetV2 CNN</li>
  <li>* Visual feedback with bounding boxes and labels</li>
  <li>* Easy to extend for custom datasets</li>
</ul>

<h2> System Workflow</h2>
<ol>
  <li>Train the MobileNetV2 model using <code>train_model.py</code> (or use pre-trained weights).</li>
  <li>Run <code>detect_mask.py</code> for real-time detection:</li>
  <ul>
    <li>Capture frames from the webcam</li>
    <li>Detect faces using OpenCV</li>
    <li>Classify each face as <strong>Mask</strong> or <strong>No Mask</strong></li>
    <li>Display results with bounding boxes and labels</li>
  </ul>
</ol>

<h2> Technologies Used</h2>
<table>
<tr><th>Category</th><th>Tools / Libraries</th></tr>
<tr><td>Programming Language</td><td>Python 3.10</td></tr>
<tr><td>Deep Learning Framework</td><td>TensorFlow, Keras</td></tr>
<tr><td>Face Detection</td><td>OpenCV</td></tr>
<tr><td>Model Architecture</td><td>MobileNetV2 CNN</td></tr>
<tr><td>Data Handling</td><td>NumPy, Pandas</td></tr>
<tr><td>Visualization</td><td>OpenCV</td></tr>
<tr><td>IDE</td><td>VS Code</td></tr>
</table>

<h2> Project Folder Structure</h2>
<pre>
FaceMaskDetection/
│
├── train_model.py           # Train the CNN/MobileNetV2 model
├── detect_mask.py           # Run real-time detection
├── mask_detector.model      # Pre-trained model weights (after training)
├── dataset/                 # Training dataset
├── requirements.txt         # Dependencies list
└── README.md                # Project documentation
</pre>

<h2> Installation & Setup (Windows)</h2>

<h3>1. Clone or Download the Project</h3>
<pre><code>git clone https://github.com/yourusername/face-mask-detection.git
cd face-mask-detection
</code></pre>

<h3>2. Open Command Prompt or PowerShell</h3>
<p>Press <strong>Windows + R</strong>, type <code>cmd</code>, and press <strong>Enter</strong>.  
Navigate to your project folder (example):</p>
<pre><code>cd C:\Users\<YourUserName>\Desktop\FaceMaskDetection
</code></pre>

<h3>3. Create a Virtual Environment</h3>
<pre><code>python -m venv venv
</code></pre>

<h3>4. Activate the Virtual Environment</h3>
<pre><code>venv\Scripts\activate
</code></pre>
<p>After activation, you should see:</p>
<pre><code>(venv) C:\Users\YourName\Desktop\FaceMaskDetection&gt;
</code></pre>

<h3>5. Install Required Libraries</h3>
<p>If <code>requirements.txt</code> exists:</p>
<pre><code>pip install -r requirements.txt
</code></pre>
<p>If not, install manually:</p>
<pre><code>pip install tensorflow opencv-python numpy pandas
</code></pre>

---

<h2> How to Run the Project</h2>

<h3>Option 1 — Train the Model (Optional)</h3>
<pre><code>python train_model.py
</code></pre>
<p>This will train the CNN/MobileNetV2 model on your dataset and save <code>mask_detector.model</code>.</p>

<h3> Option 2 — Real-time Detection</h3>
<pre><code>python detect_mask.py
</code></pre>
<p>The system will open your webcam and display:</p>
<ul>
  <li>Bounding boxes around detected faces</li>
  <li>Labels: <strong>Mask</strong> (green) or <strong>No Mask</strong> (red)</li>
</ul>

---

<h2> Example Output</h2>
<p>When running <code>detect_mask.py</code> with a webcam:</p>
<ul>
  <li>Detected faces are highlighted with bounding boxes</li>
  <li>Label indicates <strong>Mask</strong> or <strong>No Mask</strong></li>
</ul>

---

<h2> Future Improvements</h2>
<ul>
  <li>Train on larger, diverse datasets for improved accuracy</li>
  <li>Detect different types of masks (N95, cloth, surgical)</li>
  <li>Mobile app deployment using TensorFlow Lite</li>
  <li>Add alert system for public safety (notify if someone is not wearing a mask)</li>
</ul>

---

<h2> Author</h2>
<p><strong>Sasika Sewmini</strong><br>
University of Moratuwa — 3rd Year Undergraduate<br>
<a href="https://www.linkedin.com/in/sasika-sewmini-dp-829535351">LinkedIn Profile</a><br>
Email: <a href="mailto:dpsasikapeiris@gmail.com">dpsasikapeiris@gmail.com</a></p>

<p>⭐ If you like this project, give it a star on GitHub!</p>
