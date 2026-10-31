# Purdue Meal Planner

A Java command-line tool that gets Purdue's daily dining menu, takes a users calorie/protein targets and any dietary restrictions, and tells you what to eat at each dining court + how many servings of each item.

## Project goal

Tracking calories and protein at Purdue's dining courts means checking each item's nutrition, multiplying by servings, and adding everything up by hand. Most students don't do this, so they either overshoot calories or fall short on protein. This tool does the math for you and suggests a meal plan that fits your own goals.

## MVP scope

The MVP is the simplest/smallest version that solves the problem end to end:

- Pull today's menu from the Purdue dining API
- Accept the user's daily calorie and protein targets and dietary restrictions
- Filter items by dietary restrictions
- Plan a meal with servings for each item, staying within the calorie target and meeting the protein target
- Print the plan, or the closest plan if the exact numbers can't be met

## Future plans

Planned for later versions:

- Track what you've already eaten and show remaining calories and protein
- Save daily and weekly nutrition history
- Save favorite items and multiple user profiles

## Tech stack

- **Language:** Java
- **HTTP:** `java.net.http.HttpClient` which is already built into Java
- **JSON parsing:** Gson
- **Testing:** JUnit
- **Data source:** Purdue HFS dining API 
- **Output:** Plain text to the terminal and optional file download

## Design documents

- [System flowchart](docs/flowchart.png)
- Eisenhower matrix and tech stack are in the design doc in `docs/`

