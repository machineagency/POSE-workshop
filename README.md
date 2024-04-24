# POSE Workshop

April 25-27th, 2024

University of Washington 

This repository contains resources for the NSF sponsored Pathways to Open-Source Ecosystems for Laboratory Automation workshop.

## Schedule
Check out the full schedule [here](https://docs.google.com/document/d/1udCEEesGPzwMaFrfiGoRLxHk3sxxxjrCbfZWbAX9TOE/edit)!

## Activities
We have 6 Jubilees for groups to use over the workshop. 3 are prepped for pipetting/liquid handling, and 3 for gel 3D printing applications.

### To use the machine:
- Login to the provided laptops with the same login/password used for WiFi access, if needed
- Open a terminal prompt and enter the following commands:
```
cd POSE-workshop
source .venv/bin/activate
jupyter lab
```
- This should open Jupyter lab on the machine! If it doesn't open automatically, copy & paste the url that pops up.
- If prompted, select the `POSE-workshop` kernel in Jupyter.


If you want to install on your own machine:
- Clone this repositository recursively: `git clone --recursive https://github.com/machineagency/POSE-workshop.git`
    - Note that the `--recursive` flag is necessary as this repository relies on [science_jubilee](https://github.com/machineagency/science_jubilee/) 
- We recommend using python virtual environments to handle dependencies. To do this:
  - Move into the new directory: `cd POSE-workshop`
  - Create a virtual environment named `.venv`: `python3 -m venv .venv`
  - Activate the virtual environment: `source .venv/bin/activate` 
  - You should now see `(.venv)` to the left of your command line prompt! (If you wish to leave the virtual environment, type `deactivate` from any directory)
- Make sure you're using the latest version of pip: `python3 -m pip install --upgrade pip`
- Install the science_jubilee package: `python3 -m pip install -e ./science_jubilee`
- Add the kernel to jupyter lab: `python3 -m ipykernel install --user --name=POSE-workshop`


