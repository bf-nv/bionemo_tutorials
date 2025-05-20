# Tutorial: Using NVIDIA BioNeMo NIMs for Virtual Screening

This tutorial demonstrates how to use **NVIDIA BioNeMo NIMs** (NVIDIA Inference Microservices) hosted on NVIDIA computing infrastructure for virtual screening tasks.

This virtual screening workflow for drug discovery combines three key steps: protein folding using ESMFold, controlled generation of small molecules with molmim, and docking those molecules into a target protein using DiffDock.

## Getting Started

1) **Generate an `API_KEY`** <BR>
   Visit [https://build.nvidia.com/explore/discover](https://build.nvidia.com/explore/discover) to create your `API_KEY`.

2) **Set Up in Google Colab** <BR>
   Copy and paste your `API_KEY` into the Google Colab environment as instructed.

3) **Run the Tutorial Notebooks** <BR>
   Execute the three provided Jupyter Notebooks sequentially, following the step-by-step instructions included in each IPYNB.

## Details

1) **Setting up an `API_KEY`** <BR>
a) Visit [https://build.nvidia.com/explore/discover](https://build.nvidia.com/explore/discover) to create your `API_KEY`.<BR>
b) Click "Biology" in the left-hand menu (highlighted in orange below): <BR>
<img src="assets/01_Build_DiscoverySection.png" alt="Alt text" width="300"> <BR>   
c) Under the "Generative Virtual Screening" heading, click on the right arrow (highlighted in orange below) to find the "molmim" application: <BR>
<img src="assets/03_GenerativeVirtualScreen.png" alt="Alt text" width="300"> <BR>
d) Click the "Deploy" tab in the center of the page, then click on the "Get API Key" button (highlighted in orange below): <BR> 
<img src="assets/04_MolMIM.png" alt="Alt text" width="300"> <BR>
e) In the pop-up window, enter your email address to receive free credits for using NVIDIA NIMs, then click "Next" (highlighted in orange below): <BR>
<img src="assets/05_SignIn_NV_NIM.png" alt="Alt text" width="300"> <BR>
f) Follow the instructions to either: 1) log in; or 2) create a free NVIDIA Developer account. <BR>
<img src="assets/gen_API_key.png" alt="Alt text" width="300"> <BR>
g) When your `API_KEY` appears, click the button next to it to copy the key (highlighted in orange stroke below): <BR> 
<img src="images/copy_key.png" alt="Alt text" width="200"> <BR>

2) **Adding the `API_KEY` to Your Jupyter Notebook Colab**
\- Click "Open in Colab" next to `Step_1_Predict_target_protein_structure.ipynb` in section **2. Run Jupyter Notebooks** to open it in Colab.  
\- Click key button in the left-hand menu, turn on "Notebook access", put "API_KEY" under "Name", and paste the API Key under "Value" (highlighted with orange strokes below):    
<img src="images/colab_copy.png" alt="Alt text" width="300">  
\- Now you're ready to run the three Jupyter notebooks one-by-one.  
\- **Note that the API Key might expire after 24 hours. If it no longer works, please repeat the above steps to generate a new API Key.**

2) **Running the Jupyter Notebooks in Colab**
### 2. Run Jupyter Notebooks
Step_1_Predict_target_protein_structure.ipynb [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hw-ju/bionemo_nim/blob/main/Step_1_Predict_target_protein_structure.ipynb)

Step_2_MolMIM_controlled_generation.ipynb [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hw-ju/bionemo_nim/blob/main/Step_2_MolMIM_controlled_generation.ipynb)

Step_3_Predict_docking_poses.ipynb [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/hw-ju/bionemo_nim/blob/main/Step_3_Predict_docking_poses.ipynb)
