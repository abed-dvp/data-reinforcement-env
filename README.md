# ⚙️ Setting up a Reinforcement Learning environment

## 🎯 Goal of this challenge

Setting up a separate environment for Reinforcement Learning.

In this unit we need a lot of new packages. Some of these packages are not compatible with the package versions we needed for other parts of the bootcamp.

So we will set up a new virtual environment. That way we have two separate python environments, and our packages will not conflict. 🦾

This is something you will often do for your projects: create dedicated virtual environments.

## 🐍 Create a new virtual environment

🐍 Create the virtual env

```bash
cd ~/code/<user.github_nickname>/{{local_path_to("06-Deep-Learning/08-GAN-and-RL/00-Reinforcement-Env")}}
cd .. # Move to the unit's main folder
python --version # First, check your Python version for <YOUR_PYTHON_VERSION> below (e.g. 3.12.9)
pyenv virtualenv <YOUR_PYTHON_VERSION> reinforcement-env
pyenv local reinforcement-env
pip install --upgrade pip
```

Then, make sure your Terminal displays `[🐍 reinforcement-env]` to the right.

## 📦 Install the packages

Navigate back to this challenge's folder:

```bash
cd ~/code/<user.github_nickname>/{{local_path_to("06-Deep-Learning/08-GAN-and-RL/00-Reinforcement-Env")}}
```

In this folder, we created a `requirements.txt` file with all the requirements for this unit's challenges. We just need to `pip install` it to have all of them:

```bash
pip install -r requirements.txt
```

In essence we are installing:
- Jupyter Notebook and all its dependencies
- Classics like Pandas and NumPy
- `gymnasium` to create reinforcement learning environments
- `stable-baselines` to run reinforcement learning algorithms
- `tensorboard` to log the results

## ✅ Check your installation

```bash
make test
```

All good? If not, ask a TA to help you.

Don't forget to commit and push your test results:

```bash
git add tests/test_output.txt
git commit -m "Completed Reinforcement Env setup"
git push origin master
```

## 🏁 Finished

You now have a fresh environment to work with LLMs.

Just remember to always check that you are using the `reinforcement-env` environment. Especially when you are using VS Code, make sure to select this new environment.
