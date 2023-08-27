# Background Removal with Azure AI Vision and Gradio

![Example image](https://github.com/ppiova/AIVision-ImageRetrieval/blob/main/images/Gradio-RemovalBackground.gif "GradioDemmo")

This Jupyter Notebook uses Azure Computer Vision to remove the background from images and visualizes the results using a Gradio web interface. Users can upload an image through the Gradio interface, and the service will return the image with the background removed as well as a mask of the object.

## Requirements

- Python 3.6+
- Azure Subscription
- Azure Computer Vision Service
- Jupyter Notebook

## Installation

1. **Clone the repository**
    ```bash
    git clone https://github.com/YourRepo/YourProject.git
    ```
   
2. **Change to project directory**
    ```bash
    cd YourProject
    ```

3. **Install the required packages**
    ```bash
    pip install gradio
    pip install requests
    pip install python-dotenv
    pip install pillow
    ```

4. **Set Environment Variables**  
   Create an `.env` file in the root folder named `azure.env`. In this file, set your Azure AI Vision API key and endpoint:
    ```
    azure_cv_key=YOUR_AZURE_CV_KEY
    azure_cv_endpoint=YOUR_AZURE_CV_ENDPOINT
    ```

## Running the Web App in Jupyter Notebook

1. **Open the Jupyter Notebook file (`your_notebook_name.ipynb`).**
   
2. **Navigate to the cell that contains the Gradio web interface code.**
   
3. **Run the cell to launch the Gradio web interface.**

A URL will appear in the output section below the cell. Click on it to access the web interface.

## Code Structure

- `post_request`: Function for sending POST requests to Azure.
- `remove_background_from_image`: Main function to remove background from an image.
- **Gradio UI in Jupyter Notebook**: Code to set up the Gradio web interface within the notebook.

## Sample Images

You can use the sample images (`piova-01.jpg`, `piova-02.jpg`, etc.) provided in the `images` directory to test the background removal.


## Sample Images

You can use the sample images (`piova-01.jpg`, `piova-02.jpg`, etc.) provided in the `images` directory to test the background removal.

## Additional Resources

For more code examples and use-cases, feel free to check out this repository by Serge Retkowsky on removing background using Azure Computer Vision:

[Removing Background Using Azure Computer Vision by Serge Retkowsky](https://github.com/retkowsky/Removing-background-using-Azure-Computer-Vision-4)

This repository can serve as an additional resource for enhancing and expanding your own projects.

