# Computer-vision-And-ML-Technical-Task
A real-time object tracking system using Python and OpenCV. Users select an object in the webcam feed using a bounding box, and the system tracks it live using CSRT or other OpenCV trackers. Includes reset and quit options. Fast and easy to use with multiple tracker support.
# Real-Time Object Tracker - Eyego Intern Task
A comprehensive real-time object tracking system built with OpenCV for the Eyego ML and Computer Vision Intern position. This system allows users to interactively select objects in a webcam feed and track them in real-time using state-of-the-art computer vision algorithms.

## 🎯 Project Overview
This project implements a robust real-time object tracker that meets all the specified requirements:

- ✅ **Interactive Object Selection**: Click and drag to select objects using bounding boxes
- ✅ **Real-Time Tracking**: Smooth, low-latency tracking in live webcam feed
- ✅ **Visual Feedback**: Professional UI with tracking status, performance metrics, and controls
- ✅ **Multiple Algorithms**: Support for various tracking algorithms (CSRT, KCF, BOOSTING, MIL, MOSSE)
- ✅ **Performance Analysis**: Built-in benchmarking and comparison tools

## 🚀 Quick Start

### Prerequisites

- Python 3.7 or higher
- Webcam or camera device
- Operating System: Windows, macOS, or Linux

### Installation

1. **Clone or download the project files**

2. **Install dependencies:**
   \`\`\`bash
   pip install -r scripts/requirements.txt
   \`\`\`

3. **Run the tracker:**
   \`\`\`bash
   python scripts/real_time_tracker.py
   \`\`\`

### Basic Usage

1. **Start the application** - The webcam feed will open
2. **Press 's'** to select an object by drawing a bounding box
3. **Watch real-time tracking** - The system will track your selected object
4. **Press 'r'** to reset and select a new object
5. **Press 'q'** to quit

## 🔧 Technical Implementation

### Core Architecture

The system is built around the `RealTimeObjectTracker` class which provides:

```python
class RealTimeObjectTracker:
    def __init__(self, tracker_type='CSRT')
    def initialize_camera(self, camera_index=0)
    def select_object(self, frame)
    def start_tracking(self)
