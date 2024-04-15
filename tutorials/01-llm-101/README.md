Using Jupyter on my laptop using an ANL GPU machine connected to the ANL VPN.

Assumes the conda command is in your path on the ANL GPU machine. 

(base) Toms-MacBook-Pro:~ brettin$ ssh -L 8999:localhost:8999 rbdgx2.cels.anl.gov
conda create -p /rbscratch/brettin/conda_envs/llm_apis python=3.12.2
(base) brettin@rbdgx2:~$ conda activate /rbscratch/brettin/conda_envs/llm_apis
(/rbscratch/brettin/conda_envs/llm_apis) brettin@rbdgx2:~$ conda install jupyter


(/rbscratch/brettin/conda_envs/llm_apis) brettin@rbdgx2:~$ pip install langchain openai






(/rbscratch/brettin/conda_envs/llm_apis) brettin@rbdgx2:~$ jupyter notebook --no-browser --port 8999

paste localhost URL into browser.

i.e. http://localhost:8999/tree?token=675c4b6d67c673dbb60e0d4431db07252ee1e876ca95e54e
