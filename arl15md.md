# Mission Design

## Motivation 
 In a movie <Iron man 3>, many high-technologies developed by Tony Stark are described. The most amazing invention is, we think, ‘JAVIS’ the AI computer. JAVIS, Tony Stark’s computer assistant, often seems much more powerful than human brain. Our team members interested in one of its function and especially paid attention to a scene below.
 
 
 ‘Happy’ who was one of Tony’s friend seriously injured by an unknown enemy. Tony and JAVIS analyze this scene of accident ‘in their laboratory’. His AI computer shows him the site in three-dimensional hologram. From the image, Tony figures out some important clues of criminal.  Before that, how did JAVIS take the 3D image of the place?
 The solution is in our eyes. Everyone knows that human has 2 eyes. Each eye gets two-dimensional image of some objects. We don’t know how far the objects are with this image separately. Our brain, however, can combine these two images taken by both sides of eyes and figure out approximate distance. The x-position of two images differs for a distance between two eyes. The brain senses this difference. 
  
 Our satellite, similarly, has two cameras called stereo camera. So, a main computer of it takes two pictures per one shot. As these two cameras are separated each other, there is difference of x-position on the pictures. As we can measure this difference of angle (theta) and distance between cameras, it is possible to calculate how far some points on object are. After combining this points, we can get 3D image of the surface of it.
 Furthermore, our satellite has GPS and compass sensor. They stores its location and direction for every single shot. Then, a main computer of it calculates position of rendered objects on ground. The computer develops one solid surface from a pair of right and left images with the process. Finally, it combines these respective surfaces in same coordinate system to 3D map.  

## 3. Mission process
### 3.1 First mission
The main mission of the ARLISS competition is arriving at a goal point the satellite itself without any manual control. The goal is located on middle of the black rock desert in US, Nevada. We enter a GPS coordinate of the location into the satellite in advance. After landing, the rover decides where to go and drives to the goal itself.

3.2 Second mission
 When the satellite arrives at goal, it moves on to a second mission. The second mission is taking pictures and storing GPS and compass data with it around the final point. It will render the surroundings with these data and develop complete three-dimensional image of the site.

## 4. Possibility
---
### 4.1 Pathfinder
The satellite can calculate the distance to an objects from a single shot of the stereo camera. Therefore, it knows geographical features in front of it and can find where obstacles are. This means that our explorer is able to cognize which path is the best. It helps the rover to drive into the destination successfully.

### 4.2 Exploration
If the satellite is used for exploring an unknown planet surface, it can build up 3D maps from terrain features. The map has more detailed information than 2D. Explorers and scientists can figure out where is the best spot for base camp, landing spot or etc.

## 5. Success Criteria
1.  To bring a completed (satisfying all system requirements) satellite to a lunching site without any damage.
2. To successfully arrive into radius 5m around a goal point.
3. To build up 3D map 10m around the goal point with stereo camera images taken by the satellite. 
