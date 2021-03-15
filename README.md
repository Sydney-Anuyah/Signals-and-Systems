% #Signals-and-Systems
%Design of Signals and Systems code for first year university students. The code is done in matlab.
%

%Problem 1A
%Let us plot a discrete time sinusoid 𝑥[n] = sin[Ωo * n]. 
% Ωo = - pi/4.
%First we have to define the independent variable axis [n] in our script:
% Ωo is Omega0 in our script
clear all; 
close all;
clc;

%1a

n = 0:10;
% This creates an array of 11 digits from 0 to 10.
% These variables will form the independent axis

Omega0 = -pi/4;
%For the value of x[n], we must find the value of omega as given in the
%question

xn = sin (Omega0 *n);

%After representing omega, we can now calculate the value of the amplitude
%of each value on the dependent axis using what we have obtained from the
%independent axis.

figure;
%This brings out an empty figure sheet for diagrams.

stem (n, xn)
%stem(X,Y) plots the data sequence Y at the values specified in X
%Discrete sequence or "stem" plot. stem(Y) plots the data sequence Y as stems from the x axis terminated with circles for the data value. 


xlabel('Time \itn'); 
%labels the x axis
ylabel('\itx\rm[\itn\rm] = sin(\Omega_{0}\itn\rm)');
%labels the y axis
title('Task 1, Part (a), \Omega_{0} = -\pi/4');
%Titles the graph

%The command \it makes the text that follows it 
%italics and \rm returns the text to normal. 

%PLOTTING THE CONTIONUS TIME SIGNAL

t = 0:0.01:10;
%Creates an array ot t from 0 to 10 with an interval of 0.01
xn_ct  = sin(Omega0 *t)
%For a value of t, a contionous value of xn was created.

figure; 
hold on;

%hold ON holds the current plot and all axis properties, including 
%the current color and linestyle, so that subsequent graphing commands
%add to the existing graph without resetting the color and linestyle.


%
%
%
%
%

