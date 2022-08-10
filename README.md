# SPIRAL v1.0
SPIRAL is a method for batch effect removing and coordinationg alignment for spatially resolved transcriptomes.  
![image](https://user-images.githubusercontent.com/17848453/183861675-b8b63081-83f3-4957-a3f8-0b822a4980cd.png)
# Usage
SPIRAL consistis two consective modules  
* **SPIRAL-integraion**    
 * Input  
   feature mat: Ncell x Ngene    
   edge mat: Nedge x 2    
   meta mat: Ncell x 2: domain label and batch label  
* Output  
   embeddings: Ncell x zdim  
   recovery gene expression: Ncell x Ngene  
* **SPIRAL-alignemnt**  
 * Input    
   embeddings of SPIRAL-integration: Ncell x zdim  
   clusters  
 * Ouput  
   aligned coordinates: Ncell x 2  
* **Demo can be obtained in Run_Spiral.ipynb**
# Installing
git clone https://github.com/guott15/SPIRAL.git  
cd SPIRAL  
python setup.py build  
python setup.by install  
#### Note: pytorch_revgrad should be in your current path.
