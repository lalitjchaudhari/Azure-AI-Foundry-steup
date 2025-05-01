# Setup on Gitbug Codespaces

Install uv:
``
curl -LsSf https://astral.sh/uv/install.sh | sh
``

## Create & activate a virtual environment: 
``
uv venv
source .venv/bin/activate
``

## Install azure dependencies 
``
uv pip install azure-identity azure-ai-projects azure-ai-inference[opentelemetry] azure-search-documents azure-ai-evaluation azure-monitor-opentelemetry
``
## Install Jupyter requirements
``
uv pip install ipykernel jupyterlab notebook
``
## Register the kernel with Jupyter
``
python -m ipykernel install --user --name=.venv --display-name="Python (.venv)"
``
## Install additional requirements (optional - for deploying repo or running mkdocs)
``
uv pip install -r requirements.txt
``

## Install Azure CLI 
``
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
``
