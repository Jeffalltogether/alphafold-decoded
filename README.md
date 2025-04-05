# AlphaFold Decoded

This project aims to provide an easy-to-understand implementation of AlphaFold, designed for educational purposes. Rather than filling in small gaps in an existing codebase, this project guides users through building AlphaFold entirely from scratch. The repository is structured with a series of Jupyter Notebooks or Python files containing interactive explanations, coding exercises, and TODO markers to support hands-on learning.

A companion [YouTube series](https://youtube.com/playlist?list=PLJ0WcPQS7xJVJr6ceIPFSkAGAgrkmw1c9&si=GUj4NePZ2i2ZnTBY) is available, offering detailed walkthroughs and explanations of each concept and implementation step.

## Project Description

AlphaFold revolutionized the field of protein structure prediction. This project breaks down AlphaFold's complex processes into manageable steps. Users will actively participate in the implementation process by:

* Filling out missing code sections within provided Jupyter Notebooks or Python files.
* Following the guidance of TODO markers.
* Referencing solution files for assistance and to check their work.

## Folder Structure

* **tutorials:** Houses Jupyter Notebooks and Python files containing interactive exercises designed to guide users through implementing all AlphaFold components. 
* **solutions:** Provides solutions to the coding exercises.  

## Setup Instructions

**Choose the method that works best for you:**

### Working with Colab (Recommended for beginners)

Colab provides a fast and easy way to get started with the tutorials, especially if you don't have a powerful GPU. You can even access a GPU within Colab for the final prediction steps.

1. **Upload the 'tutorials' folder to Google Drive.**

2. **Activate Colab in Google Drive:**
   * Go to My Drive -> More -> Connect more Apps
   * Search for "Colaboratory" and install it

3. **Open a tutorial notebook in Colab:**
   * Navigate to the `.ipynb` file of the tutorial you want to run in your Google Drive.
   * Right-click the file and select Open with -> Colaboratory 

4. **Grant permissions when prompted.**

5. **Enable GPU (optional):**
   * If the tutorial requires a GPU, go to Runtime -> Change Runtime Type -> Select "GPU" and save.

6. **Set your folder path (first cell):**
   * In the first code cell of your notebook, you'll likely see a line to set the `folder_name`. Update this with the correct path to your 'tutorials' folder in Google Drive.  

### Local Setup (For advanced users) 

If you're an advanced user and prefer working in your own local environment, follow these steps:

1. **Install a Package Manager (if needed):**
   * **Conda:** If you have Conda, proceed to the next step.
   * **Mamba:** For faster setup, install Mamba ([https://mamba.readthedocs.io/en/latest/](https://mamba.readthedocs.io/en/latest/)).

2. **Install Dependencies**
   * **Select the right environment file:**
      * `environment_cpu.yml` (no GPU) 
      * `environment_cuda.yml` (NVIDIA GPU)
      * `environment_mac.yml` (Mac systems)  
   * **Install using Conda or Mamba:**
      ```bash
      # With Conda:
      conda env create -f environment_cpu.yml  # Or environment_cuda.yml/mac.yml

      # With Mamba:
      mamba env create -f environment_cpu.yml  # Or environment_cuda.yml/mac.yml
      ```

3. **Activate the Environment:**
   ```bash
   conda activate alphafold
   ```

4. **Launch Jupyter Notebook and Select Kernel:**
   * Start Jupyter Notebook from the 'tutorials' folder.
   * In text editors like VS Code, set the workspace setting "Jupyter: Notebook File Root" to 'tutorials'.
   * Open a tutorial, ensuring the kernel name matches your environment ('alphafold').


## Working on the Tutorials
The tutorials should be completed in the following order:

1. Tensor Introduction
2. Machine Learning Introduction
3. Attention
4. Feature Extraction
5. Evoformer
6. Feature Embedding
7. Geometry
8. Structure Module
9. Model

If you are already familiar with tensors and machine learning, feel free to start at Attention.
