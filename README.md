# Music-AI

import random

music_db = { 
"happy": ["Blinding Lights - The Weeknd", "Levitating - Dua Lipa"], 
"sad": ["Someone Like You - Adele", "Fix You - Coldplay"], 
"energetic": ["Industry Baby - Lil Nas X", "Believer - Imagine Dragons"], 
"chill": ["Heat Waves - Glass Animals", "Peaches - Justin Bieber"]
}

def recommend_music(mood): 
mood = mood.lower() 
songs = music_db.get(mood, music_db["happy"]) 
print(f"🎵 I recommend this song for {mood}:") 
print(f"→ {random.choice(songs)}")

# Test
recommend_music("happy")
recommend_music("sad")
