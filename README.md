# Google-earth-optimization-Algorithm
This repository will help us to understand google earth shortest distance algorithm and how can we optimize it in convex polygon and circle.
Lets first understand your aim by taking a simple example. You are given an array trees where trees[i] = [xi, yi] represents the location of a tree in the garden.
You are asked to fence the entire garden using the minimum length of rope as it is expensive. The garden is well fenced only if all the trees are enclosed.
Aim is find the coordinates of trees that are exactly located on the fence perimeter.

![2021-08-13 (2)](https://user-images.githubusercontent.com/88893810/129377564-c94fed72-7663-4acb-bab1-3f0b84a5f84e.png)

![2021-08-13 (4)](https://user-images.githubusercontent.com/88893810/129377789-f6eb2540-5b5a-485b-8407-9d93222fa432.png)

![2021-08-13 (9)](https://user-images.githubusercontent.com/88893810/129377901-1d713f03-47dd-400f-9f8e-0f736d2c8ea9.png)

![2021-08-13 (10)](https://user-images.githubusercontent.com/88893810/129377942-a58ead59-040a-44b2-b037-dde0056a5626.png)


This function is similar to distance finding in google earth(min dis). We achieve your goal by using Jarvis March convex hull algorithm. In optimization we can use Graham Scan algorithm ( Time omplexity ----> O(n * log n)

![2021-08-13 (12)](https://user-images.githubusercontent.com/88893810/129378036-cc2d884b-5cff-40bf-bf6e-e303365a7893.png)
