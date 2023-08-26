# Background Removal with Azure AI Vision and Gradio

![Example image](https://github.com/ppiova/AIVision-ImageRetrieval/blob/main/images/Gradio-RemovalBackground.gif "GradioDemmo")

This project uses Azure AI Vision to remove the background from images and visualize the results using a Gradio web interface. The user can upload an image to the Gradio web interface, and the backend service will remove the background from the image and return both the processed image and its corresponding mask.

## Requirements

- Python 3.6+
- Azure Subscription
- Azure AI Vision Service

## Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/YourRepo/YourProject.git
    ```
   
2. **Change to project directory**
    ```bash
    cd YourProject
    ```

3. **Open Visual Studio Code and create a Python environment**  
   Press `Ctrl+Shift+P` and select `Python: Select Interpreter` followed by `Python: Create New Environment`.

4. **Install the required packages**
    ```bash
    pip install gradio
    pip install requests
    pip install python-dotenv
    pip install pillow
    ```

5. **Set Environment Variables**  
   Create an `.env` file in the root folder named `azure.env`. In this file, set your Azure AI Vision API key and endpoint:
    ```
    azure_cv_key=YOUR_AZURE_CV_KEY
    azure_cv_endpoint=YOUR_AZURE_CV_ENDPOINT
    ```

## Running the Web App

1. **Run the main Python script**  
   Start the Gradio web interface by running the Python script:
    ```bash
    python your_script_name.py
    ```

2. **Access Web Interface**  
   Navigate to the URL provided in the console to access the web interface.

3. **Upload and Process**  
   Upload an image and click "Submit" to remove the background.

## Code Structure

- `post_request`: Function for sending POST requests to Azure.
- `remove_background_from_image`: Main function to remove background from an image.
- **Gradio UI**: Code to set up the Gradio web interface.

## Sample Images

You can use the sample images (`piova-01.jpg`, `piova-02.jpg`, etc.) provided in the `images` directory to test the background removal.
