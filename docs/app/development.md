# Develop on BBB

### Prepare VENV

```bash
mkdir ~/boneio_development
python3 -m venv ~/boneio_development/venv
source ~/boneio_development/venv/bin/activate
cd ~/boneio_development
git clone https://github.com/boneIO-eu/app_bbb.git
```

In below instruction I assume you still in activated venv.

```
source ~/boneio_development/venv/bin/activate
```

### Install Dependencies

```bash
cd app_bbb
pip3 install -r requirements.txt
pip3 install -e .
```

### Run tests on board

```bash
cd tests
python3 relay_32_5.py
```
