# Adaptive PID Control System
https://github.com/lawaty/CV-Libraries

## Overview
Generally, Control system is used to generate a signal that overcomes error and achieves some desired state like moving the ROV a certain distance in a certain direction. PID control system is an optimized control system that takes the environment effect into consideration to face it as possible. Unfortunately PID systems are tightly bound to environments that changing the environment intensity results in system disturbance and accordingly system redesign becomes a must for every single environment. Adaptive PID system is a further improvement for the control system that allows the pid system to adapt to different environments without human interaction.

## My Role
1. PID Main System Design & Implementation
2. PID Adaption Design & Implementation

## Technologies & Specifications
1. `Python` Script
2. `OpenCV` image processing library

## Features
1. `Setup & Running modes`  
    Setup mode allows the PID script to keep tuning its values continuously till `fit state` is achieved based on some `fitness evaluation`