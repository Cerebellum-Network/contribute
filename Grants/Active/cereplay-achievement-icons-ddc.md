# CerePlay Games SDK Enhancement: Custom Achievements & UI Themes

- **Proposer:** [Your Organization Name](Link)
- **Payment Address:** [Your Payment Address]

## Project Description

[Your Organization Name] is offering an enhancement to the Cere Gaming SDK to enable the tracking of in-game activities and achievements. This upgrade is inspired by the desire to allow gamers to view unique achievement icons on the leaderboard based on specific in-game events. For instance, if Player A eliminates 100 enemies in the game, leading in the "Enemies Killed" category, a distinct achievement icon should be displayed on the leaderboard. This icon represents a special achievement, not necessarily the 1st place.

## Use-Case
Scenario: As a gamer, when I achieve specific milestones in a game, I want to see a unique achievement icon on the leaderboard, distinct from the regular 1st, 2nd, or 3rd place icons.
Example: If Player A eliminates 100 enemies in a game and leads in the "Enemies Killed" category, the leaderboard should display a special achievement icon for Player A, signifying this accomplishment.

Key features to be added include:
1. Enhancement of Cere Gaming SDK to monitor in-game actions and achievements.
2. Display of achievement icons on the leaderboard when players meet certain criteria (e.g., highest number of kills, most levels completed).
3. Introduction of new SDK methods for transmitting custom/system events in the form of arbitrary JSON data.

## Requirements
Enhance the Cere Gaming SDK to support the tracking of custom in-game activities and achievements. The SDK should be capable of saving and retrieving JSON data, which can then be integrated into the Leaderboard UI. This will allow the leaderboard to showcase specific achievement icons based on custom events.

## Key Features
SDK Enhancement: Upgrade the Cere Gaming SDK to monitor custom in-game actions and achievements.
Achievement Display: Show achievement icons on the leaderboard when a player meets predefined criteria.

* Store meta-data and digital asset data (png's) on DDC.
* User profiles should contain achievement data.
* Link icons with corresponding achievements.
* Make the leaderboard extendable to display more user profile data, especially achievement icons.
* Design considerations for displaying multiple achievements. 
 * Support multiple ahchievements.
 * Support clickable user profiles to reveal detailed achievements.
* It contains achievement icons saved to DDC and retrieved from DDC. 
 * Icons should be saved on user bases per the game. 
 * Achievements should be linked to the user and icon can be customizable. 
 * Leaderboard has to maintain extensions for user profiles in order to let this implementation to be done.



# **Read/Write/Update Achievement's on DDC with customer Leadeboard UI**

## Development Roadmap
- **Total Duration:** [Total Duration]
- **Total Costs:** [Total Cost]

### Milestone 1: SDK Method Enhancements
Achievements: Introduce new SDK methods to read/write/update custom 'achievement' events in the form of arbitrary JSON data. 

- **Estimated Duration:** [Duration]
- **Costs:** [Cost]

1. New SDK Methods: Introduction of new SDK methods for transmitting custom/system events in the form of arbitrary JSON data.
1. Data Validation: While the SDK should offer extension points for validation, developers must ensure data accuracy. For instance, discrepancies like a player claiming 3 hours of playtime in a 15-second session should be flagged.
2. Data Analysis: Events should be collected on the Cere side for future analysis, offering game developers potential restoration points. This data can also aid in constructing an analytics board for activity tracking.
3. Security Mechanism: The SDK should provide mechanisms to assist developers in performing security checks.

Example 1: 
``` 
{"fruits_collected": 10}
```

Example 2:
```
{
   "progress":{
      "achievements":{
         "cars_stolen": 1
      }
   }
}
```


### Milestone 2: Leaderboard UI Enhancements
Achievements: UI Components should should support showing achievements.

- **Estimated Duration:** [Duration]
- **Costs:** [Cost]

1. Customiazble UI: components to display the Leaderboard Screen data, which can encompass custom icons, font customizations, dialog box modifications, dynamic or static text, and animations.
2. Themes: Maintain a per-game config for uniform appearance across all game developer applications, with references like Metaverse Dash Run.

For example player1 killed 20 zombies and got achievement with zombie icon posted below, Leaderboard could look like the following:
 - ![image](./src/imgs/273535206-65a36558-6fc8-4494-af7d-d3952b887b0a.png)
 - ![image](./src/imgs/273535618-bdc260d3-2089-4793-90f2-9c2bfaa91865.png)

## Community engagement

1. Publish articles on our Blog, Telegram, Discord, and other community channels to highlight each milestone.

### Repository Hierarchy
```
├── ./ [CerePlay SDK Root]
│   ├── ./SDK Method Enhancements
│   ├── ./Leaderboard UI Components
│   ├── ./External Dependencies
```

Repository contains these primary directories:
1. SDK Method Enhancements: Contains tools and scripts for enhancing the SDK to support custom events and achievements.
2. Leaderboard UI Components: Modules for upgrading the UI components of the leaderboard.
3. External Dependencies: Information and updates related to external dependencies like Freeport API/docs.
## Team

- **Team Members:** [Member 1], [Member 2], [Member 3]
- **Team Website:** [Team Website Link]
- **Code Repos:** [Repository Link]
- **Website:**	[Organization Website]
- **Legal Structure:** [Legal Structure Type]
- **Team's Experience:** Brief descriptions of team members' experiences and contributions.

## Additional Information

Relevant additional information:

- **Work Done So Far:** [Description of the work that has been completed.]
- **Previous Contributions:** [Information about any teams or entities that have financially contributed to the project.]
- **Other Grants:** [Information about any other grants applied for or received.]
