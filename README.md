```markdown
# Game Character Stats Tracker

This project implements a `GameCharacter` class that models a game character with core attributes such as name, health, mana, and level. It provides functionality to create, update, and display character stats, along with leveling up mechanics.

---

## Features

- Create a game character with a specified name.
- Automatically initialized with:
  - Health: 100
  - Mana: 50
  - Level: 1
- Read-only access to character name.
- Controlled modification of health and mana with caps:
  - Health: 0 to 100
  - Mana: 0 to 50
- Level up method that increases level by 1, resets health and mana, and prints a message.
- String representation of character stats for easy display.

---

## Usage

```python
# Create a new character
hero = GameCharacter('Kratos')
print(hero)

# Modify stats
hero.health -= 30
hero.mana -= 10
print(hero)

# Level up the character
hero.level_up()
print(hero)
``

---

## Implementation Details

- **Initialization (`__init__`)**: Sets name, health, mana, and level.
- **Properties**:
  - `name`: Read-only.
  - `health` and `mana`: Getter and setter with bounds checking.
  - `level`: Read-only.
- **Methods**:
  - `level_up()`: Increases level, resets health and mana, and prints a message.
  - `__str__()`: Returns a formatted string of the character's current stats.

---

## Requirements

- Python 3.x

---

## License

This project is for educational purposes.

---

## Contributing

Contributions are welcome! Please fork the repository and submit a pull request.
