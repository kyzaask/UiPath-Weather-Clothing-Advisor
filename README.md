````markdown
# 🌤️ UiPath Weather Clothing Advisor

An RPA project developed with **UiPath Studio** that retrieves weather information for a selected city and recommends suitable clothing based on weather conditions and temperature.

## 📌 Overview

The **Weather Clothing Advisor** automates the process of checking weather conditions and providing a clothing recommendation.

The workflow:

1. Takes a city as input.
2. Searches for the city's weather information using Google.
3. Extracts the temperature and weather condition.
4. Checks whether it is raining.
5. If it is not raining, checks whether the temperature is very cold.
6. If it is not very cold, checks whether the temperature is very hot.
7. Assigns a suitable clothing recommendation.
8. Displays the city, temperature, and recommendation in a final Message Box.

## 🔀 Decision Logic

The workflow uses three main decisions:

### Is raining?
- **True** → Assign rain gear.
- **False** → Check if the temperature is very cold.

### Is it very cold?
- **True** → Assign a warm outfit.
- **False** → Check if the temperature is very hot.

### Is it very hot?
- **True** → Assign a hot-weather outfit.
- **False** → Assign a mild-weather outfit.

```text
                  Is raining?
                 /           \
              True           False
               ↓               ↓
        Assign rain gear   Is it very cold?
                           /             \
                        True             False
                         ↓                 ↓
                  Assign warm outfit   Is it very hot?
                                      /             \
                                   True             False
                                    ↓                 ↓
                              Assign hot outfit   Assign mild outfit
                                      \             /
                                       \           /
                                        ↓         ↓
                                      Final Message Box
````

## 🛠️ Technologies & Tools

* UiPath Studio
* RPA (Robotic Process Automation)
* VB.NET Expressions
* Web Automation
* Google Weather Search
* Type Into
* Click
* Get Text
* Assign
* Flow Decision
* Message Box

## 🌡️ Weather-Based Recommendations

| Weather Condition | Recommendation      |
| ----------------- | ------------------- |
| Rainy             | Rain gear           |
| Very cold         | Warm outfit         |
| Very hot          | Hot-weather outfit  |
| Mild              | Mild-weather outfit |

## 🎯 Project Purpose

This project was created to practice and demonstrate fundamental **RPA and UiPath concepts**, including:

* Web automation
* Data extraction
* Variables and data types
* VB.NET expressions
* Conditional logic
* Flowcharts
* Automation workflow design
* User interaction

## 📂 Project Structure

```text
UiPath-Weather-Clothing-Advisor/
│
├── Main.xaml
├── project.json
├── .gitignore
└── README.md
```

## 🚀 How to Run

1. Clone this repository.
2. Open the project in **UiPath Studio**.
3. Make sure the required UiPath packages are installed.
4. Open `Main.xaml`.
5. Run the workflow.
6. Enter a city when prompted.
7. The robot retrieves the weather information and displays a clothing recommendation.

## 📷 Workflow

The workflow follows a simple decision-based process:

**Weather → Temperature → Clothing Recommendation → Final Result**

## 👩‍💻 Author

**Büşra Turğut**


```
```
