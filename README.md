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

What if we want to choose points in form of circle.
![CentreCalculation](https://user-images.githubusercontent.com/88893810/130540076-1cd44e9c-5d55-4c1d-96d8-3cac1f6a702a.jpg)

Consider similar example to understand this case, You are given a 2D integer array trees where trees[i] = [xi, yi] represents the location of the ith tree in the garden.
You are asked to fence the entire garden using the minimum length of rope possible. The garden is well-fenced only if all the trees are enclosed and the rope used forms a perfect circle. A tree is considered enclosed if it is inside or on the border of the circle.
More formally, you must form a circle using the rope with a center (x, y) and radius r where all trees lie inside or on the circle and r is minimum.
Return the center and radius of the circle as a length 3 array [x, y, r].
![2021-08-24 (2)](https://user-images.githubusercontent.com/88893810/130540360-92f45f41-6a87-445b-ade9-8d4822adfde8.png)
trees = [[1,1],[2,2],[2,0],[2,4],[3,3],[4,2]]
Output: [2.00000,2.00000,2.00000]
Explanation: The fence will have center = (2, 2) and radius = 2
![2021-08-24 (3)](https://user-images.githubusercontent.com/88893810/130540464-abdaedb6-9e3b-4ff1-a68c-7e87c0820183.png)
trees = [[1,2],[2,2],[4,2]]
Output: [2.50000,2.00000,1.50000]
Explanation: The fence will have center = (2.5, 2) and radius = 1.5
We will be using welzls algorithm, which help us find the minimum enclosing circle. 
![2021-08-24 (5)](https://user-images.githubusercontent.com/88893810/130540698-a435e10c-2c6e-4cc2-b840-97159625ca34.png)
