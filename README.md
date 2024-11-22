# 📦 Bellande Limit Models & Executables

# Demo of Bellande Limit
![Demo GIF](executable/bellande_limit.gif)

## 🧙 Organization Website
- [![Organization Website](https://img.shields.io/badge/Explore%20Our-Website-0099cc?style=for-the-badge)](https://robotics-sensors.github.io)

## 🧙 Organization Github
- [![Organization Github ](https://img.shields.io/badge/Explore%20Our-Github-0099cc?style=for-the-badge)](https://github.com/Robotics-Sensors)

# Author, Creator and Maintainer
- **Ronaldson Bellande**

## Usage
```
./Bellande_Limit passcode node0 node1 environment size goal obstacles search_radius sample_points
```

### Arguments
1. `passcode`: The access key (must be "bellande_limit_executable_access_key")
2. `node0`: Starting point coordinates as a Python list (e.g., "[0, 0, 0]")
3. `node1`: Target point coordinates as a Python list (e.g., "[100, 100, 100]")
4. `environment`: Environment dimensions as a Python list (e.g., "[1000, 1000, 1000]")
5. `size`: Step sizes for each dimension as a Python list (e.g., "[10, 10, 10]")
6. `goal`: Goal point coordinates as a Python list (e.g., "[200, 200, 200]")
7. `obstacles`: List of obstacles with position and dimensions (e.g., '[{"position":[50,50,50],"dimensions":[20,20,20]}]')
8. `search_radius`: Float value for obstacle detection radius (default: 50.0)
9. `sample_points`: Integer number of sampling points (default: 20)

### Example
```
./Bellande_Limit "bellande_limit_executable_access_key" "[0,0,0]" "[100,100,100]" "[1000,1000,1000]" "[10,10,10]" "[200,200,200]" '[{"position":[50,50,50],"dimensions":[20,20,20]}]' 50 20
```

### Notes
- Passcode must be exactly "bellande_limit_executable_access_key"
- All coordinate lists must have the same dimensions as the environment
- Obstacle positions and dimensions must match environment dimensions
- Use proper Python list syntax for coordinates and obstacles
- The script supports infinite dimensions, limited only by system resources
- All numeric values can have decimal precision

### Error Handling
The script includes error handling for:
- Incorrect number of arguments
- Invalid passcode
- Mismatched dimensions across coordinates
- Invalid input format (syntax errors)
- Other unexpected errors

## License
This Algorithm or Models is distributed under the [Creative Commons Attribution-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-sa/4.0/), see [LICENSE](https://github.com/RonaldsonBellande/bellande_limit_models/blob/main/LICENSE) and [NOTICE](https://github.com/RonaldsonBellande/bellande_limit_models/blob/main/LICENSE) for more information.
