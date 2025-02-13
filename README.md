# Solar System Simulation 🌎 🌍 🌏

A Python-based solar system simulation using PyGame that accurately models planetary orbits based on gravitational forces.

## ✨ Features

- Real-time planetary motion simulation
- Gravitational force calculations between celestial bodies
- Distance tracking from the Sun
- Orbital path visualization
- Accurate scaling of astronomical units
- Multiple planets including:
  - Sun (central body)
  - Mercury
  - Venus
  - Earth
  - Mars

## 🔧 Physics Implementation

The simulation implements several key astronomical and physical concepts:
- **Gravitational Force**: Uses Newton's law of universal gravitation (G = 6.67428e-11)
- **Astronomical Unit**: Accurately scaled distances (1 AU = 149.6e6 km)
- **Velocity Calculations**: Realistic orbital velocities for each planet
- **Time Scaling**: One day per timestep (3600*24 seconds)

## 🛠️ Technical Details

### Constants
```python
AU = 149.6e6 * 1000  # Astronomical Unit in meters
G = 6.67428e-11      # Gravitational constant
SCALE = 250 / AU     # Pixel scaling (1AU = 100 pixels)
TIMESTEP = 3600*24   # One day per simulation step
```

### Planet Properties
| Planet  | Mass (kg)        | Orbital Velocity (km/s) | Color     |
|---------|------------------|------------------------|-----------|
| Sun     | 1.98892 × 10^30 | -                      | Yellow    |
| Mercury | 3.30 × 10^23    | 47.4                   | Dark Grey |
| Venus   | 4.8685 × 10^24  | 35.02                  | White     |
| Earth   | 5.9742 × 10^24  | 29.783                 | Blue      |
| Mars    | 6.39 × 10^23    | 24.077                 | Red       |

## 🚀 Getting Started

1. Install Python 3.x
2. Install PyGame:
```bash
pip install pygame
```

3. Clone the repository:
```bash
git clone https://github.com/yourusername/solar-system-simulation.git
cd solar-system-simulation
```

4. Run the simulation:
```bash
python solar_system.py
```

## 🎮 Controls

- Close window to exit simulation
- Simulation runs automatically once started
- Orbits are traced automatically

## 🖥️ Display Features

- 800x800 pixel window
- Planet sizes scaled for visibility
- Distance from Sun displayed in kilometers
- Orbital paths traced in planet's color
- Smooth 60 FPS animation

## 🧮 Classes and Methods

### Planet Class
- **Attributes**:
  - Position (x, y)
  - Radius
  - Color
  - Mass
  - Velocity (x_vel, y_vel)
  - Orbit path tracking

- **Methods**:
  - `draw()`: Renders planet and orbit path
  - `attraction()`: Calculates gravitational forces
  - `update_position()`: Updates planet position based on forces

## 📝 Dependencies

- Python 3.x
- PyGame
- Math module (standard library)

## 🤝 Contributing

Contributions are welcome! Here are some ways you can contribute:
1. Add more planets
2. Implement additional physics calculations
3. Add interactive features
4. Improve visualization
5. Optimize performance

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🌟 Future Enhancements

- Add more planets (Jupiter, Saturn, etc.)
- Include moons and their orbits
- Add planet rotation
- Implement zoom functionality
- Add time controls (speed up/slow down)
- Include planetary data display

## ⚠️ Notes

- Planet sizes are not to scale (enlarged for visibility)
- Time is accelerated for better visualization
- Orbits are simplified (not accounting for all real-world factors)

---
Made with ❤️ using Python and PyGame
