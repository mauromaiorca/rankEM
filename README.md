![rankEM]()


rankEM aims to improve 3D cryoEM map quality and resolution by scoring, validating, and selecting raw particles image data.


# Download & Compile

Pre-Install:
```
Ubuntu: apt-get install python3.8-venv
```

Get the source code:
```
git clone https://github.com/mauromaiorca/scorem.git
```

Compile:
```
cd scorem
(Remove previus installation: rm -fr build dist scorem.egg-info venv )
/usr/bin/python3.8 -m venv venv
source venv/bin/activate
/usr/bin/python3.8 setup.py bdist_wheel
/usr/bin/python3.8 -m pip install ./dist/scorem-0.1.0-cp38-cp38-linux_x86_64.whl  --force-reinstall
```



# Examples of usage

### Processing a 3D volume image

```
enhancEM virionB.mrc --o virionB_proc.mrc  --process 2.5 0.5
```
