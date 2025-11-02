# Task description
My friend sent me this picture, the snowflakes are so beautiful. Can you figure out where is this?  
  
Flag format: v1t{latitude, longitude}  
Example: v1t{22.44385,-74.22042}

[Image](https://drive.google.com/file/d/1BDD4-_E6397He7ZUsoV0e15TRwM2tUhY/view?usp=sharing)
![[chall.png]]
# Discovery
1. Both the cars license and electrical pole indicates that we are in Japan.
2. The snow indicates that we are in the northern part of Japan possible. Confirmed by the numbering and markings of the electrical pole, that is similar to what *Hokkaido Electric Power* uses.
3. You can use the numbers on the white label to find the exact location of the pole described on this website: https://www.hepco.co.jp/network/electric_life/service/location_info/index.html
	1. ![[Pasted image 20251102142546.png]]
		1. City / Power supply area.
		2. Ward zone in city. 
		3. Neighborhood / block number.
		4. Sub block number
		5. Individual sub-block number
		6. Specific pole ID
4. By using google street view and checking some citys in the Hokkaido area, I quickly found some power poles in Sapporo that where similar. 
5. Looked around the city and triangulated to find the same block number: ```73```as the original image.
6. Once I found it, I had to analyze the image to find the correct street.
	1. The image displays two roads with two houses in between, and some open filed behind.
	2. And I found this: ![[Pasted image 20251102145652.png]]
	3. The pole in the street view confirmed it was the same pole ![[Pasted image 20251102145914.png]]
7. I had to be extremely accurate with the coordinates, so I broke down the perspective from the image and using those coordinates.
	1. ![[Screenshot 2025-11-02 at 12.33.41.jpg]]
	2. But this was wrong. And asked a admin that said it was second floor near the window. 
		1. ![[Screenshot 2025-11-02 at 15.03.36.jpg]]
	3. After trying basically every coordinates in the house I found it: ```43.06743, 141.29253```, so the middle of the house.
		1. ![[Screenshot 2025-11-02 at 15.12.31.jpg]]
		2.  This also destroyed my solve percentage. ![[Pasted image 20251102151628.png]]
# Flag: v1t{43.06743,141.29253}