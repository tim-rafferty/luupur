# Luupur

Generative groove machine with included looper and sampler.

**Description:**  
Inspired by PromptDJ and PromptDJMidi with the same core sequencer and beat-making interface, but add:  
- A looped audio playback system (import or record audio)  
- A drum machine sequencer  
- A sample pad player for triggering custom sounds  

---

## Key Features

### 1. Drum Machine Sequencer
- 16-step grid (expandable to 32 steps per generative track)  
- Multiple drum kits (kick, snare, hi-hat, percussion)  
- Tempo control (BPM slider)   
- Swing adjustment
- Odd timing adjustments

### 2. Looping Audio System
- Upload MP3/WAV files (max 10MB) or record via microphone  
- Waveform display with draggable start/end loop markers  
- Loop playback in sync with BPM (quantized start/end)  
- Up to 4 simultaneous loop tracks  

### 3. Sample Player Pads
- 8 trigger pads  
- Assign uploaded samples to pads  
- Trigger by mouse click, keyboard keys, or MIDI input  
- Low latency playback (<50ms)  

### 4. Playback & Project Management
- Play, Stop, Reset controls  
- Master volume slider  
- Export full mix as WAV/MP3  
- Save/load projects to LocalStorage (optional cloud save with Firebase/Supabase)  

---

## Technical Requirements
- **Frontend:** HTML5, CSS3, JavaScript (React or similar)  
- **Audio Engine:** Web Audio API + Tone.js for sequencing, loop sync, and sample playback  
- **File Handling:** Drag-and-drop + file picker  
- **Recording:** Web Audio API microphone input  
- **Storage:** LocalStorage for offline saves; optional Firebase/Supabase for cloud saves  
- **Responsive Design:** Works on desktop and mobile browsers  

---

## UI Layout
- **Top:** Transport controls (Play, Stop, BPM, Swing, Volume)  
- **Middle:** Sequencer grid for drums  
- **Bottom Left:** Looping section with waveform view + markers  
- **Bottom Right:** Sample pad grid (8 pads)  
- Tooltips for all interactive controls  

---

## User Flow Example
1. User loads the app and sees sequencer + empty loops + pads.  
2. Selects a drum kit and places beats on the grid.  
3. Uploads or records an audio loop, sets start/end markers.  
4. Adds samples to pads and plays them live.  
5. Loops and samples stay in sync with the drum machine.  
6. Exports the project as a WAV/MP3 or saves it for later.  

---

## Stretch Goals (Optional)
- MIDI mapping for external controllers  
- Basic effects (delay, reverb, filter)  
- Shareable project links  
- Real-time multiplayer via WebRTC  

