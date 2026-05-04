# Drug-Diffusion-Simulation-MATLAB
3D Biomedical Data Visualization using MATLAB

PK + 3D Diffusion 

MATLAB LINK : https://youtu.be/xU2DuzuOn7k

clc;
clear;
close all;

% Sample medical data
blood_pressure = [120 130 125 140 135 150 128 132 145 138];
glucose        = [90 110 100 130 125 140 95 105 135 120];
cholesterol    = [180 200 190 220 210 230 185 195 225 205];

% 3D scatter plot
figure;
scatter3(blood_pressure, glucose, cholesterol, 80, cholesterol, 'filled');

grid on;
xlabel('Systolic Blood Pressure');
ylabel('Glucose Level');
zlabel('Cholesterol');
title('3D Scatter Plot of Patient Medical Data');
colorbar;
view(45, 30);
