# ML-Open-Loop-Optimization-of-TC-Lab
This project was done in collaboration with Caleb Rosa and Jason Rabinowitz in Alexander Dowling's class, Data Analytics Optimization and Control in the University of Notre Dame CBE Department.
This is a Python notebook that collects data for the TC Lab and creates an LSTM neural network model to perform open loop optimization on the system.
In order to run this notebook you will need your own TC Lab and need to run this in the python environment described in the Notre Dame CBE Controls Syllabus excerpted below (https://ndcbe.github.io/controls/Readme.html).

    Software Installation Instructions:
    
    Install anaconda: https://www.anaconda.com/
    Mac users: if you have a computer with an M1, M2, M3, or M4 processor, please choose “Apple Silicon”
    Windows users: install LaTeX (https://miktex.org/download) or add miktex to the end of the above command
    Mac users: install LaTeX (https://tug.org/mactex/mactex-download.html)
    Linux users: install LaTeX via your package manager
    
    Opening Anaconda:
    Windows users: in the Start menu, search search for “Anaconda prompt”. Open it and copy-paste-run the commands below
    Mac users: press command + space, then search for “terminal”. Open it and copy-paste-run the commands below
    
    In the terminal/prompt, type:
    conda create -n controls -c anaconda -c conda-forge -c IDAES-PSE python=3.10 pandas numpy matplotlib scipy jupyterlab nb_conda_kernels pandoc nbconvert-pandoc idaes-pse
    
    Next, in the terminal type:
    conda activate controls (activates the new environment)
    idaes get-extensions (installs optimization solvers)
    pip install tclab (installs TCLab software)
    
    To start using Python, in either the Acaconda promptly (Windows) or terminal (Mac):
    Activate our environment: conda activate controls
    Launch Jupyter lab: jupyter lab
    
    In the upper right corner, click on “Kernel” and change to “controls”
    You are now ready to test the TCLab hardware!
    
    Advanced Users macOS users who would like to use Ipopt without adding import idaes may need to add the following line to their .bashrc file:
    export DYLD_LIBRARY_PATH="$DYLD_LIBRARY_PATH:/Users/yourname/.idaes/bin" export PATH="$PATH:/Users/yourname/.idaes/bin
    Replace yourname with your username. You can likely skip this step.
