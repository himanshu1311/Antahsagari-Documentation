## INTRODUCTION

The acronym stands for Simultaneous Localization and Mapping. Let’s understand it with an example. Tushar is kidnapped and left in a dense forest by his enemies. He has no phone so he can’t communicate with anyone nor has accessibility to navigation tools like google maps or compass. Luckily there is abundant food in the forest. Now what he should do? 
There are broadly two possibilities - one is he accepts his fate and spends the rest of his life in the forest. The other option is that he figures out a way to get out of the forest. Talking about Tushar he has a good presence of mind and always keeps a pocket diary and a pen in his secret pocket. He starts from a place and notes down the distinguishable landmarks(features). Like Stones, trees, etc. of forest in his diary. Whenever he sees a new feature, he adds it in his diary. He is moving completely arbitrarily but carefully and consciously. Many times he encounters the same path giving him a strong hint about  connectivity between different paths . In some days he figures out a rough map of the forest with the help of which he rushes out of the forest.

Now what Tushar did above was the concept of feature-based SLAM. In technical terms, SLAM is the computational problem of constructing or updating a map of an unknown environment while simultaneously keeping track of an agent's location within it. It’s like a chicken-egg problem. You can build a map only if you know your absolute location at each point of the environment and if you want to determine your location in a surrounding you should have a pre-built map of the surrounding. But luckily we have certain algorithms for SLAM.


### Why feature-based SLAM is not suited for underwater environments

One of the most important factors for SLAM is the landmarks. Due to the unstructured characteristics of the environment, in most cases, there are no distinct objects or features. The turbidity disturbs the operation of sensors, particularly those based on light such as cameras and lasers.




