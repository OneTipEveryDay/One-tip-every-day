 switching to a **virtual environment** is the cleanest way. Here’s the step-by-step:

---



## 🔹 1. Create a virtual environment

Pick a folder for your project, e.g. `myproject`:

```bash
mkdir myproject
cd myproject
python3 -m venv venv
```

---

## 🔹 2. Activate the environment

```bash
source venv/bin/activate
```

When active, your shell prompt will usually show `(venv)` at the start.

---

## 🔹 3. Upgrade pip (important)

```bash
pip install --upgrade pip
```

---

## 🔹 4. Install OpenCV + Matplotlib via pip

```bash
pip install opencv-python matplotlib
```

(You can also add `numpy` if not already installed.)

---

## 🔹 5. Test everything

Run:

```bash
python -c "import cv2, matplotlib; print(cv2.__version__); import matplotlib; print(matplotlib.__version__)"
```

You should see version numbers without errors 🎉

---

✅ From now on, whenever you work on your project, just run:

```bash
source venv/bin/activate
```

and Python will use the packages inside the virtual environment.

---

Do you want me to also show you how to **freeze dependencies** into a `requirements.txt` so you can reinstall the same environment easily later?
