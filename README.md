# Google-earth-optimization-Algorithm
This repository will help us to understand google earth shortest distance algorithm and how can we optimize it in convex polygon and circle.
Lets first understand your aim by taking a simple example. You are given an array trees where trees[i] = [xi, yi] represents the location of a tree in the garden.
You are asked to fence the entire garden using the minimum length of rope as it is expensive. The garden is well fenced only if all the trees are enclosed.
Aim is find the coordinates of trees that are exactly located on the fence perimeter.

This function is similar to distance finding in google earth(min dis). We achieve your goal by using Jarvis March convex hull algorithm. In optimization we can use Graham Scan algorithm ( Time omplexity ----> O(n * log n)
