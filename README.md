# SELU


#### OSX:
```bash
virtualenv -p python3.6 venv
source venv/bin/activate
pip install numpy==1.12.1
pip install requests==2.13.0
pip install -r requirements.txt
pip install http://download.pytorch.org/whl/torch-0.1.11.post5-cp36-cp36m-macosx_10_7_x86_64.whl
pip install torchvision
```

### Set Up Crayon (Port: 8888) - https://github.com/torrvision/crayon
```bash
cd server
docker build -t crayon:latest -f Dockerfile .
docker run -d -p 8888:8888 -p 8889:8889 --name crayon crayon

Go to locahost:8888 for Tensorboard.
```