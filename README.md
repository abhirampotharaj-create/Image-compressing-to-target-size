# Image-compressing-to-target-size

A simple, lightweight Python utility script to compress heavy mobile videos (`.mp4`) using the widely compatible **H.264 video codec** and **AAC audio codec**. It utilizes **FFmpeg's Constant Rate Factor (CRF)** to optimize the video file size while maintaining excellent visual quality, preserving essential metadata (such as video rotation from mobile captures).

## 🚀 Quick Setup: Downloading & Installing FFmpeg

To run this script, FFmpeg must be accessible via your system's command line interface. Follow these setup steps:

### 1. Download FFmpeg
* **Windows:** Go to [Gyan.dev](https://www.gyan.dev/ffmpeg/builds/) and download the **ffmpeg-release-essentials.zip** compilation.
* **macOS:** Install via Homebrew: `brew install ffmpeg`
* **Linux:** Install via apt: `sudo apt update && sudo apt install ffmpeg`

### 2. Configure Environment Variables (For Windows Users)
To allow the Python script to find FFmpeg automatically from anywhere on your computer without modifying the code, add it to your System PATH:
1. Extract the downloaded `.zip` file into a folder (e.g., `C:\ffmpeg`).
2. Copy the path to the `bin` folder (e.g., `C:\ffmpeg\bin`).
3. Press the Windows Key, search for **"Edit the system environment variables"**, and click it.
4. Click the **Environment Variables...** button at the bottom right.
5. Under *System Variables*, find and select **Path**, then click **Edit**.
6. Click **New** and paste your path to the `bin` folder (e.g., `C:\ffmpeg\bin`).
7. Click **OK** on all windows to save and apply.
8. Open a **new** Command Prompt or Terminal and type `ffmpeg -version` to verify it works!

---

## 🛠️ Requirements & Installation

1. Clone or download this repository to your local machine.
2. Install the required Python wrapper library using pip:
   ```bash
   pip install ffmpeg-python
