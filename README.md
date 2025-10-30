# Ex.No.6 Development of Python Code Compatible with Multiple AI Tools

# Date:  30 /10 /2025
# Register no. 212224040358
# Aim:
Write and implement Python code that integrates with multiple AI tools to automate the task of interacting with APIs, comparing outputs, and generating actionable insights with Multiple AI Tools

# AI Tools Required: 
ChatGPT,Google gemini..

# Explanation:
Experiment the persona pattern as a programmer for any specific applications related with your interesting area. 
Generate the outoput using more than one AI tool and based on the code generation analyse and discussing that. 

# Output:

##  **Title:**

**Framing Prompts for AI-Assisted Project Coding**


## **Objective:**

To help students learn how to **ask the right questions (prompts)** to get useful help from AI tools in coding.
By doing this, students will:

* Understand how to get AI to write Python code for APIs.
* Compare results from different APIs.
* Ask AI to explain and give insights based on data.

---

##  **Exercise Description:**

Instead of writing full code themselves, students will **create prompts** that guide AI tools to do the coding and explain the logic clearly.

They will go through **three stages** — (1) generating code, (2) comparing data, and (3) finding insights.

---

### **Stage 1 – Code Generation**

🧠 **Prompt 1:**

> Write Python code that gets current weather data from one API and a random joke from another API. Show both results clearly with short explanations.

**AI’s Expected Response:**

```python
import requests

# Get weather data (using open-meteo free API)
weather = requests.get("https://api.open-meteo.com/v1/forecast?latitude=13.08&longitude=80.27&current_weather=true").json()

# Get a random joke
joke = requests.get("https://official-joke-api.appspot.com/random_joke").json()

print(" Weather Details:", weather["current_weather"])
print(" Joke of the Day:", joke["setup"], "-", joke["punchline"])
```

**Explanation:**

* `requests` is used to connect with APIs.
* One API gives live weather data, another gives jokes.
* Results are shown using simple `print()` statements.

 **Learning Point:**
Good prompts ask AI to **explain each step**, not just show the code.

---

###  **Stage 2 – Comparison and Analysis**

🧠 **Prompt 2:**

> Write code that compares temperature from two APIs — one gives Celsius and another gives Fahrenheit. Convert both to the same unit and tell if they match.

**AI’s Expected Response:**

```python
# Temperatures from two imaginary APIs
api1_temp_c = 30
api2_temp_f = 86

# Convert Fahrenheit to Celsius
converted_temp = (api2_temp_f - 32) * 5/9

print("API 1:", api1_temp_c, "°C")
print("API 2 (converted):", round(converted_temp, 2), "°C")

if abs(api1_temp_c - converted_temp) < 1:
    print(" Both APIs give almost the same temperature.")
else:
    print(" There is a clear difference between API results.")
```

**Explanation:**

* The code changes Fahrenheit to Celsius for fair comparison.
* If both results are close, we can trust both APIs.
* If not, we should check which one is updated more recently.

 **Learning Point:**
A good comparison prompt tells AI *what to compare* and *how to decide* if results match.

---

###  **Stage 3 – Insight Generation**

🧠 **Prompt 3:**

> Based on temperature differences from the two APIs, explain why the values might not match and suggest how to make results more accurate.

**AI’s Expected Response:**

```
The temperature difference can happen because:
- APIs may use different data sources or update times.
- Some APIs round values differently.
- Geographic coordinates might not match exactly.

To improve accuracy:
- Use multiple APIs and take the average.
- Check the update time of each API.
- Verify with a local sensor or weather station.
```

**Explanation:**

This shows how AI can give **meaningful insights**, not just code.
It helps students see how to use AI for analysis and reasoning.

 **Learning Point:**
 
If your prompt asks AI to “explain why” or “suggest next steps,” you’ll get deeper answers.

---


---

###  **Example Reflection**

> My first prompt only gave code, not explanations. When I added “explain each step,” the output became much clearer.
> The comparison code worked well, and I learned how to convert units.
> I realized detailed prompts make AI respond more intelligently.

---





# Conclusion:


This exercise helps you learn how to ask AI the right questions to get useful code for your project. Instead of writing code directly, you practice giving clear, step-by-step prompts to generate Python code, compare API results, and get smart suggestions. By doing this, you become better at using AI as a coding partner.



# Result: 
The corresponding Prompt is executed successfully.
