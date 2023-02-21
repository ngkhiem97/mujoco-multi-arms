# mujoco-multi-arms

Demonstration of multi-arms with MuJoCo.
![](gen3_multi_arms.gif)

This Python project uses MuJoCo simulation to control **two** [six degrees of freedom Gen3 robotic arm](https://www.kinovarobotics.com/product/gen3-robots) with pick-and-place action. For instructions on running the program, please see below.

Multi-arm simulation with MuJoCo involves simulating the dynamics of multiple robotic arms in a virtual environment. MuJoCo, or the Multi-Joint Dynamics with Contact physics engine, is a powerful tool for simulating the behavior of complex mechanical systems, such as robots. With MuJoCo, users can create virtual environments with a high degree of fidelity, allowing for accurate predictions of the behavior of multiple robotic arms interacting with one another and their environment. By adjusting parameters such as joint stiffness and friction, users can explore the impact of different physical properties on the behavior of the arms. This type of simulation is valuable for both research and engineering applications, as it allows for the testing and refinement of robotic control algorithms in a safe and controlled environment.

## Install requirements

```bash
pip install -r ./requirements.txt
```

## Start demo on a specific action

```bash
cp -R ./gen3 /tmp
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/home/khiem/.mujoco/mujoco210/bin
export LD_LIBRARY_PATH=$LD_LIBRARY_PATH:/usr/lib/nvidia
export LD_PRELOAD=/usr/lib/x86_64-linux-gnu/libGLEW.so
python3 ./gen3_multi_arms.py
```

## Acknowledgement

This repository is developed from [Dr. Cui](https://www.jindacui.com/bio) source code.
