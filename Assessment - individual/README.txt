Run the following in jupyter notebook to install packages required:
-----------------------------

import subprocess
import sys
required_packages = [
    'pandas', 
    'numpy', 
    'scipy', 
    'matplotlib', 
    'seaborn'
]
for package in required_packages:
    try:
        __import__(package)
    except ImportError:
        subprocess.check_call([sys.executable, "-m", "pip", "install", package])

------------------------------
