# 21cmFAST GPU Implementation and Optimisation

## 1 Outline of work on CPU code

All template calculations are set up for systematic
comparison of the compiler options.

github/claude-4-nt2-performance

## 2 Outline of work on GPU code

All GPU code builds without the `ninja` hack
from last week. Full GPU calculations are running.

These branches have the GPU work:

`github/claude-3-oz2-check_cuda`

`github/claude-4-oz2-performance`

and in install/21cmFAST/gpu-build-v4

`github/adacs-gpu-build-v5rc`

## 3 Timings for template example CPU calculations

An illustration of timinngs for a wide range of template jobs.

execution_times_small.o2.run0_small.o2.native.run1_small.ofast.run2_small.ofast.native.run3.png

This will have GPU data too.

## 4 Example profile for a CPU job

Illustration of a profile.

profile_simple-coeval-small.png

## 5 Timings for a template GPU job

GPU timings on different CPUs so not yet on the same plot as the CPU data.

execution_times_park19.gpu.run0.png

## 	6 Work on the GPU branch is in this fork

https://github.com/gusgw/21cmFAST  adacs-gpu-build-v5rc

## 7 The example jobs with build, run, and measure scripts are here

https://github.com/ADACS-Australia/YQin2025b-21cm
