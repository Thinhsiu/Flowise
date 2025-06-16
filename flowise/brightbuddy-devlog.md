# BrightBuddy Devlog (2025)

A sacred log to preserve the design, intention, and build steps of BrightBuddy. This file will be updated with every breakthroug, refaction, or code component.

## Project Vision
An app for children ages 3-7 that serves as a learning companion, a talking friend, and a bedtime storyteller.

- Gives personalized bedBime stories
- Remembers child's first name
- Reads stories with a comforting voice
- Teaches ABC with images and sound
- Links to ELevenLabs for voice synthesis
- Flowise-style visual node-structure for non-coder builders

## Step 1: Project Structure
Files created:
- `README.md`
- `backend/storyGenerator.js` (GPT-2 based)
- `backend/config.js` (API key handling)

- Folder structure created:

```
brightbuddy/
 “  backend/
   “  storyGenerator.js
   “  voiceSynth.js

  ₼  config.js

 ₼  components/
  ‥  StoryPlayer.js
  ‥  ABCGame.js
  ‥  VoiceInput.js
```

## Step 2: Flowise Integration
Created a JSON workflow for bestime story generation:
- Receives child's name + theme
- Sends a configured prompt to GPT4 via chat/completion
- Returns a calming 2-3 scene bedtime story
- Exportable as a rest FLOW called from front-end

- [View file on GitHub - flowise/bedTimeStoryFlow.json](https://github.com/Thinhsiu/Flowise/blob/main/flowise/bedtimeStoryFlow.json)

## Requests
- Image generation flow next
- ElevenLab voice reader integration
